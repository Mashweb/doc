---
categories: ["white paper", "survey"]
tags: ["user programming", "low code", "no code", "web applications", "web develoment", "Zen", "free software", "continuations", "Nexus browser", "Berners-Lee", "contentEditable", "rich-text editor", "WYSIWYG", "WYSIWYM", "augmented browsing", "IDE", "CMS", "website builder", "web framework", "web portal"]
title: "Introduction"
linkTitle: "Introduction"
weight: 1
description: >
  Zen: User-Programmed Web Applications
type: docs
---

This white paper presents a profoundly unique, personalized, and adaptable system called Zen, under development, for creating web applications--a radically new system usable by a very inclusive class of people. It links to [live, interactive experiments](https://web-call.cc) showing the incremental progress in building Zen. Each investigation tests at least one new function to make web-page editing easy and natural and enable non-programmers to create simple web applications. Someday, Zen might allow end-users to build highly interactive web applications from scratch and decide virtually every detail of their look, structure, and function simply, efficiently, and quickly without prior learning.

{{< figure src="/images/programming.jpg" title="Old School">}}

Zen's unique selling point (USP) will be in-context, instant feedback, *full-featured* editing of website or web application structure, function, and styling. Zen will make it easy for users to create valid HTML and styles in web pages without getting into the complexity or distraction of code. Zen users will quickly develop basic web application programs using visual-programming principles adopted from successful visual-programming languages for children. Most importantly, all this "development" and its *deployment* can be continuous, carried on by a *website's users* of all levels of experience. Deploying and sharing a new application could be as simple as clicking a *Share* button. Self-organizing Zen user communities might even develop novel applications.

The unusual part of Zen will be [free software](https://www.gnu.org/philosophy/pragmatic.html) that programmers can use to give their websites Zen's unique capabilities. Zen's core ("Core Zen"){{< fnref 1 >}} will work with virtually any website's server technology. Model website server technology{{< fnref "2" >}}will develop alongside Core Zen. It will be made available on the internet,{{< fnref "3" >}} providing user registration and private accounts for users who want to save their work.

The book *No Code Required*{{< fnref "4" >}}describes many user-programmed systems for customizing websites but none for creating web apps.  Zen will enable the easy creation of many kinds of web apps. Children write application programs in specially designed visual programming languages, so why not adults?

Many problems of end-user programming environments for the web have been overcome to some degree or other by the thousands or millions of web developers in the world. However, the biggest of these problems arises from the stateless nature of the web.  To illustrate, let us first review how simple and straightforward it is for a typical desktop program to ask a user's name and greet him accordingly:

<pre>
<code>
    PRINT "What is your name?"
    INPUT "(Enter your name.)", $name
    PRINT
    PRINT "Hello, "; $name; ", how are you today?"
</code>
</pre>

The flow of this program is apparent but can only work on a platform that hides complexity. It must be halted, waiting for a response.  For desktop applications, the operating system provides system calls, a scheduler, and library functions that allow the look of such a program to mirror its progress. There is no underlying operating system for web applications to support the halting and restarting of the program. However, the Scheme programming language supports *first-class continuations*.{{< fnref 5 >}}<sup>, </sup>{{< fnref 6 >}}<sup>, </sup>{{< fnref 7 >}}<sup>, </sup>{{< fnref 8 >}} These continuations allow programs to be halted and restarted using <em>language-level</em> mechanisms (as opposed to operating-system system calls and library functions). Zen will utilize continuations to simplify both the Zen developer's job and the user's programming tasks.

This paper will explain the appeal of Zen's new approach and the plan to make work it work. A brief video from the Digital Archaeology project{{< fnref 9 >}} showing the operation of the first web browser can provide some background context. The video shows the function of the first web browser, called Nexus, crafted by the inventor of the World Wide Web himself, Sir Tim Berners-Lee. Nexus's editing function is demonstrated twelve minutes and nine seconds into the video (Figure 1). Thus, Berners-Lee intended the web browser to enable easy collaborative authoring from the very beginning. However, as he says, "It didn't really take off that way."
{{< fnref 10 >}}<sup>, </sup>
{{< fnref 11 >}}<sup>, </sup>
{{< fnref 12 >}}

{{< figure src="http://img.youtube.com/vi/3c3Rt6QbHDw/0.jpg" title="Figure 1. Demonstration of the editing function of the first web browser. Click to open." link="http://www.youtube.com/watch?feature=player_embedded&v=3c3Rt6QbHDw#t=12m9s" target="_blank" >}}

Now, a quarter of a century later, the position of the A-grade web browsers{{< fnref 13 >}}<sup>, </sup>
{{< fnref 14 >}}<sup>, </sup>
{{< fnref 15 >}}<sup>, </sup>
{{< fnref 16 >}}
as the central applications for online sharing seems unshakeable. Yet till today, not one A-grade web browser has full-fledged web-authoring capabilities. (We shall discuss the browser features _contentEditable_ and _designMode_ later, since these do not, without external programming, constitute web-authoring capabilities.) The direct descendents of Berners-Lee's early web-page editing application are visual web-page editors in three broad categories:
1. in-browser rich-text editors. These are web-page-embedded, JavaScript-based, WYSIWYG web-page editors that convert HTML textarea fields or other HTML elements into editor instances. TinyMCE and CKeditor are typical examples.
1. standalone WYSIWYG web-page editors that operate on web-page sources and show a preview of the resultant web page. Sources can be HTML or markup to be translated into HTML.
1. WYSIWYM semantic web-page editors. Examples of this type of editor are WYMEditor, RDFaCE, BlueprintUI, PageDown, and Showdown. (The author needs to further investigate these editors.) Source can be HTML or markup that can be translated into HTML.

Apart from editors that only edit web pages, there are other tools and applications for developing web experiences:
1. online web development tools for testing and debugging code (e.g. JSFiddle.net, CodePen.io, jsbin.com, etc.),
1. web-developer tools and "augmented-browsing software"{{< fnref 17 >}}<sup>, </sup>{{< fnref 18 >}}<sup>, </sup>{{< fnref 19 >}}<sup>, </sup>{{< fnref 20 >}} (e.g. Firebug for Firefox, Developer Tools for Chrome, Developer Tools for Safari, Greasemonkey, Tampermonkey, Chickenfoot, X-Ray Goggles),
1. integrated development environments (IDEs) that build websites,
1. web content management systems (web CMSs or simply WCMSs),
1. website builders,
1. web frameworks, and
1. web portals.
