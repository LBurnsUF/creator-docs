---
title: Region3
type: datatype
---

# `Datatype.Region3`

Describes a rectangular volume in 3D space.

## Description

The `Datatype.Region3` data type describes a volume in 3D space similar to an
**axis-aligned rectangular prism**. It is commonly used with `Class.Terrain`
functions and functions that detect parts within a volume, such as
`Class.WorldRoot:FindPartsInRegion3()`.

The prism's center is accessible using the `Datatype.Region3.CFrame` property
and the prism's size is accessible through the `Datatype.Region3.Size`
property. Note that the components of this property may be **negative**.

The `Datatype.Region3:ExpandToGrid()` method returns a new `Datatype.Region3`
whose bounds comply with a provided resolution value. The resulting volume may
be equal to or greater than the original volume, but never smaller.

See also:

- `Datatype.Region3int16`

## Constructors

### `Region3.new`

Returns a new `Datatype.Region3` given the `Datatype.Vector3` bounds of the
rectangular prism volume.

Note that the order of the provided bounds matters: by switching them, the
polarity of the size components will switch. It is possible to create a
`Datatype.Region3` with a **negative volume**.

**Parameters:**

- `min`: `Vector3`
- `max`: `Vector3`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Region3.CFrame` | `CFrame` | The center location and rotation of the `Datatype.Region3`. |
| `Region3.Size` | `Vector3` | The 3D size of the `Datatype.Region3`. |

## Methods

### `Region3:ExpandToGrid`

Expands the `Datatype.Region3` based on the provided resolution and
returns the expanded `Datatype.Region3` aligned to the `Class.Terrain`
voxel grid.

**Parameters:**

- `resolution`: `number`

## API Usage (20 locations)

### Used as Parameter Type

- `Class.HeightmapImporterService:ImportHeightmap` (parameter `region`)
- `Class.Terrain:ClearVoxelsAsync_beta` (parameter `region`)
- `Class.Terrain:FillRegion` (parameter `region`)
- `Class.Terrain:IterateVoxelsAsync_beta` (parameter `region`)
- `Class.Terrain:ModifyVoxelsAsync_beta` (parameter `region`)
- `Class.Terrain:ReadBufferAsync` (parameter `region`)
- `Class.Terrain:ReadVoxelChannels` (parameter `region`)
- `Class.Terrain:ReadVoxels` (parameter `region`)
- `Class.Terrain:ReadVoxelsAsync_beta` (parameter `region`)
- `Class.Terrain:ReplaceMaterial` (parameter `region`)
- `Class.Terrain:SmoothRegion` (parameter `region`)
- `Class.Terrain:WriteVoxelChannels` (parameter `region`)
- `Class.Terrain:WriteVoxels` (parameter `region`)
- `Class.Terrain:WriteVoxelsAsync_beta` (parameter `region`)
- `Class.WorldRoot:FindPartsInRegion3` (parameter `region`)
- `Class.WorldRoot:FindPartsInRegion3WithIgnoreList` (parameter `region`)
- `Class.WorldRoot:FindPartsInRegion3WithWhiteList` (parameter `region`)
- `Class.WorldRoot:IsRegion3Empty` (parameter `region`)
- `Class.WorldRoot:IsRegion3EmptyWithIgnoreList` (parameter `region`)
- `Class.WorldRoot:findPartsInRegion3` (parameter `region`)
