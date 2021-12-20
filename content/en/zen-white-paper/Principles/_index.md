
---
categories: ["white paper"]
tags: ["principles", "values", "practices", "prototype", "object system", "installation", "composition", "GUI", "DOM", "API", "SVG", "Canvas", "Squeak", "AST", "visual programming", "sequential programming", "copy", "paste", "asynchronous", "event", "input", "I/O", "synchronize", "continuation", "Scheme", "interpreter", "JavaScript", "TTI", "scene graph", "CSS2", "visual formatting model", "CSS3", "A-grade web browser"]
title: "Principles"
linkTitle: "Principles"
weight: 5
date: 2017-01-04
description: >
  The principles of the Zen system.
type: docs
---

As pointed out by David Ungar (who pioneered the type of prototypal object system that JavaScript uses), from values derive principles and from principles derive practices.{{< fnref 35 >}}<sup>, </sup>{{< fnref 36 >}} We have just explored the values behind the Zen system. Now let's examine the principles of the Zen system. Zen will complement the approach of Lively Kernel,{{< fnref 37 >}}<sup>, </sup>{{< fnref 38 >}} which shares Zen's principles 1–3 as listed below. How much, if any, of Lively Kernel's code it will borrow is yet to be determined. Note, in particular, the following principle 11 of Zen that is different than the principles of Lively Kernel:

1. It will run in any _browser_ without a download or installation. (Sometime in the future, an attempt might be made to make it work in mobile browsers.)
1. It will be a composition environment, a GUI builder.
1. It will store its apps as web pages.
1. It will compose web pages using the DOM's interfaces and APIs{{< fnref 39 >}}<sup>, </sup>{{< fnref 40 >}} but not SVG or Canvas drawing operations.
1. Zen will allow its composition objects and simple programs to be inspected and edited via a Squeak-like object inspector.{{< fnref 41 >}} Zen will, by default, hide its visual programming environment. When visual programming is enabled, Zen will use HTML elements like `DIV` to model nodes in the program's abstract syntax tree (AST).{{< fnref 42 >}} Zen will enable these program nodes or blocks to be copied, pasted, and rearranged, just like the ordinarily visible parts of a Zen web page.
1. It will enable its users to easily compose sequential programs, that is, programs that can wait for external, asynchronous events such as user input or I/O. Zen will synchronize its user's sequential programs through Scheme continuations in an interpreter running on top of JavaScript in the web browser. (See below.)
1. Zen will be loadable into any web page as a library, although caution will be required to ensure compatibility.
1. It will *complement*, *augment*, and *interact* with existing web page editors and website builders, not replace them.
1. It will allow the Zen-editing of a web page to be locked, leaving intact the form and behavior it built inside the web page.
1. Zen will not add more than 1&ndash;3 seconds to a web page's TTI (time to interact).
1. Zen will not follow Lively Kernel's principle of implementing a scene graph.{{< fnref 37 >}} Instead, it will leverage the CSS2 visual formatting model{{< fnref 43 >}} and CSS3 features implemented by A-grade web browsers{{< fnref 44 >}} to model a document in a web browser.
