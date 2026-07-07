---
title: Terrain
type: class
superclass: BasePart
tags: [NotCreatable]
---

# Terrain

**Inherits from:** `Class.BasePart` > `Class.PVInstance` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.Terrain.Decoration` | `bool` | [NotScriptable] |
| `Class.Terrain.GrassLength` | `float` | [NotScriptable] |
| `Class.Terrain.IsSmooth` | `bool` | [ReadOnly] [NotReplicated] [Deprecated] |
| `Class.Terrain.LastUsedModificationMethod` | `Enum.TerrainAcquisitionMethod` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Terrain.MaterialColors` | `Datatype.BinaryString` | [NotScriptable] |
| `Class.Terrain.MaxExtents` | `Datatype.Region3int16` | [ReadOnly] [NotReplicated] |
| `Class.Terrain.SmoothVoxelsUpgraded` | `bool` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.Terrain.WaterColor` | `Datatype.Color3` |  |
| `Class.Terrain.WaterReflectance` | `float` |  |
| `Class.Terrain.WaterTransparency` | `float` |  |
| `Class.Terrain.WaterWaveSize` | `float` |  |
| `Class.Terrain.WaterWaveSpeed` | `float` |  |

## Methods

### `Class.Terrain:AutowedgeCell`

``AutowedgeCell(x: `int`, y: `int`, z: `int`)`` → `bool`
  [Deprecated]

### `Class.Terrain:AutowedgeCells`

``AutowedgeCells(region: `Datatype.Region3int16`)`` → `null`
  [Deprecated]

### `Class.Terrain:CanSmoothVoxelsBeUpgraded`

``CanSmoothVoxelsBeUpgraded()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.Terrain:CellCenterToWorld`

``CellCenterToWorld(x: `int`, y: `int`, z: `int`)`` → `Datatype.Vector3`

### `Class.Terrain:CellCornerToWorld`

``CellCornerToWorld(x: `int`, y: `int`, z: `int`)`` → `Datatype.Vector3`

### `Class.Terrain:Clear`

``Clear()`` → `null`

### `Class.Terrain:ClearVoxelsAsync_beta`

``ClearVoxelsAsync_beta(region: `Datatype.Region3`, channelIds: `Array`)`` → `null`
  [CustomLuaState]

### `Class.Terrain:ConvertToSmooth`

``ConvertToSmooth()`` → `null`
  [Deprecated] {security: PluginSecurity}

### `Class.Terrain:CopyRegion`

``CopyRegion(region: `Datatype.Region3int16`)`` → `Class.TerrainRegion`

### `Class.Terrain:CountCells`

``CountCells()`` → `int`

### `Class.Terrain:CreateVoxelBuffer_beta`

``CreateVoxelBuffer_beta()`` → `Class.VoxelBuffer`
   {security: RobloxScriptSecurity}

### `Class.Terrain:DrawBufferAsync`

``DrawBufferAsync(cframe: `Datatype.CFrame`, scale: `float`, resolution: `int`, source: `Class.VoxelBuffer`, mergeConfig: `Dictionary`)`` → `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.Terrain:FillBall`

``FillBall(center: `Datatype.Vector3`, radius: `float`, material: `Enum.Material`)`` → `null`

### `Class.Terrain:FillBlock`

``FillBlock(cframe: `Datatype.CFrame`, size: `Datatype.Vector3`, material: `Enum.Material`)`` → `null`

### `Class.Terrain:FillCylinder`

``FillCylinder(cframe: `Datatype.CFrame`, height: `float`, radius: `float`, material: `Enum.Material`)`` → `null`

### `Class.Terrain:FillRegion`

``FillRegion(region: `Datatype.Region3`, resolution: `float`, material: `Enum.Material`)`` → `null`

### `Class.Terrain:FillWedge`

``FillWedge(cframe: `Datatype.CFrame`, size: `Datatype.Vector3`, material: `Enum.Material`)`` → `null`

### `Class.Terrain:GetCell`

``GetCell(x: `int`, y: `int`, z: `int`)`` → `Tuple`
  [Deprecated]

### `Class.Terrain:GetMaterialColor`

``GetMaterialColor(material: `Enum.Material`)`` → `Datatype.Color3`

### `Class.Terrain:GetMaterialSlot`

``GetMaterialSlot(slotIndex: `int`)`` → `Tuple`

### `Class.Terrain:GetTerrainWireframe`

``GetTerrainWireframe(cframe: `Datatype.CFrame`, size: `Datatype.Vector3`)`` → `Array`
   {security: RobloxScriptSecurity}

### `Class.Terrain:GetWaterCell`

``GetWaterCell(x: `int`, y: `int`, z: `int`)`` → `Tuple`
  [Deprecated]

### `Class.Terrain:IterateVoxelsAsync_beta`

``IterateVoxelsAsync_beta(region: `Datatype.Region3`, resolution: `int`, channelIds: `Array`)`` → `Class.TerrainIterateOperation`
  [CustomLuaState]

### `Class.Terrain:ModifyVoxelsAsync_beta`

