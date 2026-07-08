---
title: Frame
type: class
superclass: GuiObject
---

# Frame

A `Class.GuiObject` that renders as a plain rectangle, generally used as a
container.

**Inherits from:** `Class.GuiObject` > `Class.GuiBase2d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Description

`Class.Frame` is a `Class.GuiObject` that acts as a container for other
`Class.GuiObject|GuiObjects`. You can use it for UI that either displays on a
user's [screen](../../../ui/on-screen-containers.md) or on a
[surface](../../../ui/in-experience-containers.md) within the experience.

<img src="/assets/ui/ui-objects/Frame-Example.jpg" width="840" />

`Class.Frame|Frames` are ideal containers for responsive layouts such as
[list and flex layouts](../../../ui/list-flex-layouts.md), allowing you to
change the size of the frame and dynamically adjust how layout items fit
within it. `Class.Frame|Frames` are also core `Class.GuiObject|GuiObjects`, so
you can customize properties such as
`Class.GuiObject.BackgroundColor3|BackgroundColor3`,
`Class.GuiObject.Transparency|Transparency`, apply a
[background gradient](../../../ui/appearance-modifiers.md#gradient) or
[border](../../../ui/appearance-modifiers.md#stroke), and more.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Frame.Style` | `Enum.FrameStyle` |  |
