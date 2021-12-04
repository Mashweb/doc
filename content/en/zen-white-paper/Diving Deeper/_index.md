---
title: "Diving Deeper: Zen According to The Elements of User Experience"
linkTitle: "Diving Deeper: Zen According to The Elements of User Experience"
weight: 8
description: >
  The stragy framework for the development of Zen.
type: docs
---

Jesse James Garrett, who coined the term AJAX, wrote an influential book entitled The Elements of User Experience{{< fnref 54 >}}, which will serve to inform the strategy for the development of Zen. (The acronym AJAX refers to a set of Web technologies that enable the Web to be used as a remote software interface and employing JavaScript and asynchronous HTTP requests.) Garrett's elements are summarized in a chart{{< fnref 55 >}}. The "Surface Plane" described in that book corresponds roughly to the concerns of the Red End; the "Strategy Plane" to the concerns of the Violet End.

## User Needs for a "Zen Website"

There is a very specific set of user needs that a "Zen website" could uniquely fulfil. At least some of these are:

1. A Web CMS that eschews text-based "code" in favor of a direct manipulation interface (DMI).
1. A Web CMS that excels in the management of intermeshed or intertwined trees and meshes of data of many types: Document Object Models (DOMs, including shadow DOMs), including at least nodes implementing the HTMLElement, Attr, and Text interfaces; CSS classes; and link trees and meshes. See "DOM Standard",{{< fnref 56 >}} published by the WHATWG community.
1. A Web CMS (or WCMS) that can nest web components and widgets with no arbitrary limit.
1. An easy way to consume and perhaps even interrelate Web schema. (See schema.org.{{< fnref 57 >}})

## Site Objectives of a "Zen Website"

If there is a site objective, then there must be a website. If that website has a tight focus, it must be oriented toward a particular segment of its entire potential user population (that is, anyone who comes to the website). My initial attempt to segment users was this:

1. Users who are only fluent in the most basic Web-application constructs: URLs (or URIs), browsers, windows, links, and maybe simple, clear buttons.
1. Users who are fluent in most of the basic, modern user interface patterns used in modern Web applications like those described in the Yahoo Design Pattern Library{{< fnref 58 >}}, such as Top Navigation, Accordion, Breadcrumbs, Tabs, Navigation Bar, Calendar Picker, Collapse Transition, Expand Transition, Slide Transition, and Drag and Drop.
1. Users with enough prior experience and intelligence to quickly adopt new methods of interaction with computers, such as a Windows user who can adapt to an Apple laptop computer, or a user who can learn about dragging and dropping URLs into a web browser or a images from the web browser to the desktop.
1. Users who can productively use a complex, specialized Web application such as a Web-page design application, an application for photo manipulation, a paint application, an application for technical analysis of financial data—an application that typically cannot be learned in less than an hour. Some of the barriers to learning such an application more quickly are jargon, densely packed user interface elements, and domain-specific knowledge.
1. A bit of reflection and research determined that I need to seek out experts' Web user segmentation. That quickly turned up the topic of "web analytics user segmentation", where there is much good information available for free. However, "levels of Web user ability" is a topic I have not explored much at all. It appears there is some very good guidance in the blog entry "Enabling new types of web user experiences". A key insight in that post is that currently the dominant model of how web apps should be experienced is that they should be "web ports" of iPhone apps. The author of the post believes that is aiming far too low in aspiration. He gives some examples of devices like doorknobs and toasters broadcasting web services over Bluetooth or WiFi. Such ideas, while not directly providing much help to Zen development, provide inspiration for the necessary lateral thinking.

Some Zen website use cases could be:

1. Organizing the user's own text collections as hypertext in order to manage relationships between various pieces of information, particularly hypertext documents
1. Creating a "notebook" or "log"
1. Creating a Web app for further personal Web exploration and use
1. Creating a website or Web app for creative or commercial use
1. Create any kind of webiste by doing the front-end design, the front-end programming, and the backend programming
