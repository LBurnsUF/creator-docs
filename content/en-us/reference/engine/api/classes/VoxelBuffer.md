---
title: VoxelBuffer
type: class
superclass: Object
tags: [NotCreatable, NotReplicated]
---

# VoxelBuffer

**Inherits**: Object

**Tags**: NotCreatable, NotReplicated

## Methods

- **ClearAsync**(`sizeInVoxels: Vector3?`) -> `null` [Yields]
- **DrawBufferAsync**(`cframe: CFrame`, `scale: float`, `source: VoxelBuffer`, `mergeConfig: Dictionary`) -> `null` [Yields]
- **FromHeightmapAsync**(`heightMap: buffer`, `width: int`, `height: int`, `heightMapRect: Rect`, `offset: float`, `scale: float`, `material: int`) -> `null` [Yields]
- **GetSizeInVoxels**() -> `Vector3`
- **NormalizeAsync**() -> `null` [Yields]
- **ReadVoxels**(`channelIds: Array`) -> `Dictionary` [CustomLuaState]
- **UnclampAsync**() -> `null` [Yields]
- **WriteVoxels**(`channels: Dictionary`) -> `null` [CustomLuaState]
