---
title: Region3int16
type: datatype
---

# `Datatype.Region3int16`

Represents a Region3 stored as two boundaries as opposed to position and size
components.

## Description

Not to be confused with `Datatype.Region3`, a separate class that fulfills a
different purpose.

The `Datatype.Region3int16` data type represents a volume in 3D space similar
to an **axis-aligned rectangular prism**. It uses two `Datatype.Vector3int16`
to store the volume's bounds in the `Min` and `Max` properties. It is
constructed using `Region3int16.new(Min, Max)`, given the two
`Datatype.Vector3int16` bounds. This data type features no functions or
operations.

## Calculating Center and Size

This data type differs from `Datatype.Region3` in that it stores its bounds
directly, rather than through a center and size combination. Nonetheless, it
is possible to calculate these dimensions using `Min` and `Max`:

```lua
local region = Region3int16.new(Vector3int16.new(0, 0, -3), Vector3int16.new(4, 4, 4))
local size = region.Max - region.Min
local center = (region.Max + region.Min) / 2
```

## Conversion to Region3

The following function can be used to convert a Region3int16 into a similar
`Datatype.Region3`. It does this by converting the `Min` and `Max` properties,
which are Vector3int16, into `Datatype.Vector3` used with
`Datatype.Region3.new()`.

```lua
local function Region3int16toRegion3(region16)
	return Region3.new(
		Vector3.new(region16.Min.X, region16.Min.Y, region16.Min.Z),
		Vector3.new(region16.Max.X, region16.Max.Y, region16.Max.Z)
	)
end
```

See also:

- `Datatype.Region3`, a similar data type

## Constructors

### `Region3int16.new`

Returns a new Region3int16 from the provided boundaries.

**Parameters:**

- `min`: `Vector3int16`
- `max`: `Vector3int16`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Region3int16.Min` | `Vector3int16` | The lower bound of the `Datatype.Region3int16`. |
| `Region3int16.Max` | `Vector3int16` | The upper bound of the `Datatype.Region3int16`. |

## API Usage (7 locations)

### Used as Property Type

- `Class.Terrain.MaxExtents`

### Used as Parameter Type

- `Class.Terrain:AutowedgeCells` (parameter `region`)
- `Class.Terrain:CopyRegion` (parameter `region`)
- `Class.Terrain:ReplaceMaterialInTransformSubregion` (parameter `targetRegion`)
- `Class.Terrain:SetCells` (parameter `region`)
- `Class.Terrain:SetMaterialInTransformSubregion` (parameter `targetRegion`)
- `Class.TerrainRegion:ApplyTransformSubregion` (parameter `region`)
