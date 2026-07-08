---
title: RaycastParams
type: datatype
---

# `Datatype.RaycastParams`

A container for parameters used in raycasting operations.

## Description

The `Datatype.RaycastParams` data type stores parameters for
`Class.WorldRoot:Raycast()` operations. The
`Datatype.RaycastParams.ExcludeInstances|ExcludeInstances` and
`Datatype.RaycastParams.IncludeInstances|IncludeInstances` properties store a
set of objects and their descendants that will be excluded and included from
the query. The `Datatype.RaycastParams.IgnoreWater` property can be used to
ignore `Class.Terrain` water, and the `Datatype.RaycastParams.CollisionGroup`
property can specify a collision group for the raycasting operation.

This object is different from the similarly named `Datatype.RaycastResult`
which provides the results of a raycast.

Unlike most data types in Luau, you can change all of the members of
`Datatype.RaycastParams` without creating a new object, allowing you to reuse
the same object repeatedly.

## Constructors

### `RaycastParams.new`

Returns a blank `Datatype.RaycastParams` object. Unlike other data type
constructors, this constructor does not have any parameters, so you should
set its properties appropriately.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `RaycastParams.ExcludeInstances` | `{Instance}?` | An optional array of instances whose descendants will be excluded from the query. |
| `RaycastParams.IncludeInstances` | `{Instance}?` | An optional array of instances whose descendants will be included in the query. |
| `RaycastParams.IgnoreWater` | `bool` | Determines whether the water material is considered when raycasting against `Class.Terrain`. |
| `RaycastParams.CollisionGroup` | `string` | The collision group used for the operation. |
| `RaycastParams.RespectCanCollide` | `bool` | Determines whether the raycast operation considers a part's `Class.BasePart.CanCollide/CanCollide` p |
| `RaycastParams.BruteForceAllSlow` | `bool` | When enabled, the query will ignore all part collision properties and perform a brute-force check on |
| `RaycastParams.FilterDescendantsInstances` | `Array` | An array of objects whose descendants are used to filter raycasting candidates. |
| `RaycastParams.FilterType` | `RaycastFilterType` | Determines whether the `Datatype.RaycastParams.FilterDescendantsInstances/FilterDescendantsInstances |

## Methods

### `RaycastParams:AddToFilter`

Adds the instances provided to
`Datatype.RaycastParams.FilterDescendantsInstances|FilterDescendantsInstances`.
Note that this property has been superseded by
`Datatype.RaycastParams.ExcludeInstances|ExcludeInstances` and
`Datatype.RaycastParams.IncludeInstances|IncludeInstances` which should be
used for new work.

**Parameters:**

- `instances`: `Instance | Array` - An instance or an array containing instances to add.

## API Usage (5 locations)

### Used as Parameter Type

- `Class.StudioService:GizmoRaycast` (parameter `raycastParams`)
- `Class.WorldRoot:Blockcast` (parameter `params`)
- `Class.WorldRoot:Raycast` (parameter `raycastParams`)
- `Class.WorldRoot:Shapecast` (parameter `params`)
- `Class.WorldRoot:Spherecast` (parameter `params`)
