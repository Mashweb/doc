
---
title: "Initial Questions and Ideas for Zen Development"
linkTitle: "Initial Questions and Ideas for Zen Development"
weight: 7
date: 2017-01-05
description: >
  Now we shall make our first foray into describing Zen. How do we propose to solve the problems listed in "Introduction"?
type: docs
---

Which of the following do we want to focus upon?

1. A Lego-like construction kit, basically for building a Website (or web page) from scratch? Such a construction kit would concentrate upon a tall stack of capabilities based upon a narrow, "opinionated" trunk of foundational technologies. Examples of the foundational technologies could be a CSS framework like Bootstrap or Foundation, a CSS grid system like 960 Grid System, a CSS framework oriented to working with web components, components from customelements.io or webcomponents.org, and widgets from ExtJS or the Dojo Toolkit.
1. A tool kit for creating or modifying web pages? Such a tool kit would concentrate upon the broadest possible comprehension of different kinds of web components in the broadest meaning of the term—including JavaScript-based widgets. Such a tool kit could not reasonably be made to comprehend attached JavaScript, but could understand the protocols of JavaScript-based widget libraries to intervene in and interact with the lifecycle of widgets. Such a tool kit could not reasonably comprehend other JavaScript, but could leave that JavaScript untouched. Such a tool kit could not reasonably be able to add useful, arbitrary JavaScript to a web page, but could add a very broad class of visually programmed functions as described later in this white paper.

Whichever path we choose—the creation of an isolated silo of technology or the utility belt of tools—there are some data-wrangling capabilities it seems Web users should be getting for free, but aren't. These could be part of a Zen Manifesto:

1. Simple copying, cutting, and pasting of text, images, HTML components, and widgets should be possible. It should be possible to save various versions of these copied or cut items in a repertoire of patterns—with or without the text and images, with or without style classes, with or without style overrides. It should be possible to add parameters to the patterns so they can be used to easiy add to the Web. The patterns should be stored in a version control system that makes branching of versions very easy, as Git{{< fnref 52 >}} does.
1. The Web user should have the ability to create spreadsheets (like Google Sheets{{< fnref 53 >}} via simple drag-and-drop. It should be possible to drag and drop whole cells, rows, and tables without even double-clicking and swiping the mouse pointer across words. These spreadsheets should be able to include images.
