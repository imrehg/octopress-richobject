Social meta tags for Octopress
==============================

Plugin to provide the necessary changes to enable rich objects for the
given site. Currently aiming to cover the following:

* [Open Graph][og]
* [Rich Snippets][rs]

This mostly means adding extra meta tags and other things.

Documentation
=============

Add `richobject.html` to `source/_includes/custom`, and edit `source/_includes/head.html` to add this line
just before the closing `</head>` tag:

    {% include custom/richobject.html %}

To have correctly filled out fields, add these new properties to every new post you make (for description
and cover image URL):

    description:
    cover:

Also, in `_config.yaml` fill out the `description:`, and add a `cover:` property.

Testing tools
=============

* [Facebook debugger][fdebug] for the Open Graph tags
* [Rick Snippets Testing Tool][rstt], from Google Webmaster Tools

 [og]: http://ogp.me/ "The Open Graph protocol"
 [rs]: http://support.google.com/webmasters/bin/answer.py?hl=en&answer=99170 "Google Rich Snippets documentation"
 [fdebug]: https://developers.facebook.com/tools/debug "Facebook debugger"
 [rstt]: http://www.google.com/webmasters/tools/richsnippets "Rich Snippets Testing Tool"
