---
title: GuiBase2d
type: class
superclass: GuiBase
tags: [NotCreatable, NotBrowsable]
---

# GuiBase2d

An abstract class inherited by 2D `Class.GuiObject|GuiObjects`.

**Inherits from:** `Class.GuiBase` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotBrowsable]

## Description

`Class.GuiBase2d` is an abstract class inherited by 2D
`Class.GuiObject|GuiObjects`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.GuiBase2d.AbsolutePosition` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] |
| `Class.GuiBase2d.AbsoluteRotation` | `float` | [ReadOnly] [NotReplicated] |
| `Class.GuiBase2d.AbsoluteSize` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] |
| `Class.GuiBase2d.AutoLocalize` | `bool` |  |
| `Class.GuiBase2d.ClippedRect` | `Datatype.Rect` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.GuiBase2d.IsNotOccluded` | `bool` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.GuiBase2d.Localize` | `bool` | [Hidden] [NotReplicated] [Deprecated] |
| `Class.GuiBase2d.RawRect2D` | `Datatype.Rect` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.GuiBase2d.RootLocalizationTable` | `Class.LocalizationTable` |  |
| `Class.GuiBase2d.SelectionBehaviorDown` | `Enum.SelectionBehavior` |  |
| `Class.GuiBase2d.SelectionBehaviorLeft` | `Enum.SelectionBehavior` |  |
| `Class.GuiBase2d.SelectionBehaviorRight` | `Enum.SelectionBehavior` |  |
| `Class.GuiBase2d.SelectionBehaviorUp` | `Enum.SelectionBehavior` |  |
| `Class.GuiBase2d.SelectionGroup` | `bool` |  |
| `Class.GuiBase2d.TotalGroupScale` | `float` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |

## Events

### `Class.GuiBase2d.SelectionChanged`

Fires with: (amISelected: `bool`, previousSelection: `Class.GuiObject`, newSelection: `Class.GuiObject`)
