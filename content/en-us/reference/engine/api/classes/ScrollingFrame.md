---
title: ScrollingFrame
type: class
superclass: GuiObject
---

# ScrollingFrame

`ScrollingFrame` is a special `Class.Frame` type with built-in scrolling
interactivity and different ways to customize how the scrolling works.

**Inherits from:** `Class.GuiObject` > `Class.GuiBase2d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Description

`ScrollingFrame` is a special `Class.Frame` type with built-in scrolling
interactivity and different ways to customize how the scrolling works.

<img src="/assets/ui/ui-objects/ScrollingFrame-Example.jpg" width="840" alt="Example ScrollingFrame on the screen containing a tabbed category bar and a list of magical items for the player to consider purchasing." />

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ScrollingFrame.AbsoluteCanvasSize` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] |
| `Class.ScrollingFrame.AbsoluteWindowSize` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] |
| `Class.ScrollingFrame.AutomaticCanvasSize` | `Enum.AutomaticSize` |  |
| `Class.ScrollingFrame.BottomImage` | `Datatype.ContentId` |  |
| `Class.ScrollingFrame.BottomImageContent` | `Datatype.Content` |  |
| `Class.ScrollingFrame.CanvasPosition` | `Datatype.Vector2` |  |
| `Class.ScrollingFrame.CanvasSize` | `Datatype.UDim2` |  |
| `Class.ScrollingFrame.DraggingScrollBar` | `Enum.DraggingScrollBar` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.ScrollingFrame.ElasticBehavior` | `Enum.ElasticBehavior` |  |
| `Class.ScrollingFrame.HorizontalBarRect` | `Datatype.Rect` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.ScrollingFrame.HorizontalScrollBarInset` | `Enum.ScrollBarInset` |  |
| `Class.ScrollingFrame.MaxCanvasPosition` | `Datatype.Vector2` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.ScrollingFrame.MidImage` | `Datatype.ContentId` |  |
| `Class.ScrollingFrame.MidImageContent` | `Datatype.Content` |  |
| `Class.ScrollingFrame.ScrollBarImageColor3` | `Datatype.Color3` |  |
| `Class.ScrollingFrame.ScrollBarImageTransparency` | `float` |  |
| `Class.ScrollingFrame.ScrollBarThickness` | `int` |  |
| `Class.ScrollingFrame.ScrollRate` | `float` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.ScrollingFrame.ScrollVelocity` | `Datatype.Vector2` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.ScrollingFrame.ScrollingDirection` | `Enum.ScrollingDirection` |  |
| `Class.ScrollingFrame.ScrollingEnabled` | `bool` |  |
| `Class.ScrollingFrame.SmoothScroll` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.ScrollingFrame.TopImage` | `Datatype.ContentId` |  |
| `Class.ScrollingFrame.TopImageContent` | `Datatype.Content` |  |
| `Class.ScrollingFrame.VerticalBarRect` | `Datatype.Rect` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.ScrollingFrame.VerticalScrollBarInset` | `Enum.ScrollBarInset` |  |
| `Class.ScrollingFrame.VerticalScrollBarPosition` | `Enum.VerticalScrollBarPosition` |  |

## Methods

### `Class.ScrollingFrame:ClearInertialScrolling`

``ClearInertialScrolling()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.ScrollingFrame:GetSampledInertialVelocity`

``GetSampledInertialVelocity()`` -> `Datatype.Vector2`
   {security: RobloxScriptSecurity}

### `Class.ScrollingFrame:GetScrollVelocity`

``GetScrollVelocity()`` -> `Datatype.Vector2`

### `Class.ScrollingFrame:ResetScrollVelocity`

``ResetScrollVelocity()`` -> `null`

### `Class.ScrollingFrame:ScrollToTop`

``ScrollToTop()`` -> `null`
   {security: RobloxScriptSecurity}
