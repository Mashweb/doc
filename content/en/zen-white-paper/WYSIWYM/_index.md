
---
categories: ["white paper", "critique", "state of the art"]
tags: ["wysiwym", "web-page composer", "structured document", "structure", "presentation", "web design"]
title: "Critique of current WYSIWYM web-page composers"
linkTitle: "Critique of current WYSIWYM web-page composers"
weight: 3
date: 2017-01-05
description: >
  Problems with current WYSIWYM web-page composers.
type: docs
---

WYMeditor is the best-known WYSIWYM web page editor. *WYSIWYM* stands for *What You See Is What You Mean*. In a WYSIWYM editor, the user creates a document with *structured, meaningful content*. The *presentation* of the content is out of his hands. The separation of *content* from its *look and feel* makes it possible to view the document in many ways on many devices, which is a central principle of good web design.
{{< figure src="/images/WYMeditor.png" title="WYMeditor" target="_blank" >}}

The WYSIWYM principle undoubtedly is suitable for web design, but WYMeditor has serious drawbacks. It was tricky to set up in the author's own experience. A web page cannot embed it. According to an old Wikipedia article on WYMeditor (now archived on Archive.org),{{< fnref 27 >}} "One downside of WYMeditor is that it cannot be used to include JavaScript in the content it edits. Changing this would require eliminating WYMeditor's use of the `innerHtml` property." Thus, WYMeditor won't work with reactive widgets.

*The author might expand this section to cover a representative set of WYSIWYM composers.*
