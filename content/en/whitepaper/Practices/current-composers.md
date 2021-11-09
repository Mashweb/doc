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

Zen will take a different approach. In Zen, HTML elements making up the web page will represent themselves at the top-level view, with all the obscurity of detail that implies, but when Zen's _node browser_ is open, Zen will be show a view of the web page with all borders and margins styled in such a way that, to the extent possible, all _block boxes_, _inline boxes_, and _inline-block boxes_<sup><a href="#21">21</a></sup> are visible (Figure 7).
{{< figure src="/images/node-browser-cropped.png" title="Figure 7. Screenshot of a node-browser prototype. Click to open the live demo in a new window." link="/demos/" target="_blank" >}}

Other display styles besides _block_, _inline_, and _inline-block_ will be modeled by Zen in a subsequent release. Zen will provide whatever kinds of object-browsers are necessary to unobscure details of the page-as-an-object. Although the details have not yet been worked out, hope and inspiration are provided by the <a href="https://developer.mozilla.org/en/docs/Tools/3D_View" target="_blank">3D View tool</a>, and by the <a href="https://addons.mozilla.org/en-US/firefox/addon/tilt/" target="_blank">Tilt 3D add-on</a>, for the Firefox browser (Figures 8a and 8b). These screenshots are not meant to represent the paradigm that Zen will use.

{{< figure src="https://developer.mozilla.org/en-US/docs/Tools/3D_View/3dview.png" title="Figure 8a. Screenshot of the Firefox 3D View tool for Firefox versions prior to Firefox 47." >}}

{{< figure src="https://wiki.mozilla.org/images/5/5f/Tilt.png" title="Figure 8b. Screenshot of the Tilt 3D Add-on for Firefox." >}}

The user will be able to select any node that can be the target of a mouse event. In node-selection mode, passing the mouse pointer over nodes will highlight them one at a time (Figure 9).

{{< figure src="/images/layout-manipulator.gif" title="Figure 9. Layout-manipulator prototype. Click to open the live demo in a new window." link="/demos" target="_blank" >}}

When the user wants to add an HTML element to his web page, Zen will first present a choice of block, inline, and inline-block box types, because in Zen's paradighm, the visual behavior of a box is mainly determined by its display style, not by HTML tag type. This is demonstrated by the [w3schools.com]({{< ref "https://www.w3schools.com" >}} )'s "Tryit Editor" page for converting <code>&lt;li&gt;</code> HTML elements into a <a href="http://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_horizontal">horizontal navigation bar</a>.

<a href="www.w3schools.com">w3schools.com's</a> "Tryit Editor" page for converting <code>&lt;li&gt;</code> HTML elements into a <a href="http://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_horizontal">horizontal navigation bar</a>. Using Zen's paradigm, with virtually zero learning, the user could intuitively mock up a web page using only <em>block</em>, <em>inline</em>, and <em>inline-block</em> boxes, and convert it piece by piece into semantic markup. Or he could set the HTML element tag of each element immediately when adding it to the web page.
