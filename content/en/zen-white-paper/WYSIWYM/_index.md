
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

WYMeditor is the best-known WYSIWYM web page composer. *WYSIWYM* stands for *What You See Is What You Mean*. In a WYSIWYM editor the user creates a document with a *structure*. The *presentation* of the document is out of his hands. Separating content and structure from presentation makes it possible to view the document in many ways on many devices, which is a main principle of good web design.
{{< figure src="/images/WYMeditor.png" title="WYMeditor" target="_blank" >}}

Good as the WYSIWYM principle is for web design, WYMeditor has serious drawbacks. It is tricky to set up. A web page cannot embed it. According to the Wikipedia article on WYMeditor,{{< fnref 27 >}} "One downside of WYMeditor is that it cannot be used to include JavaScript in the content it edits. Changing this would require eliminating WYMeditor's use of the innerHtml property." Thus, WYMeditor won't work with reactive widgets.

*This section might be expanded later to elaborate on WYSIWYM and to cover a representative set of WYSIWYM composers.*
