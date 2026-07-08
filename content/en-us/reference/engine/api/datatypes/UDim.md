---
title: UDim
type: datatype
---

# `Datatype.UDim`

Represents a one-dimensional value with two components, a relative scale and
an absolute offset.

## Description

The `Datatype.UDim` data type represents a one-dimensional value with two
components, a relative scale and an absolute offset in pixels.

## Constructors

### `UDim.new`

Returns a `Datatype.UDim` from the given components.

**Parameters:**

- `Scale`: `number`
- `Offset`: `number`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `UDim.Scale` | `number` | The relative scale component of the `Datatype.UDim`. |
| `UDim.Offset` | `number` | The absolute offset component of the `Datatype.UDim`. |

## Math Operations

| Operation | Description |
|-----------|-------------|
| `UDim` + | Produces a `Datatype.UDim` representing the sum of the two `Datatype.UDim` values. |
| `UDim` - | Produces a `Datatype.UDim` representing the difference between the two `Datatype.UDim` values. |

## API Usage (13 locations)

### Used as Property Type

- `Class.UICorner.BottomLeftRadius`
- `Class.UICorner.BottomRightRadius`
- `Class.UICorner.CornerRadius`
- `Class.UICorner.TopLeftRadius`
- `Class.UICorner.TopRightRadius`
- `Class.UIListLayout.Padding`
- `Class.UIPadding.PaddingBottom`
- `Class.UIPadding.PaddingLeft`
- `Class.UIPadding.PaddingRight`
- `Class.UIPadding.PaddingTop`
- `Class.UIPageLayout.Padding`
- `Class.UIShadow.BlurRadius`
- `Class.UIStroke.BorderOffset`
