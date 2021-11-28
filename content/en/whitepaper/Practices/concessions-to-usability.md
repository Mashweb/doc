---
title: "Concessions to usability"
linkTitle: "Concessions to usability"
weight: 3
date: 2017-01-05
description: >
  Some dilemmas Zen will face in its manipulation of the DOM. How it will ameliorate them.
type: docs
---

Some concessions to manipulability are necessary so that Zen can successfully edit all webpages. When HTML elements are grabbed Zen should temporarily apply suitable styles to HTML elements like high-contrast borders to make them visible during element selection. When the display-style property of an HTML element is none, Zen should make it possible for users to temporarily set it to another value so the element can be seen. Likewise, wherever desired, Zen should employ similar tactics to make all elements visible and manipulable, whether they are too small; too big; too transparent; or animated. Zen should employ intuitive, adaptive, custom cursors with contrast and distinctive patterns that show up with whatever colors are behind them. The animations in Figures 14 and 15 are actual screen recordings of rough-prototype GUIs for rearranging NodeLists that contain just blocks or just inlines, respectively.

{{< figure src="/images/block-demo.gif" title="Figure 14. Block-manipulator prototype. Click to open the live demo in a new window." target="_blank" >}}

{{< figure src="/images/inline-demo.gif" title="Figure 15. Inline-manipulator prototype. Click to open the live demo in a new window." target="_blank" >}}
