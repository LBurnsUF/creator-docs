---
title: Path2DControlPoint
type: datatype
---

# `Datatype.Path2DControlPoint`

Stores the info for a single control point used with the `Class.Path2D`
instance.

## Description

The `Path2DControlPoint` data type represents a single control point used with
the `Class.Path2D` instance.

## Constructors

### `Path2DControlPoint.new`

Returns an empty `Datatype.Path2DControlPoint`.

### `Path2DControlPoint.new`

Returns a `Datatype.Path2DControlPoint` with the position set. This 
constructor will set the tangents to default `Datatype.UDim2` values.

**Parameters:**

- `Position`: `UDim2` - The `Datatype.UDim2` position of the control point.

### `Path2DControlPoint.new`

Returns a `Datatype.Path2DControlPoint` with the position, left
tangent, and right tangent set.

**Parameters:**

- `Position`: `UDim2` - The `Datatype.UDim2` position of the control point.
- `Left Tangent`: `UDim2` - The `Datatype.UDim2` left tangent of the control point.
- `Right Tangent`: `UDim2` - The `Datatype.UDim2` right tangent of the control point.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Path2DControlPoint.Position` | `UDim2` | The position of the `Datatype.Path2DControlPoint`. |
| `Path2DControlPoint.LeftTangent` | `UDim2` | The left tangent of the `Datatype.Path2DControlPoint`. |
| `Path2DControlPoint.RightTangent` | `UDim2` | The right tangent of the `Datatype.Path2DControlPoint`. |

## API Usage (4 locations)

### Used as Property Type

- `Class.Path2D.SelectedControlPointData`

### Used as Parameter Type

- `Class.Path2D:InsertControlPoint` (parameter `point`)
- `Class.Path2D:UpdateControlPoint` (parameter `point`)

### Used as Return Type

- `Class.Path2D:GetControlPoint`
