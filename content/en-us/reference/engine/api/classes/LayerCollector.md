---
title: LayerCollector
type: class
superclass: GuiBase2d
tags: [NotCreatable, NotBrowsable]
---

# LayerCollector

The base class of 2D UI containers which render `Class.GuiObject|GuiObjects`
in layers.

**Inherits from:** `Class.GuiBase2d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotBrowsable]

## Description

**LayerCollector** is the base class of 2D UI containers which render
`Class.GuiObject` descendants, such as `Class.ScreenGui`.

For performance improvements, the appearance of a `Class.LayerCollector` is
cached until one of the following events occurs:

- A descendant is added to or removed from it.
- A property of a descendant changes.
- A property of the `Class.LayerCollector` itself changes.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.LayerCollector.Enabled` | `bool` |  |
| `Class.LayerCollector.ResetOnSpawn` | `bool` |  |
| `Class.LayerCollector.TabKeyboardNavigation` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.LayerCollector.ZIndexBehavior` | `Enum.ZIndexBehavior` |  |

## Methods

### `Class.LayerCollector:GetGuiObjectsAtPosition`

``GetGuiObjectsAtPosition(x: `int`, y: `int`)`` -> `Datatype.Instances`
   {security: RobloxScriptSecurity}

### `Class.LayerCollector:GetLayoutNodeTree`

``GetLayoutNodeTree()`` -> `Dictionary`
  [Deprecated]
