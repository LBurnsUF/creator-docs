---
title: UDim2
type: datatype
---

# `Datatype.UDim2`

Represents a two-dimensional value where each dimension is composed of a
relative scale and an absolute offset.

## Description

The `Datatype.UDim2` data type represents a two-dimensional value where each
dimension is composed of a relative scale and an absolute offset in pixels. It
is a combination of two `Datatype.UDim` data types representing the **X** and
**Y** dimensions. The most common usages for `Datatype.UDim2` are setting the
`Class.GuiObject.Size|Size` and `Class.GuiObject.Position|Position` of
`Class.GuiObject|GuiObjects`.

```lua
local guiObject = script.Parent
guiObject.Size = UDim2.new(0, 300, 1, 0)  -- 300 pixels wide; full height of parent
guiObject.Position = UDim2.new(0, 50, 0, 0)  -- 50 pixels from the left
```

## Constructors

### `UDim2.new`

Returns a new `Datatype.UDim2` with the coordinates of two zero `Datatype.UDim`
components representing each axis.

### `UDim2.new`

Returns a new `Datatype.UDim2` given the coordinates of the two `Datatype.UDim`
components representing each axis.

**Parameters:**

- `xScale`: `number` - The **X** dimension scale.
- `xOffset`: `number` - The **X** dimension offset.
- `yScale`: `number` - The **Y** dimension scale.
- `yOffset`: `number` - The **Y** dimension offset.

### `UDim2.new`

Returns a new `Datatype.UDim2` from the given `Datatype.UDim` objects representing
the **X** and **Y** dimensions, respectively.

**Parameters:**

- `x`: `UDim`
- `y`: `UDim`

### `UDim2.fromScale`

Returns a new `Datatype.UDim2` with the given scalar coordinates and no offsets.
Equivalent to:

```lua
UDim2.fromScale(xScale, yScale) == UDim2.new(xScale, 0, yScale, 0)
```

**Parameters:**

- `xScale`: `number`
- `yScale`: `number`

### `UDim2.fromOffset`

Returns a new `Datatype.UDim2` with the given offset coordinates and no scaling. Equivalent to:

```lua
UDim2.fromOffset(xOffset, yOffset) == UDim2.new(0, xOffset, 0, yOffset)
```

**Parameters:**

- `xOffset`: `number`
- `yOffset`: `number`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `UDim2.X` | `UDim` | The **X** dimension scale and offset of the `Datatype.UDim2`. |
| `UDim2.Y` | `UDim` | The **Y** dimension scale and offset of the `Datatype.UDim2`. |
| `UDim2.Width` | `UDim` | The **X** dimension scale and offset of the `Datatype.UDim2`. |
| `UDim2.Height` | `UDim` | The **Y** dimension scale and offset of the `Datatype.UDim2`. |

## Methods

### `UDim2:Lerp`

Returns a `Datatype.UDim2` interpolated linearly between this
`Datatype.UDim2` and the given `goal`. The `alpha` value should be a
number between `0` and `1`.

**Parameters:**

- `goal`: `UDim2`
- `alpha`: `number`

## Math Operations

| Operation | Description |
|-----------|-------------|
| `UDim2` + | Produces a `Datatype.UDim2` with components that are the sum of the respective components of the two |
| `UDim2` - | Produces a `Datatype.UDim2` with components that are the difference of the respective components of  |

## API Usage (34 locations)

### Used as Property Type

- `Class.BillboardGui.Size`
- `Class.GuiObject.Position`
- `Class.GuiObject.Size`
- `Class.ImageButton.TileSize`
- `Class.ImageLabel.TileSize`
- `Class.ScreenshotHud.CameraButtonPosition`
- `Class.ScreenshotHud.CloseButtonPosition`
- `Class.ScrollingFrame.CanvasSize`
- `Class.UIDragDetector.DragUDim2`
- `Class.UIDragDetector.MaxDragTranslation`
- `Class.UIDragDetector.MinDragTranslation`
- `Class.UIDragDetector.SelectionModeDragSpeed`
- `Class.UIGridLayout.CellPadding`
- `Class.UIGridLayout.CellSize`
- `Class.UIShadow.Offset`
- `Class.UIShadow.Spread`
- `Class.UITableLayout.Padding`
- `Class.VideoDisplay.TileSize`

### Used as Parameter Type

- `Class.ContextActionService:SetPosition` (parameter `position`)
- `Class.GuiObject:DragBegin` (parameter `initialPosition`)
- `Class.GuiObject:TweenPosition` (parameter `endPosition`)
- `Class.GuiObject:TweenPositionInternal` (parameter `endPosition`)
- `Class.GuiObject:TweenSize` (parameter `endSize`)
- `Class.GuiObject:TweenSizeAndPosition` (parameter `endPosition`)
- `Class.GuiObject:TweenSizeAndPosition` (parameter `endSize`)
- `Class.GuiObject:TweenSizeAndPositionInternal` (parameter `endPosition`)
- `Class.GuiObject:TweenSizeAndPositionInternal` (parameter `endSize`)
- `Class.GuiObject:TweenSizeInternal` (parameter `endSize`)
- `Class.GuiService:SendUIOcclusionMetricsForQueryRegion` (parameter `position`)
- `Class.GuiService:SendUIOcclusionMetricsForQueryRegion` (parameter `size`)
- `Class.Plugin:SelectRibbonTool` (parameter `position`)

### Used as Return Type

- `Class.Path2D:GetPositionOnCurve`
- `Class.Path2D:GetPositionOnCurveArcLength`
- `Class.UIDragDetector:GetReferencePosition`
