---
title: "Introduction"
linkTitle: "Introduction"
weight: 1
description: >
  Zen: A New Approach to Authoring the Web
type: docs
---

{{% pageinfo %}}
Web-Page Editing and Web App Development
Based upon Elementary Sequential Programming,
Visual Programming, and
Direct Manipulation of the DOM,<br/>
Version 0.12.0<br/>
<br/>
by Tom Elam<br/>
Mysuru, India<br/>
November 28, 2021
{{% /pageinfo %}}

This white paper presents a profoundly unique, personalized, and adaptive approach to the creation of web experiences—a radically new approach usable by a very broad class of people. It links to live prototypes of web-page-editor interfaces to demonstrate that it could be possible for end users to build their own web pages from scratch and decide every detail of their web pages' look and structure simply, easily, and quickly, without any prior learning. The possibilities go far beyond just editing web pages, which this paper also intends to show. The code name for this approach and its implementation (under development) is Zen. The unique selling point (USP) of Zen will be in-context, instant-feedback, _full-featured_ editing of website or web app structure, function, and styling. In particular, Zen will make it easy for users to create any kind of valid HTML structure in web pages without getting into the complexity or distraction of code and will make it easy for them to create basic-level programs using visual-programming principles adopted from successful visual-programming languages for children. Most importantly, all this "development" and its _deployment_ can be continuous, carried on by a _website's users_ of all levels of experience. Since, with Zen, deploying and sharing a new application could be as simple as clicking a _Share_ or _Deploy_ button, self-organizing user communities might develop altogether novel applications.

A deliverable of the Zen project will be an example Zen-based web application framework{{<fnref "1">}}
comprising the Zen client-side JavaScript library, aka <em>Core Zen</em>, and a liberally licensed server-side framework (possibly Ruby on Rails) augmented with code to store and serve the web pages created and modified by Zen.  Even though Core Zen will only have to be loaded once to create an unlimited number of web pages with unique URLs, a strong effort will be made to keep the "time-to-interact" (TTI) delay introduced by Core Zen down to 2&ndash;3 seconds, so that Zen's potential application can be as broad as possible.  (TTI is the time it takes from the start of a web page load until the time when the user is comfortable interacting with the web page.) Potentially many other implementations of Zen could be developed to incorporate and integrate Core Zen into web content management systems, wikis, website builders, web frameworks, web portals, web development tools for editing, testing, and debugging code, and integrated development environments (IDEs) for web development.  Web services such as Google's Accelerated Mobile Pages (AMP){{<fnref "2">}}
and Google Hosted Libraries{{<fnref "3">}}
could broaden Zen's potential.

Many user-programmed systems for customizing websites are described in the book *No Code Required: Giving Users Tools to Transform the Web*{{<fnref "4">}}
but no system for _creating_ web apps.  With Zen, many kinds of web apps will be created as simply as are the applications written by children in specially designed visual programming languages. (Specific references to these child-oriented systems are provided later in this paper.)

Though many of the problems of creating end-user programming environments have been overcome to some degree or other, there is one obstacle to it that still has no embeddable (library-based) solution&mdash;as opposed to a framework-based solution.  That is a problem that arises from the stateless nature of the Web.  To illustrate, we take an example of a typical program that asks a user's name and greets him accordingly:

<pre>
<code>
    PRINT "What is your name?"
    INPUT "(Enter your name.)", $name
    PRINT
    PRINT "Hello, "; $name; ", how are you today?"
</code>
</pre>

The flow of this program is obvious, but even such a simple program must be written on a platform that hides complexity: it must be halted, waiting for a response.  This is true no matter what the programming platform is.  For desktop applications, the operating system provides system calls, a scheduler, and library functions that allow program flow to mirror the thread or process of the program, as in the example. For web apps there is no underlying operating system to support the halting and restarting of the program. However, the Scheme programming language supports _first-class continuations_,{{< fnref 5 >}}<sup>, </sup>{{< fnref 6 >}}<sup>, </sup>{{< fnref 7 >}}<sup>, </sup>{{< fnref 8 >}} which allow programs to be halted and restarted using <em>language-level</em> mechanisms (as opposed to operating-styem system calls and library functions). Zen will utilize continuations to simplify the end-user's programming tasks.

Why Zen's new approach is desirable and how it is anticipated to work are the subjects of this whole paper, but a brief video from the Digital Archaeology project{{< fnref 9 >}} showing the operation of the first web browser can provide some background context. The video shows the operation of the first web browser, called Nexus, crafted by the inventor of the World Wide Web himself, Sir Tim Berners-Lee. Twelve minutes and nine seconds into the video, Nexus's editing function is demonstrated (Figure 1). Thus, from the very beginning, Berners-Lee intended the web browser to enable easy collaborative authoring.
However, as he himself says, "It didn't really take off that
way."
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
1. standalone WYSIWYG web-page editors that operate on web-page source and show a preview of the resultant web page. Source can be HTML or markup to be translated into HTML.
1. WYSIWYM semantic web-page editors. Examples of this type of editor are WYMEditor, RDFaCE, BlueprintUI, PageDown, and Showdown. (The author needs to further investigate these editors.) Source can be HTML or markup that can be translated into HTML.

Apart from editors that only edit web pages, there are other tools and applications for developing web experiences:
1. online web development tools for testing and debugging code (e.g. JSFiddle.net, CodePen.io, jsbin.com, etc.),
1. web-developer's tools and "augmented-browsing software"{{< fnref 17 >}}<sup>, </sup>{{< fnref 18 >}}<sup>, </sup>{{< fnref 19 >}}<sup>, </sup>{{< fnref 20 >}} (e.g. Firebug for Firefox, Developer Tools for Chrome, Developer Tools for Safari, Greasemonkey, Tampermonkey, Chickenfoot, X-Ray Goggles),
1. integrated development environments (IDEs) that build websites,
1. web content management systems (web CMSs or simply WCMSs),
1. website builders,
1. web frameworks, and
1. web portals.
