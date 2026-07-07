---
title: TerrainRegion
type: class
superclass: Instance
---

# TerrainRegion

**Inherits**: Instance > Object

## Properties

- **IsSmooth**: `bool` [ReadOnly] [NotReplicated] [Deprecated]
- **SizeInCells**: `Vector3` [ReadOnly] [NotReplicated]

## Methods

- **ApplyTransform**(`rotation: CFrame`, `size: Vector3`) -> `null`
- **ApplyTransformSubregion**(`rotation: CFrame`, `size: Vector3`, `region: Region3int16`) -> `TerrainRegion`
- **ConvertToSmooth**() -> `null` [Deprecated]
- **GetRegionWireframe**() -> `Array`
