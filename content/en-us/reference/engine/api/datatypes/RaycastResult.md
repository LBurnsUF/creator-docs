---
title: RaycastResult
type: datatype
---

# `Datatype.RaycastResult`

Stores results from a raycast operation.

## Description

The `Datatype.RaycastResult` data type stores the result of a successful
raycasting operation performed by `Class.WorldRoot:Raycast()`. It contains the
properties listed below.

This object should not be confused with the similarly-named
`Datatype.RaycastParams` which is used to perform a raycast.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `RaycastResult.Distance` | `number` | The distance between the ray origin and the intersection point. |
| `RaycastResult.Instance` | `BasePart` | The `Class.BasePart` or `Class.Terrain` cell that the ray intersected. |
| `RaycastResult.Material` | `Material` | The `Enum.Material` at the intersection point. |
| `RaycastResult.Position` | `Vector3` | The world space point at which the intersection occurred. |
| `RaycastResult.Normal` | `Vector3` | The normal vector of the intersected face. |

## API Usage (6 locations)

### Used as Return Type

- `Class.StudioService:GizmoRaycast`
- `Class.WorldRoot:Blockcast`
- `Class.WorldRoot:Raycast`
- `Class.WorldRoot:RaycastCachedTerrain`
- `Class.WorldRoot:Shapecast`
- `Class.WorldRoot:Spherecast`
