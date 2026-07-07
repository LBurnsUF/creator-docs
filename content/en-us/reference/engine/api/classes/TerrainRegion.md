---
title: TerrainRegion
type: class
superclass: Instance
---

# TerrainRegion

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.TerrainRegion.IsSmooth` | `bool` | [ReadOnly] [NotReplicated] [Deprecated] |
| `Class.TerrainRegion.SizeInCells` | `Datatype.Vector3` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.TerrainRegion:ApplyTransform`

``ApplyTransform(rotation: `Datatype.CFrame`, size: `Datatype.Vector3`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.TerrainRegion:ApplyTransformSubregion`

``ApplyTransformSubregion(rotation: `Datatype.CFrame`, size: `Datatype.Vector3`, region: `Datatype.Region3int16`)`` → `Class.TerrainRegion`
   {security: RobloxScriptSecurity}

### `Class.TerrainRegion:ConvertToSmooth`

``ConvertToSmooth()`` → `null`
  [Deprecated] {security: PluginSecurity}

### `Class.TerrainRegion:GetRegionWireframe`

``GetRegionWireframe()`` → `Array`
   {security: RobloxScriptSecurity}
