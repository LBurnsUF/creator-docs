---
title: Rect
type: datatype
---

# `Datatype.Rect`

A value that represents a two-dimensional rectangle.

## Description

**Rect** describes a rectangle on a 2D plane. It is constructed using two
corners, either two `Datatype.Vector2` positions or four numbers:

```lua
local rect1 = Rect.new(Vector2.new(10, 10), Vector2.new(80, 80))
local rect2 = Rect.new(10, 10, 80, 80)
```

This data type is used in the `Class.ImageLabel.SliceCenter` property which
determines the center area of a scaled image.

## Constructors

### `Rect.new`

Constructs a new **Rect** with two zero `Datatype.Vector2` positions.

### `Rect.new`

Constructs a new **Rect** given two `Datatype.Vector2` positions: `min` as
the top-left corner and `max` as the bottom-right corner.

**Parameters:**

- `min`: `Vector2`
- `max`: `Vector2`

### `Rect.new`

Constructs a new **Rect** using `minX` and `minY` as coordinates for the
top-left corner, and `maxX` and `maxY` as coordinates for the bottom-right
corner.

**Parameters:**

- `minX`: `number`
- `minY`: `number`
- `maxX`: `number`
- `maxY`: `number`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Rect.Width` | `number` | The width of the **Rect**. |
| `Rect.Height` | `number` | The height of the **Rect**. |
| `Rect.Min` | `Vector2` | The coordinates of the top-left corner. |
| `Rect.Max` | `Vector2` | The coordinates of the bottom-right corner. |

## API Usage (12 locations)

### Used as Property Type

- `Class.GuiBase2d.ClippedRect`
- `Class.GuiBase2d.RawRect2D`
- `Class.GuiObject.SelectionRect2D`
- `Class.GuiService.TopbarInset`
- `Class.ImageButton.SliceCenter`
- `Class.ImageLabel.SliceCenter`
- `Class.ScrollingFrame.HorizontalBarRect`
- `Class.ScrollingFrame.VerticalBarRect`

### Used as Parameter Type

- `Class.GuiService:SetTopbarInset` (parameter `topbarInset`)
- `Class.VoxelBuffer:FromHeightmapAsync` (parameter `heightMapRect`)

### Used as Return Type

- `Class.GuiService:GetInsetArea`
- `Class.Path2D:GetBoundingRect`
