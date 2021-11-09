
---
title: "Principles"
linkTitle: "Principles"
weight: 5
date: 2017-01-04
description: >
  The principles of the Zen system.
type: docs
---

As pointed out by David Ungar (who pioneered the type of prototypal object system that JavaScript uses), from values arise principles and from principles arise practices.<sup><a href="#13">13</a>, <a href="#14">14</a></sup> We have just explored the _values_ behind the Zen system. Now let's explore the _principles_ of the Zen system. Zen will complement the approach of Lively Kernel,<sup><a href="#15">15</a>, <a href="#16">16</a></sup> which shares Zen's principles 1&ndash;3 as listed below. How much, if any, of Lively Kernel's code it will borrow is yet to be determined. Note, in particular, the following principle 11 of Zen that is different than the principles of Lively Kernel:
1. It will run in any _browser_ without a download and without installation. (Sometime in the future an attempt might be made to make it work in mobile browsers.)
1. It will be a composition environment, a GUI builder.
1. It will store its apps as web pages, even new versions of itself.
1. It will use only the DOM's interfaces and APIs<sup><a href="#17">17</a>, <a href="#18">18</a></sup> for the composition of web pages and web GUIs by element _insertion_, _manipulation_, _editing_, and _deletion_&mdash; as opposed to _drawing_ objects using SVG or Canvas operations.
1. Zen will not provide IDEs, but instead will allow objects in its compositions to be inspected and edited via a Squeak<sup><a href="#19">19</a></sup>-like object inspector.  Zen will allow its simple programs to be inspected and edited in a normally hidden visual programming environment, using HTML elements like DIV to model nodes in the program's abstract syntax tree (AST).<sup><a href="#20">20</a></sup> Zen will enable these program nodes or blocks to be copied, pasted, and rearranged, just like the normally visible parts of a Zen web page.
1. It will enable its users to easily compose sequential programs, that is, programs that can wait for external, asynchronous events such as user input or I/O. This will be accomplished by instantiating ntrue continuations_ in an interpretter running on top of JavaScript in the web browser. (See below.)
1. It will exist as a library that can be loaded into any web page to provide the page with Zen's capabilities, although caution will be required to ensure compatibility.
1. It will _complement_, _augment_, and _interact_ with existing web-page editors and website builders, not replace them.
1. It will allow the Zen-editing of a web page to be locked, leaving intact the form and behavior it built inside the web page.
1. Zen will not add more than 1&ndash;3 seconds to the TTI (time to interact) for a web page.
1. Zen will not follow Lively Kernel's principle of implementing a scene graph.<sup><a href="#15">15</a></sup> Instead, it will honor the CSS2 visual formatting model<sup><a href="#21">21</a></sup> in its modeling of a document in a web browser.  Zen will not be able use SVG or Canvas graphics for the creation of objects, except where particular Zen-composed apps borrow the pertinent capabilities from other software systems.
