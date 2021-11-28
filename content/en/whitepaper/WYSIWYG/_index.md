---
categories: []
tags: ["test","docs"] 
title: "Critique of current WYSIWYG web-page composers"
linkTitle: "Critique of current WYSIWYG web-page composers"
weight: 2
description: >
  Problems with current WYSIWYG web-page composers.
type: docs
---

All the well-known WYSIWYG web-page composers, whether standalone or embedded, treat web-page composition like word-processing&mdash;that is, like a layout or 2-D-drawing  problem&mdash;rather than as an organizational (structured, semantic, dynamic-design) problem. Typically visual web-page composers are designed merely to provide a gentle approach to HTML editing, leaving out important aspects like styling based upon semantic meaning; <code>div</code> and <code>span</code> elements; reactive widgets; and dynamic (AJAX-enabled) web pages. They often sport a button to switch to an HTML-source view. Their interfaces are reminiscent of IDEs or RAD tools provided by frameworks used by web-developer frameworks. Indeed, WYSIWYG web-page composers are sometimes included in IDEs. The HTML they produce tends not to be "clean," in the sense that it contains excess pieces of HTML, and not well-behaved, as explained by Nick Santos.{{< fnref 21 >}} The HTML they produce gets dirtier and dirtier as the user makes more and more changes to the web page.

The main problem with web-page-embedded, JavaScript-based editors is that the jobs they are tasked with are extremely difficult and not well supported by web browsers. Piotrek Koszuliński, lead developer of CKEditor, has written a detailed technical explanation{{< fnref 22 >}} of why the key browser feature supporting web-page editing&mdash;<code>contentEditable</code>&mdash;is both flawed and indispensable. Some of his points are:

1. It is difficult to force every browser to use <code>&lt;strong&gt;</code> instead of <code>&lt;b&gt;</code> for the _bold_ command.
1. It is difficult to force the <em>Enter</em> key to create new paragraphs instead of <code>&lt;br&gt;</code> or <code>&lt;div&gt;</code>.
1. Cleaning up pasted code is messy and imperfect.
1. As of August, 2015, the selection systems of the Blink and WebKit web browser engines had been broken for eight years.
1. APIs and their implementations related to <code>contentEditable</code> "are incomplete and/or inconsistent and buggy."
1. Trying to avoid <code>contentEditable</code> uncovers many large difficulties in correctly handling <em>composition events</em> (which allow multiple keystrokes to form an accented letter, a complex Japanese character, or a letter with a diacritic) without breaking editing on an iPad, the keystrokes for jumping over words, shake-to-undo on the iPhone, spell checking, and screen readers.
1. Standardizing browser APIs to address all the above issues is an extremely difficult job.

Nick Santos explains how HTML is not well behaved in WYSIWYG editors. For example, he says, all the forms: <small><pre>&lt;strong&gt;&lt;em&gt;Baggins&lt;/em&gt;&lt;/strong&gt;<br>&lt;em&gt;&lt;strong&gt;Baggins&lt;/strong&gt;&lt;/em&gt;<br>&lt;em&gt;&lt;strong&gt;Bagg&lt;/strong&gt;&lt;strong&gt;ins&lt;/strong&gt;&lt;/em&gt;<br>&lt;em&gt;&lt;strong&gt;Bagg&lt;/strong&gt;&lt;/em&gt;&lt;strong&gt;&lt;em&gt;ins&lt;/em&gt;&lt;/strong&gt;</pre></small> should be treated the same by the WYSIWYG editor. An edit to any of these forms should be treated the same, but, as he says, "For many ContentEditable implementations on the web, some invisible character or empty span tag may slip into the HTML, so that two ContentEditable elements behave totally differently (even though they look the same)."

According to Dan Dascalescu,{{< fnref 22 >}} in a survey of about 60 in-browser, WYSIWYG editors, only one editor could paste images directly from the clipboard.

Here are screenshots of a few of the many composers in this class, leaving aside the composers tied to heavyweight integrated development environments:

{{< figure src="/images/bluegriffon1_6_french.jpeg" title="BlueGriffon" target="_blank" >}}
{{< figure src="/images/ckeditor.jpeg" title="CKeditor" target="_blank" >}}
{{< figure src="/images/kompozer.png" title="KompoZer" target="_blank" >}}
{{< figure src="/images/maqetta.png" title="Maqetta" target="_blank" >}}
{{< figure src="/images/tinymce.jpeg" title="TinyMCE" target="_blank" >}}

##### Aside
<small>Maqetta, although its development is inactive, provides an interesting and unique approach to WYSIWYG web-page composition, in that it
1. supports composition with OpenAjax widgets,
1. "allows User Experience Designers (UXD) to perform drag/drop assembly of live UI mockups,"
1. includes "deep support for CSS styling (the application includes a full CSS parser/modeler),"
1. includes "a mechanism for organizing a UI prototype into a series of 'application states' (aka 'screens' or 'panels') which allows a UI designer to define interactivity without programming," and
1. has a code base with "a toolkit-independent architecture that allows for plugging in arbitrary widget libraries and CSS themes."
</small>