``ModifyVoxelsAsync_beta(region: `Datatype.Region3`, resolution: `int`, channelIds: `Array`)`` → `Class.TerrainModifyOperation`
  [CustomLuaState]

### `Class.Terrain:PasteRegion`

``PasteRegion(region: `Class.TerrainRegion`, corner: `Datatype.Vector3int16`, pasteEmptyCells: `bool`)`` → `null`

### `Class.Terrain:ReadBufferAsync`

``ReadBufferAsync(region: `Datatype.Region3`, resolution: `int`)`` → `Class.VoxelBuffer`
  [Yields] {security: RobloxScriptSecurity}

### `Class.Terrain:ReadVoxelChannels`

``ReadVoxelChannels(region: `Datatype.Region3`, resolution: `float`, channelIds: `Array`)`` → `Dictionary`
  [CustomLuaState]

### `Class.Terrain:ReadVoxels`

``ReadVoxels(region: `Datatype.Region3`, resolution: `float`)`` → `Tuple`
  [CustomLuaState]

### `Class.Terrain:ReadVoxelsAsync_beta`

``ReadVoxelsAsync_beta(region: `Datatype.Region3`, resolution: `int`, channelIds: `Array`)`` → `Class.TerrainReadOperation`
  [CustomLuaState]

### `Class.Terrain:ReplaceMaterial`

``ReplaceMaterial(region: `Datatype.Region3`, resolution: `float`, sourceMaterial: `Enum.Material`, targetMaterial: `Enum.Material`)`` → `null`

### `Class.Terrain:ReplaceMaterialInTransform`

``ReplaceMaterialInTransform(cframe: `Datatype.CFrame`, size: `Datatype.Vector3`, sourceMaterial: `Enum.Material`, targetMaterial: `Enum.Material`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Terrain:ReplaceMaterialInTransformSubregion`

``ReplaceMaterialInTransformSubregion(cframe: `Datatype.CFrame`, size: `Datatype.Vector3`, sourceMaterial: `Enum.Material`, targetMaterial: `Enum.Material`, targetRegion: `Datatype.Region3int16`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Terrain:ResetMaterialSlot`

``ResetMaterialSlot(slotIndex: `int`)`` → `null`

### `Class.Terrain:SetCell`

``SetCell(x: `int`, y: `int`, z: `int`, material: `Enum.CellMaterial`, block: `Enum.CellBlock`, orientation: `Enum.CellOrientation`)`` → `null`
  [Deprecated]

### `Class.Terrain:SetCells`

``SetCells(region: `Datatype.Region3int16`, material: `Enum.CellMaterial`, block: `Enum.CellBlock`, orientation: `Enum.CellOrientation`)`` → `null`
  [Deprecated]

### `Class.Terrain:SetMaterialColor`

``SetMaterialColor(material: `Enum.Material`, value: `Datatype.Color3`)`` → `null`

### `Class.Terrain:SetMaterialInTransform`

``SetMaterialInTransform(cframe: `Datatype.CFrame`, size: `Datatype.Vector3`, targetMaterial: `Enum.Material`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Terrain:SetMaterialInTransformSubregion`

``SetMaterialInTransformSubregion(cframe: `Datatype.CFrame`, size: `Datatype.Vector3`, targetMaterial: `Enum.Material`, targetRegion: `Datatype.Region3int16`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Terrain:SetMaterialSlot`

``SetMaterialSlot(slotIndex: `int`, baseMaterial: `Enum.Material`, materialVariant: `string`, color: `Datatype.Color3`)`` → `null`

### `Class.Terrain:SetWaterCell`

``SetWaterCell(x: `int`, y: `int`, z: `int`, force: `Enum.WaterForce`, direction: `Enum.WaterDirection`)`` → `null`
  [Deprecated]

### `Class.Terrain:SmoothRegion`

``SmoothRegion(region: `Datatype.Region3`, resolution: `float`, strength: `float`)`` → `Tuple`
  [CustomLuaState] {security: RobloxScriptSecurity}

### `Class.Terrain:WorldToCell`

``WorldToCell(position: `Datatype.Vector3`)`` → `Datatype.Vector3`

### `Class.Terrain:WorldToCellPreferEmpty`

``WorldToCellPreferEmpty(position: `Datatype.Vector3`)`` → `Datatype.Vector3`

### `Class.Terrain:WorldToCellPreferSolid`

``WorldToCellPreferSolid(position: `Datatype.Vector3`)`` → `Datatype.Vector3`

### `Class.Terrain:WriteVoxelChannels`

``WriteVoxelChannels(region: `Datatype.Region3`, resolution: `float`, channels: `Dictionary`)`` → `null`
  [CustomLuaState]

### `Class.Terrain:WriteVoxels`

``WriteVoxels(region: `Datatype.Region3`, resolution: `float`, materials: `Array`, occupancy: `Array`)`` → `null`
  [CustomLuaState]

### `Class.Terrain:WriteVoxelsAsync_beta`

``WriteVoxelsAsync_beta(region: `Datatype.Region3`, resolution: `int`, channelIds: `Array`)`` → `Class.TerrainWriteOperation`
  [CustomLuaState]
