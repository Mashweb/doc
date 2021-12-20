---
categories: ["white paper"]
tags: ["website builder", "wcms", "cms", "wix.com", "weebly.com", "business type", "template", "plugin", "module", "font", "element", "node", "NodeList", "DOM", "grab", "drag", "metaphor", "drag-and-drop", "DMI", "direct manipulation", "interface", "move", "coordinate", "cut and paste", "block", "inline", "inline-block", "none", "live demo", "demo", "experiment", "15 puzzle", "JavaScript", "html", "css", "comment system", "forum", "wiki", "casual author"]
title: "Zen vs. website builders"
linkTitle: "Zen vs. website builders"
weight: 2
date: 2017-01-05
description: >
  How Zen will avoid the problems of current website builders.
type: docs
---

It is important to characterize and visualize how Zen will be different from "website builders" and WCMSs like Wix.com and Weebly.com. In contrast to such WCMSs, which prescribe construction methods at the level of business type, templates, plugins, modules, fonts, etc., Zen will give the user ultimate control of detail at the element/node/NodeList level of web pages. Zen will allow a DOM node to be grabbed and "dragged" to different positions in its containing NodeList because this is the simplest metaphor for that operation. Drag-and-drop is a classic feature of direct-manipulation interfaces (DMIs) and this metaphor of "moving" an HTML element or node is so compelling that we have to look at the code to see that the element has not moved in terms of x and y coordianates, but rather in terms of its cardinal position in a NodeList. Zen will allow a DOM node to be "cut and pasted" to any valid position in the DOM—an interaction between multiple NodeLists. An HTML element's style has four possible, well-supported values for its display property: block, inline, inline-block, and none. Live demo code to implement GUIs to rearrange element positions in the NodeLists of the first three of these display styles is located on the author's GitHub Pages here, here, and here. (Right-click on the links to open the pages in new tabs or windows.) The method of sliding elements in these prototype GUIs was partly inspired by the 15 Puzzle and JavaScript-based implementations of the 15 Puzzle. There are notes about some of these implementations on this website. Below is a screen recording of Jamie Wong's AI-based automated 15-Puzzle solver, which is written solely in JavaScript, HTML, and CSS (Figure 13).

{{< figure src="/images/15-puzzle.gif" title="Figure 13. Jamie Wong's 15-Puzzle solver." target="_blank" >}}

Presently, the customization of templates, plugins, and modules for website builders and web CMSs and the creation of novel comment systems, forums, wikis, and presently unimagined communication systems are far outside the bounds of casual web authorship.
