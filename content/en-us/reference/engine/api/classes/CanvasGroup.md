---
title: CanvasGroup
type: class
superclass: GuiObject
---

# CanvasGroup

Blends descendants as a group with color/transparency.

**Inherits from:** `Class.GuiObject` > `Class.GuiBase2d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Description

`CanvasGroup` renders descendants as a group with color and transparency
applied to the render result. `Class.UIComponent` visual modifiers such as
`Class.UICorner` and `Class.UIGradient` under a `CanvasGroup` will also apply
to the whole group. Note that `CanvasGroup` always has
`Class.GuiObject.ClipsDescendants|ClipsDescendants` set to `true` and all
descendants will render within group's viewport.

#### Important Notes

- Descendants of `CanvasGroup` will be rendered as a flattened texture only
  when the ancestor `Class.LayerCollector` has its
  `Class.LayerCollector.ZIndexBehavior|ZIndexBehavior` set to
  `Enum.ZIndexBehavior.Sibling`.
- `CanvasGroup` consumes extra texture memory. The quality of the texture and
  total memory usage is limited by the `Enum.QualityLevel` of the client. When
  exceeding the memory cap, `CanvasGroup` will render as a blank texture.
- It's recommended to use `CanvasGroup` with static sizes, otherwise a new
  texture would need to be created to accommodate new sizes.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.CanvasGroup.GroupColor3` | `Datatype.Color3` |  |
| `Class.CanvasGroup.GroupTransparency` | `float` |  |
| `Class.CanvasGroup.ResolutionScale` | `float` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
