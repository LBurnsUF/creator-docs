---
title: StyleLink
type: class
superclass: Instance
---

# StyleLink

Links a `Class.StyleSheet` to the instance tree whose root is the parent of
the `StyleLink`.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

Links a `Class.StyleSheet` to the instance tree whose root is the parent of
the `StyleLink`. For example, placing a `StyleLink` under a `Class.ScreenGui`
applies the referenced `Class.StyleSheet` to both the `Class.ScreenGui` and
all of the `Class.GuiObject|GuiObjects` within it. Only one `Class.StyleSheet`
can apply to a given tree.

<img src="/assets/studio/explorer/StyleLink-Propagation.png" width="320" />

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.StyleLink.StyleSheet` | `Class.StyleSheet` |  |
