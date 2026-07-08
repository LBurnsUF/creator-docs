---
title: Ray
type: datatype
---

# `Datatype.Ray`

Represents a line with a starting point that casts infinitely in a specific
direction.

## Description

The `Datatype.Ray` data type represents a half-line, finite in one direction
but infinite in the other. It can be defined by a 3D point, where the line
originates from, and a direction vector, which is the direction it goes in.

## Constructors

### `Ray.new`

Returns a new `Datatype.Ray` with given `Origin` and `Direction`.

**Parameters:**

- `Origin`: `Vector3`
- `Direction`: `Vector3`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Ray.Unit` | `Ray` | The `Datatype.Ray` with a normalized direction (the direction has a magnitude of `1`). |
| `Ray.Origin` | `Vector3` | The position of the origin. |
| `Ray.Direction` | `Vector3` | The direction vector of the `Datatype.Ray`. |

## Methods

### `Ray:ClosestPoint`

Returns a `Datatype.Vector3` projected onto the ray so that it is within
the `Datatype.Ray` line of sight.

**Note:** the `Datatype.Ray` **must** be a unit ray for this method to
behave as expected!

**Parameters:**

- `point`: `Vector3`

### `Ray:Distance`

Returns the distance between the given point and the point on the ray
nearest to the given point (`Datatype.Ray.ClosestPoint(point)`).

**Parameters:**

- `point`: `Vector3`

## API Usage (13 locations)

### Used as Property Type

- `Class.Mouse.UnitRay`
- `Class.RayValue.Value`

### Used as Parameter Type

- `Class.DragDetector:DragContinue` (parameter `cursorRay`)
- `Class.DragDetector:DragStart` (parameter `cursorRay`)
- `Class.Dragger:MouseMove` (parameter `mouseRay`)
- `Class.RayValue:Changed` (parameter `value`)
- `Class.RayValue:changed` (parameter `value`)
- `Class.WorldRoot:FindPartOnRay` (parameter `ray`)
- `Class.WorldRoot:FindPartOnRayWithIgnoreList` (parameter `ray`)
- `Class.WorldRoot:FindPartOnRayWithWhitelist` (parameter `ray`)
- `Class.WorldRoot:findPartOnRay` (parameter `ray`)

### Used as Return Type

- `Class.Camera:ScreenPointToRay`
- `Class.Camera:ViewportPointToRay`
