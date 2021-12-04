---
title: "Zen vs. current WYSIWYG and WYSIWYM web-page composers"
linkTitle: "Zen vs. current web-page composers"
weight: 1
date: 2017-01-05
description: >
  How Zen will avoid the problems of current WYSIWYG and WYSIWYM composers.
type: docs
---
Present-day WYSIWYG and WYSIWYM web-page composers immediately confront the user with web-page structure details, requiring the user to prematurely optimize his web page. With these composers, the web-page under construction is dominated by a pallette of HTML elements with which the user can "paint" a web page. Some of these composers offer the user a view of the web page that is strewn with icons representing HTML elements.

Zen will take a different approach. In Zen, HTML elements making up the web page will represent themselves at the top-level view, with all the obscurity of detail that implies, but when Zen's _node browser_ is open, Zen will be show a view of the web page with all borders and margins styled in such a way that, to the extent possible, all _block boxes_, _inline boxes_, and _inline-block boxes_{{< fnref 33 >}} are visible (Figure 7).
{{< figure src="/images/node-browser-cropped.png" title="Figure 7. Screenshot of a node-browser prototype. Click to open the live demo in a new window." link="/demos/" target="_blank" >}}

Other display styles besides _block_, _inline_, and _inline-block_ will be modeled by Zen in a subsequent release. Zen will provide whatever kinds of object-browsers are necessary to unobscure details of the page-as-an-object. Although the details have not yet been worked out, hope and inspiration are provided by the <a href="https://developer.mozilla.org/en/docs/Tools/3D_View" target="_blank">3D View tool</a>, and by the <a href="https://addons.mozilla.org/en-US/firefox/addon/tilt/" target="_blank">Tilt 3D add-on</a>, for the Firefox browser (Figures 8a and 8b). These screenshots are not meant to represent the paradigm that Zen will use.

{{< figure src="https://developer.mozilla.org/en-US/docs/Tools/3D_View/3dview.png" title="Figure 8a. Screenshot of the Firefox 3D View tool for Firefox versions prior to Firefox 47." >}}

{{< figure src="https://wiki.mozilla.org/images/5/5f/Tilt.png" title="Figure 8b. Screenshot of the Tilt 3D Add-on for Firefox." >}}

The user will be able to select any node that can be the target of a mouse event. In node-selection mode, passing the mouse pointer over nodes will highlight them one at a time (Figure 9).

{{< figure src="/images/layout-manipulator.gif" title="Figure 9. Layout-manipulator prototype. Click to open the live demo in a new window." link="/demos" target="_blank" >}}

When the user wants to add an HTML element to his web page, Zen will first present a choice of block, inline, and inline-block box types, because in Zen's paradighm, the visual behavior of a box is mainly determined by its display style, not by HTML tag type. The priority of display style over tag type in the visual behavior of a box  is illustrated by the [w3schools.com](https://www.w3schools.com)'s "Tryit Editor" page for converting <code>&lt;li&gt;</code> HTML elements into a [horizontal navigation bar](http://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_horizontal). Using Zen's paradigm, with virtually zero learning, the user could intuitively mock up a web page using only _block_, _inline_, and _inline-block_ boxes, and convert it piece by piece into semantic markup. Or he could set the HTML element tag of each element immediately when adding it to the web page.

Zen will allow the user to inspect and manipulate these boxes in a way pioneered and developed by Smalltalk and Smalltalk variants, using inspectors and browsers to inspect live web-page objects. For a relatively gentle introduction to Smalltalk-style inspectors and browsers, see Cincom Smalltalk's tutorials (Figures 10 and 11). The specific HTML tag of an HTML element will be a detail to be drilled down to rather than a primary detail of interest.

{{< figure src="/images/Inspector.jpeg" title="Figure 10. Cincom Smalltalk Inspector Tool overview tutorial video. Click to open in a new window." link="https://www.youtube.com/watch?feature=player_embedded&v=N55hT-abBaA" target="_blank" >}}

{{< figure src="/images/Browser.png" title="Figure 11. Cincom Smalltalk Browser Tool overview tutorial video. Click to open in a new window." link="https://www.youtube.com/watch?feature=player_embedded&v=9e5UI_PMGEM" target="_blank" >}}

Zen will take an embedded, instant-feedback, hybrid WYSIWYM-WYSIWYG (not "pure" WYSIWYG) approach to pull the authoring of novel, Semantic-Web applications out of the exclusive province of programmer-specialists and put it into the hands of amateurs and dilettantes (in the original, non-pejorative sense of the words). The Zen project will primarily focus upon working with the "purest" web technologies—HTML and CSS—rather than backend technologies like web servers and web frameworks, because the back-end web framework or web server is opaque to JavaScript running in the web page. That is, the JavaScript running in the page has no way to affect the operation of the back end unless specific arrangements have been made for it. Zen will work by providing updates to web-page source in some format. Where web-page source is persisted and how it is used to generate the web page Zen is embedded in will not be the concern of Zen, though a reference implementation for that will be developed along with Zen.

In spite of these strict limitations, Zen as a building block for web servers and web frameworks is anticipated to be a game-changing addition to present-day website and web-app techniques. In some cases, Zen might even be developed to itself reflect changes to content, structure, and style back to sources, using a bit of code on the back end (i.e. on the web server). Perhaps, for example, in WebDAV-enabled websites—Zen could relatively easily be leveraged to rewrite web-page source, including stylesheets. On the other hand, using Zen only as a low-level, embedded, solid building block, it should be possible to augment web frameworks of many types to achieve a new, higher level of interactivity and customization in web applications.

None of the well-known WYSIWYG and WYSIWYM page editors directly support the creation of web applications. The most radical aspect of Zen will be that it will allow simple, sequential programs to be created and edited using a block representation of the program's abstract syntax tree (AST),{{< fnref 34 >}} where blocks can be moved around using the same user interface Zen will provide for moving web page elements, with minimal modifications. Zen will accomplish this unusual feat by implementing a version of Scheme language in JavaScript, along with _true_ continuations,{{< fnref 34 >}} various supporting functions written in JavaScript, and some resources like icons. The author has already used such continuations to string together JavaScript event handlers to create a small sequential program without resorting to callbacks, continuatinon-passing style, promises, or state machines. Scratch{{< fnref 35 >}} and Snap!{{< fnref 36 >}} (formerly called BYOB) demonstrate that even young children can program using a cleverly designed visual programming language (Figure 12).

{{< figure src="/images/snap.png" title="Figure 12. The Snap! visual programming language. Click to open in a new window." target="_blank" >}}
