---
title: OverlapParams
type: datatype
---

# `Datatype.OverlapParams`

Stores parameters used in boundary-querying functions.

## Description

The `Datatype.OverlapParams` data type stores parameters for use with
`Class.WorldRoot` boundary-querying functions, in particular
`Class.WorldRoot:GetPartBoundsInBox()`,
`Class.WorldRoot:GetPartBoundsInRadius()` and
`Class.WorldRoot:GetPartsInPart()`. The
`Datatype.OverlapParams.ExcludeInstances|ExcludeInstances` and
`Datatype.OverlapParams.IncludeInstances|IncludeInstances` properties store a
set of objects and their descendants that will be excluded and included from
the query. The `Datatype.OverlapParams.CollisionGroup` property can specify a
collision group for the boundary query operation.

Unlike most data types in Luau, you can change all of the members of
`Datatype.OverlapParams` without creating a new object, allowing you to reuse
the same object repeatedly.

## Constructors

### `OverlapParams.new`

Returns a blank `Datatype.OverlapParams` object. Unlike other data type
constructors, this constructor does not have any parameters, so you should
set its properties appropriately.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `OverlapParams.ExcludeInstances` | `{Instance}?` | An optional array of instances whose descendants will be excluded from the query. |
| `OverlapParams.IncludeInstances` | `{Instance}?` | An optional array of instances whose descendants will be included in the query. |
| `OverlapParams.MaxParts` | `number` | The maximum amount of parts to be returned by the query. |
| `OverlapParams.CollisionGroup` | `string` | The collision group used for the operation. |
| `OverlapParams.Tolerance` | `number` | Slightly increases the volume of the boundary-querying operation. |
| `OverlapParams.RespectCanCollide` | `bool` | Determines whether the boundary-querying operation considers a part's `Class.BasePart.CanCollide` pr |
| `OverlapParams.BruteForceAllSlow` | `bool` | When enabled, the query will ignore all part collision properties and perform a brute-force check on |
| `OverlapParams.FilterDescendantsInstances` | `Array` | An array of objects whose descendants are used in filtering candidates. |
| `OverlapParams.FilterType` | `RaycastFilterType` | Determines whether the `Datatype.OverlapParams.FilterDescendantsInstances/FilterDescendantsInstances |

## Methods

### `OverlapParams:AddToFilter`

Adds the instances provided to
`Datatype.OverlapParams.FilterDescendantsInstances|FilterDescendantsInstances`.
Note that this property has been superseded by
`Datatype.OverlapParams.ExcludeInstances|ExcludeInstances` and
`Datatype.OverlapParams.IncludeInstances|IncludeInstances` which should be
used for new work.

**Parameters:**

- `instances`: `Instance | Array` - An instance or an array containing instances to add.

## API Usage (3 locations)

### Used as Parameter Type

- `Class.WorldRoot:GetPartBoundsInBox` (parameter `overlapParams`)
- `Class.WorldRoot:GetPartBoundsInRadius` (parameter `overlapParams`)
- `Class.WorldRoot:GetPartsInPart` (parameter `overlapParams`)
