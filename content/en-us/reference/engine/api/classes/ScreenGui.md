---
title: ScreenGui
type: class
superclass: LayerCollector
---

# ScreenGui

Primary container of on-screen 2D user interface elements.

**Inherits from:** `Class.LayerCollector` > `Class.GuiBase2d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Description

`Class.ScreenGui` is a storage container for 2D `Class.GuiObject|GuiObjects`
displayed on the user's screen. A `Class.ScreenGui` only shows if parented to
a player's `Class.PlayerGui`; parenting a `Class.ScreenGui` to
`Class.StarterGui` ensures it clones into each player's `Class.PlayerGui` when
they join the experience and their character first spawns. See
[On‑Screen UI Containers](../../../ui/on-screen-containers.md) for further
details.

<img src="../../../assets/ui/ui-objects/ScreenGui-Example.jpg" width="840" alt="Example ScreenGui with various GuiObject children, including a Frame, TextLabel, TextBox, and ImageButton." />

For performance improvements, the appearance of a `Class.ScreenGui` is cached
until one of the following events occurs:

- A descendant is added to or removed from it.
- A property of a descendant changes.
- A property of the `Class.ScreenGui` itself changes.

If any of these events occur, the `Class.ScreenGui` appearance is recomputed
on the next frame it gets rendered.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ScreenGui.ClipToDeviceSafeArea` | `bool` |  |
| `Class.ScreenGui.DisplayOrder` | `int` |  |
| `Class.ScreenGui.IgnoreGuiInset` | `bool` | [NotReplicated] |
| `Class.ScreenGui.OnTopOfCoreBlur` | `bool` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.ScreenGui.SafeAreaCompatibility` | `Enum.SafeAreaCompatibility` |  |
| `Class.ScreenGui.ScreenInsets` | `Enum.ScreenInsets` |  |
