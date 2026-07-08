---
title: ImageButton
type: class
superclass: GuiButton
---

# ImageButton

A 2D user interface element that displays an interactive image.

**Inherits from:** `Class.GuiButton` > `Class.GuiObject` > `Class.GuiBase2d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Description

An `Class.ImageButton` behaves similarly to an `Class.ImageLabel` in regards
to rendering, with the additional behaviors of a `Class.GuiButton`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ImageButton.ContentImageSize` | `Datatype.Vector2` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.ImageButton.HoverImage` | `Datatype.ContentId` |  |
| `Class.ImageButton.HoverImageContent` | `Datatype.Content` |  |
| `Class.ImageButton.Image` | `Datatype.ContentId` |  |
| `Class.ImageButton.ImageColor3` | `Datatype.Color3` |  |
| `Class.ImageButton.ImageContent` | `Datatype.Content` |  |
| `Class.ImageButton.ImageRectOffset` | `Datatype.Vector2` |  |
| `Class.ImageButton.ImageRectSize` | `Datatype.Vector2` |  |
| `Class.ImageButton.ImageTransparency` | `float` |  |
| `Class.ImageButton.IsLoaded` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.ImageButton.PressedImage` | `Datatype.ContentId` |  |
| `Class.ImageButton.PressedImageContent` | `Datatype.Content` |  |
| `Class.ImageButton.ResampleMode` | `Enum.ResamplerMode` |  |
| `Class.ImageButton.ScaleType` | `Enum.ScaleType` |  |
| `Class.ImageButton.SliceCenter` | `Datatype.Rect` |  |
| `Class.ImageButton.SliceScale` | `float` |  |
| `Class.ImageButton.TileSize` | `Datatype.UDim2` |  |

## Methods

### `Class.ImageButton:SetEnableContentImageSizeChangedEvents`

``SetEnableContentImageSizeChangedEvents(enabled: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}
