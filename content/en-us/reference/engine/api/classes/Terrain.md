---
title: Terrain
type: class
superclass: BasePart
tags: [NotCreatable]
---

# Terrain

**Inherits**: BasePart > PVInstance > Instance > Object

**Tags**: NotCreatable

## Properties

- **Decoration**: `bool` [NotScriptable]
- **GrassLength**: `float` [NotScriptable]
- **IsSmooth**: `bool` [ReadOnly] [NotReplicated] [Deprecated]
- **LastUsedModificationMethod**: `TerrainAcquisitionMethod` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **MaterialColors**: `BinaryString` [NotScriptable]
- **MaxExtents**: `Region3int16` [ReadOnly] [NotReplicated]
- **SmoothVoxelsUpgraded**: `bool` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **WaterColor**: `Color3`
- **WaterReflectance**: `float`
- **WaterTransparency**: `float`
- **WaterWaveSize**: `float`
- **WaterWaveSpeed**: `float`

## Methods

- **AutowedgeCell**(`x: int`, `y: int`, `z: int`) -> `bool` [Deprecated]
- **AutowedgeCells**(`region: Region3int16`) -> `null` [Deprecated]
- **CanSmoothVoxelsBeUpgraded**() -> `bool`
- **CellCenterToWorld**(`x: int`, `y: int`, `z: int`) -> `Vector3`
- **CellCornerToWorld**(`x: int`, `y: int`, `z: int`) -> `Vector3`
- **Clear**() -> `null`
- **ClearVoxelsAsync_beta**(`region: Region3`, `channelIds: Array`) -> `null` [CustomLuaState]
- **ConvertToSmooth**() -> `null` [Deprecated]
- **CopyRegion**(`region: Region3int16`) -> `TerrainRegion`
- **CountCells**() -> `int`
- **CreateVoxelBuffer_beta**() -> `VoxelBuffer`
- **DrawBufferAsync**(`cframe: CFrame`, `scale: float`, `resolution: int`, `source: VoxelBuffer`, `mergeConfig: Dictionary`) -> `null` [Yields]
- **FillBall**(`center: Vector3`, `radius: float`, `material: Material`) -> `null`
- **FillBlock**(`cframe: CFrame`, `size: Vector3`, `material: Material`) -> `null`
- **FillCylinder**(`cframe: CFrame`, `height: float`, `radius: float`, `material: Material`) -> `null`
- **FillRegion**(`region: Region3`, `resolution: float`, `material: Material`) -> `null`
- **FillWedge**(`cframe: CFrame`, `size: Vector3`, `material: Material`) -> `null`
- **GetCell**(`x: int`, `y: int`, `z: int`) -> `Tuple` [Deprecated]
- **GetMaterialColor**(`material: Material`) -> `Color3`
- **GetMaterialSlot**(`slotIndex: int`) -> `Tuple`
- **GetTerrainWireframe**(`cframe: CFrame`, `size: Vector3`) -> `Array`
- **GetWaterCell**(`x: int`, `y: int`, `z: int`) -> `Tuple` [Deprecated]
- **IterateVoxelsAsync_beta**(`region: Region3`, `resolution: int`, `channelIds: Array`) -> `TerrainIterateOperation` [CustomLuaState]
- **ModifyVoxelsAsync_beta**(`region: Region3`, `resolution: int`, `channelIds: Array`) -> `TerrainModifyOperation` [CustomLuaState]
- **PasteRegion**(`region: TerrainRegion`, `corner: Vector3int16`, `pasteEmptyCells: bool`) -> `null`
- **ReadBufferAsync**(`region: Region3`, `resolution: int`) -> `VoxelBuffer` [Yields]
- **ReadVoxelChannels**(`region: Region3`, `resolution: float`, `channelIds: Array`) -> `Dictionary` [CustomLuaState]
- **ReadVoxels**(`region: Region3`, `resolution: float`) -> `Tuple` [CustomLuaState]
- **ReadVoxelsAsync_beta**(`region: Region3`, `resolution: int`, `channelIds: Array`) -> `TerrainReadOperation` [CustomLuaState]
- **ReplaceMaterial**(`region: Region3`, `resolution: float`, `sourceMaterial: Material`, `targetMaterial: Material`) -> `null`
- **ReplaceMaterialInTransform**(`cframe: CFrame`, `size: Vector3`, `sourceMaterial: Material`, `targetMaterial: Material`) -> `null`
- **ReplaceMaterialInTransformSubregion**(`cframe: CFrame`, `size: Vector3`, `sourceMaterial: Material`, `targetMaterial: Material`, `targetRegion: Region3int16`) -> `null`
- **ResetMaterialSlot**(`slotIndex: int`) -> `null`
- **SetCell**(`x: int`, `y: int`, `z: int`, `material: CellMaterial`, `block: CellBlock`, `orientation: CellOrientation`) -> `null` [Deprecated]
- **SetCells**(`region: Region3int16`, `material: CellMaterial`, `block: CellBlock`, `orientation: CellOrientation`) -> `null` [Deprecated]
- **SetMaterialColor**(`material: Material`, `value: Color3`) -> `null`
- **SetMaterialInTransform**(`cframe: CFrame`, `size: Vector3`, `targetMaterial: Material`) -> `null`
- **SetMaterialInTransformSubregion**(`cframe: CFrame`, `size: Vector3`, `targetMaterial: Material`, `targetRegion: Region3int16`) -> `null`
- **SetMaterialSlot**(`slotIndex: int`, `baseMaterial: Material`, `materialVariant: string`, `color: Color3`) -> `null`
- **SetWaterCell**(`x: int`, `y: int`, `z: int`, `force: WaterForce`, `direction: WaterDirection`) -> `null` [Deprecated]
- **SmoothRegion**(`region: Region3`, `resolution: float`, `strength: float`) -> `Tuple` [CustomLuaState]
- **WorldToCell**(`position: Vector3`) -> `Vector3`
- **WorldToCellPreferEmpty**(`position: Vector3`) -> `Vector3`
- **WorldToCellPreferSolid**(`position: Vector3`) -> `Vector3`
- **WriteVoxelChannels**(`region: Region3`, `resolution: float`, `channels: Dictionary`) -> `null` [CustomLuaState]
- **WriteVoxels**(`region: Region3`, `resolution: float`, `materials: Array`, `occupancy: Array`) -> `null` [CustomLuaState]
- **WriteVoxelsAsync_beta**(`region: Region3`, `resolution: int`, `channelIds: Array`) -> `TerrainWriteOperation` [CustomLuaState]
