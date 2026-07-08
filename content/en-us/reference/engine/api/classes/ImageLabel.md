---
title: ImageLabel
type: class
superclass: GuiLabel
---

# ImageLabel

A 2D user interface element that displays a single non-interactive image.

**Inherits from:** `Class.GuiLabel` > `Class.GuiObject` > `Class.GuiBase2d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Description

An `Class.ImageLabel` renders a rectangle, like a `Class.Frame` does, with an
image asset. The display of the image can be manipulated through the
`Class.ImageLabel.ImageColor3|ImageColor3` and
`Class.ImageLabel.ImageTransparency|ImageTransparency` properties. To display
only the image and hide the rectangle, set
`Class.GuiObject.BackgroundTransparency` to `1`.

Advanced `Class.ImageLabel` usage includes:

- Tiled images can be created by setting
  `Class.ImageLabel.ScaleType|ScaleType` to `Enum.ScaleType.Tile`, then
  `Class.ImageLabel.TileSize|TileSize` to the size of rendered tiles.

- 9-slice images can be created by setting
  `Class.ImageLabel.ScaleType|ScaleType` to `Enum.ScaleType.Slice`, then
  `Class.ImageLabel.SliceCenter|SliceCenter` to the center area of the 9‑slice
  image.

- Sprite sheets can be implemented through the use of
  `Class.ImageLabel.ImageRectOffset|ImageRectOffset` and
  `Class.ImageLabel.ImageRectSize|ImageRectSize`. Packing multiple images into
  one and using this property can make your experience's image assets load
  much quicker, especially if you use many small icons in your GUIs.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ImageLabel.ContentImageSize` | `Datatype.Vector2` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.ImageLabel.Image` | `Datatype.ContentId` |  |
| `Class.ImageLabel.ImageColor3` | `Datatype.Color3` |  |
| `Class.ImageLabel.ImageContent` | `Datatype.Content` |  |
| `Class.ImageLabel.ImageRectOffset` | `Datatype.Vector2` |  |
| `Class.ImageLabel.ImageRectSize` | `Datatype.Vector2` |  |
| `Class.ImageLabel.ImageTransparency` | `float` |  |
| `Class.ImageLabel.IsLoaded` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.ImageLabel.ResampleMode` | `Enum.ResamplerMode` |  |
| `Class.ImageLabel.ScaleType` | `Enum.ScaleType` |  |
| `Class.ImageLabel.SliceCenter` | `Datatype.Rect` |  |
| `Class.ImageLabel.SliceScale` | `float` |  |
| `Class.ImageLabel.TileSize` | `Datatype.UDim2` |  |

## Methods

### `Class.ImageLabel:SetEnableContentImageSizeChangedEvents`

``SetEnableContentImageSizeChangedEvents(enabled: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}
