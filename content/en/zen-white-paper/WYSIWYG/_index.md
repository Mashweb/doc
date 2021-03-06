---
categories: ["white paper", "critique", "state of the art"]
tags: ["wysiwyg","web-page composer"] 
title: "Critique of contemporary WYSIWYG web-page composers"
linkTitle: "Critique of contemporary WYSIWYG web-page composers"
tags: ["WYSIWYG", "web page composer", "word processing", "drawing program"]
weight: 2
description: >
  Weaknesses of current WYSIWYG web-page composers.
type: docs
---

WYSIWYG stands for “What You See Is What You Get.” All the well-known WYSIWYG web page composers, whether standalone or embedded, treat web-page composition like word processing—or like drawing—rather than like an organizational (structured, semantic, dynamic-design) problem. They work mainly on the superficial look of web pages. Typically they are designed merely to provide a gentle approach to HTML editing.

Pages produced by such WYSIWYG page composers seldom help with the powerful possibilities of web applications.  Well-crafted web pages can adjust themselves according to the type of media they appear on (e.g., phone, desktop, or paper). They can be dynamic, using AJAX, which allows them to update parts of themselves quickly without reloading the whole page. They have reactive widgets. They have structures based upon semantic meaning.

Contemporary WYSIWYG page composers often sport a button to switch to an HTML-source view, as if copping-out when their visual paradigms fail. Their interfaces are reminiscent of IDEs (integrated development environments) or RAD (rapid application development) tools provided by large, complicated, programmer-oriented frameworks. Indeed, IDEs sometimes include WYSIWYG web page composers.

These page composers produce "dirty" HTML containing excess, unruly pieces of HTML, as explained by Nick Santos.{{< fnref 21 >}} The HTML they generate gets dirtier and dirtier as the user makes more and more changes to the web page.

The thorny problem that web-page-embedded, JavaScript-based editors attempt to solve is that web browsers do not sufficiently support their tasks. The critical browser feature supporting web page editing is called `contentEditable`. Piotrek Koszuliński, the lead developer of *CKEditor*, wrote a detailed technical explanation of why `contentEditable` is flawed yet indispensable.{{< fnref 22 >}} Some of his points are:

1. It is difficult to force every browser to use `strong` instead of `b` for the *bold* command.
1. It is hard to coerce the Enter key to create new paragraphs instead of `b`  or `div`.
1. Cleaning up pasted code is messy and imperfect.
1. From mid-2007, for at least the next eight years, the selection systems of the Blink and WebKit web browser engines remained broken.
1. APIs and their implementations related to `contentEditable` "are incomplete and/or inconsistent and buggy."
1. [Composition events](https://developer.mozilla.org/en-US/docs/Web/API/CompositionEvent) are very complicated to handle without `contentEditable` breaking many things: editing in an iPad, the keystrokes for jumping over words, shake-to-undo on the iPhone, spell checking, and screen readers. (Text entry of an accented letter, a complex Japanese character, and a letter with a diacritic all invoke composition events. Googling "Mozilla composition event" and "Wikipedia input method" provides all a non-technical or technical person needs to know to get a quick start with composition events.)
1. Standardizing browser APIs to address all the above issues is a tough job.

The author does not know whether Blink and WebKit ever fixed those bugs. Still, Fatos Bediu{{< fnref 23 >}} and Mark Lancaster{{< fnref 24 >}} have recently written about how difficult it is to use `contentEditable`.

Nick Santos explains how HTML is not well behaved in WYSIWYG editors. For example, he says, all the forms:

    <strong><em>Baggins</em></strong>
    <em><strong>Baggins</strong></em>
    <em><strong>Bagg</strong><strong>ins</strong></em>
    <em><strong>Bagg</strong></em><strong><em>ins</em></strong>

should be treated the same by the WYSIWYG editor. A WYSIWYG editor should treat an edit to any of these forms the same, but, as he says, "For many `ContentEditable` implementations on the web, some invisible character or empty span tag may slip into the HTML, so that two `ContentEditable` elements behave totally differently (even though they look the same)."

According to Dan Dascalescu,{{< fnref 25 >}} in a survey of about 60 in-browser WYSIWYG editors, only one editor could paste images directly from the clipboard. More recently, Jeferson Mari and others{{< fnref 26 >}} curated another list of WYSIWYG editors.

Here are screenshots of a few of the many composers in this class (chosen a few years ago by the author), leaving aside the composers tied to heavyweight integrated development environments:

{{< figure src="/images/bluegriffon1_6_french.jpeg" title="BlueGriffon" target="_blank" >}}
{{< figure src="/images/ckeditor.jpeg" title="CKeditor" target="_blank" >}}
{{< figure src="/images/kompozer.png" title="KompoZer" target="_blank" >}}
{{< figure src="/images/maqetta.png" title="Maqetta" target="_blank" >}}
{{< figure src="/images/tinymce.jpeg" title="TinyMCE" target="_blank" >}}

## Aside
Maqetta, although its development is inactive, provides an exciting and unique approach to WYSIWYG web-page composition, in that it
1. supports composition with OpenAjax widgets,
1. "allows User Experience Designers (UXD) to perform drag/drop assembly of live UI mockups,"
1. includes "deep support for CSS styling (the application includes a full CSS parser/modeler),"
1. includes "a mechanism for organizing a UI prototype into a series of 'application states' (aka 'screens' or 'panels') which allows a UI designer to define interactivity without programming," and
1. has a code base with "a toolkit-independent architecture that allows for plugging in arbitrary widget libraries and CSS themes."
