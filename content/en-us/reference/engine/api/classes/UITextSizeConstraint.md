---
title: UITextSizeConstraint
type: class
superclass: UIConstraint
---

# UITextSizeConstraint

Ensures that the size of text rendered by certain `Class.GuiObject` classes
lies within the range described by
`Class.UITextSizeConstraint.MaxTextSize|MaxTextSize` and
`Class.UITextSizeConstraint.MinTextSize|MinTextSize`.

**Inherits from:** `Class.UIConstraint` > `Class.UIComponent` > `Class.UIBase` > `Class.Instance` > `Class.Object`

## Description

A **UITextSizeConstraint** ensures that the size of text rendered by certain
`Class.GuiObject` classes (`Class.TextLabel`, `Class.TextButton`, or
`Class.TextBox`) lies within the range described by
`Class.UITextSizeConstraint.MaxTextSize|MaxTextSize` and
`Class.UITextSizeConstraint.MinTextSize|MinTextSize`. It is meant to be used
alongside `Class.TextLabel.TextScaled`, which automatically scales text to
fill its containing object. Like other UI constraints, it is applied when
parented to the object to be constrained.

It's recommended that no values lower than 9 be used for
`Class.UITextSizeConstraint.MinTextSize|MinTextSize` property, otherwise text
may not be readable to most users.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.UITextSizeConstraint.MaxTextSize` | `int` |  |
| `Class.UITextSizeConstraint.MinTextSize` | `int` |  |
