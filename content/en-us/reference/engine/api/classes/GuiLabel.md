---
title: GuiLabel
type: class
superclass: GuiObject
tags: [NotCreatable]
---

# GuiLabel

An abstract class for non-interactive 2D user interface elements.

**Inherits from:** `Class.GuiObject` > `Class.GuiBase2d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

GuiLabel is an abstract class that inherits from `Class.GuiObject`. It is the
base class for `Class.ImageLabel` and `Class.TextLabel`. Unlike
`Class.GuiButton`, objects of this type will not register click events, but
instead serve as non-interactive labels. It does not implement any further
properties, events or methods.
