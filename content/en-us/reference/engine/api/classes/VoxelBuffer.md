---
title: VoxelBuffer
type: class
superclass: Object
tags: [NotCreatable, NotReplicated]
---

# VoxelBuffer

**Inherits from:** `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Methods

### `Class.VoxelBuffer:ClearAsync`

``ClearAsync(sizeInVoxels: `Datatype.Vector3`?)`` → `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.VoxelBuffer:DrawBufferAsync`

``DrawBufferAsync(cframe: `Datatype.CFrame`, scale: `float`, source: `Class.VoxelBuffer`, mergeConfig: `Dictionary`)`` → `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.VoxelBuffer:FromHeightmapAsync`

``FromHeightmapAsync(heightMap: `Datatype.buffer`, width: `int`, height: `int`, heightMapRect: `Datatype.Rect`, offset: `float`, scale: `float`, material: `int`)`` → `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.VoxelBuffer:GetSizeInVoxels`

``GetSizeInVoxels()`` → `Datatype.Vector3`
   {security: RobloxScriptSecurity}

### `Class.VoxelBuffer:NormalizeAsync`

``NormalizeAsync()`` → `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.VoxelBuffer:ReadVoxels`

``ReadVoxels(channelIds: `Array`)`` → `Dictionary`
  [CustomLuaState] {security: RobloxScriptSecurity}

### `Class.VoxelBuffer:UnclampAsync`

``UnclampAsync()`` → `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.VoxelBuffer:WriteVoxels`

``WriteVoxels(channels: `Dictionary`)`` → `null`
  [CustomLuaState] {security: RobloxScriptSecurity}
