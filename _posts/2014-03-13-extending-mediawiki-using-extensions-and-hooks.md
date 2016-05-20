---
id: 2950
title: Extending MediaWiki using extensions and hooks
date: 2014-03-13T13:51:22+00:00
author: rtholmes
layout: post
guid: http://ucosp.ca/?p=2950
permalink: /winter-2014/2014/03/extending-mediawiki-using-extensions-and-hooks/
categories:
  - Winter 2014
---
Wen-Chien Chen from Waterloo fills us in on his work with MediaWiki extensions:

[MediaWiki](https://www.mediawiki.org/) is a versatile wiki software package written in PHP that powers websites where users write collaboratively. It is used in a variety of applications, from Wikipedia to the online documentation of Arch Linux. The extension architecture of MediaWiki allows it to adapt to the needs of different applications: while the core portion of the software is already powerful, it can be augmented with modular extensions. In particular, MediaWiki allows extensions to define hooks, and to register handlers for hooks defined in MediaWiki and other extensions. We used this feature to add the ability to send thank you notifications to other users for their comments on discussion boards powered by the [Flow extension](https://www.mediawiki.org/wiki/Extension:Flow), leveraging existing code in the [Thanks extension](https://www.mediawiki.org/wiki/Extension:Thanks).

On a Flow discussion board, each comment has several interaction links for editing, replying and other functionality. In the Flow extension, the code that generates the interaction links is similar to the following:

<pre style="tab-size: 4; white-space: pre-wrap;"><code>public function postInteractionLinks( $replyButtonClass, $editButtonClass ) {
	$items = array();

	// Generate the HTML code for reply and edit buttons and append them to $items
	$replyButton = $this-&gt;replyButton( $replyButtonClass );
	if ( $replyButton ) {
		$items[] = $replyButton;
	}
	$editButton = $this-&gt;editPostButton( $editButtonClass );
	if ( $editButton ) {
		$items[] = $editButton;
	}

	// Construct and return formatted HTML containing the interaction links
	return implode(
		Html::element(
			'span',
			array( 'class' =&gt; 'flow-post-interaction-separator' ),
			wfMessage( 'flow-post-interaction-separator' )-&gt;text()
		),
		$items
	);
}</code></pre>

To allow other extensions to add more links, we added a call to `wfRunHooks()` immediately before the return statement:

<pre style="white-space: pre-wrap;"><code>// $this-&gt;post refers to the comment and $this-&gt;user refers to the viewing user
wfRunHooks( 'FlowAddPostInteractionLinks', array( $this-&gt;post, $this-&gt;user, &$items ) );</code></pre>

`wfRunHooks()` is a global function in MediaWiki that calls each hook function registered to handle an event—in this case, one we just defined as `FlowAddPostInteractionLinks`. Multiple handlers, which would be called in sequence, can respond to the same event. The contents of the array are passed as arguments to the hook functions. Note that a reference to `$items` is passed in, in order to allow handlers to modify the items array.

In the Thanks extension, we added a static method to the `ThanksHooks` class. It handles the event by appending a link to `$items`, returning `true` on success:

<pre style="tab-size: 4; white-space: pre-wrap;"><code>public static function onFlowAddPostInteractionLinks( $post, $user, &$links ) {

	// Perform permission checks and other processing

	// Generate the HTML code for a thank buttons and append it to $items
	$links[] = Html::element(
		'a',
		array(
			'href' =&gt; $this-&gt;getThanksApiUrl( $post-&gt;getPostId ),
			'data-post-id' =&gt; $post-&gt;getPostId()
		),
		wfMessage( 'thanks-button-text' )-&gt;parse()
	);
	return true;
}</code></pre>

To register the method as a handler so that it would be called during the call to `wfRunHooks()`, we appended its name to the relevant entry in `$wgHooks`, which is an associative array that stores the handlers registered for each event. (In general, variables in MediaWiki with the `wg` prefix have global scope.) This was done by adding following line to `Thanks.php`, which contains setup instructions for the Thanks extension:

<pre style="white-space: pre-wrap;"><code>$wgHooks['FlowAddPostInteractionLinks'][] = 'ThanksHooks::onFlowAddPostInteractionLinks';</code></pre>

And that&#8217;s pretty much all that needs to be done to integrate the two extensions! After doing the above, a link for thanking the author will be appended to the interaction links for each comment. The hooks system makes it easy to add new functionality to MediaWiki and its extensions, and enables interaction between different parts of the software.

Aside from defining hooks ourselves by adding calls to `wfRunHooks()`, the core code of MediaWiki defines a number of events that extensions can respond to. A partial list is available at the [Hooks manual page](https://www.mediawiki.org/wiki/Manual:Hooks#Available_hooks).

In my time working with MediaWiki so far, I have found writing and modifying extensions to be a great way to learn about hacking MediaWiki. Aside from the hooks system described here, there are numerous other features in MediaWiki that simplify the work needed to create an extension. The [Developing extensions manual page](https://www.mediawiki.org/wiki/Manual:Developing_extensions) is a good starting point for learning about extension development, and [MediaWiki.org](https://www.mediawiki.org/), along with the [class reference](https://doc.wikimedia.org/mediawiki-core/master/php/html/), provides extensive documentation about the internals of the software. Happy hacking!