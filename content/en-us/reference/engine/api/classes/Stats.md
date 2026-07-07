---
title: Stats
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# Stats

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Properties

- **ContactsCount**: `int` [ReadOnly] [NotReplicated]
- **DataReceiveKbps**: `float` [ReadOnly] [NotReplicated]
- **DataSendKbps**: `float` [ReadOnly] [NotReplicated]
- **FrameTime**: `float` [ReadOnly] [NotReplicated]
- **HeartbeatTime**: `float` [ReadOnly] [NotReplicated]
- **HeartbeatTimeMs**: `float` [ReadOnly] [NotReplicated] [Deprecated]
- **InstanceCount**: `int` [ReadOnly] [NotReplicated]
- **MemoryTrackingEnabled**: `bool` [ReadOnly] [NotReplicated]
- **MovingPrimitivesCount**: `int` [ReadOnly] [NotReplicated]
- **PhysicsReceiveKbps**: `float` [ReadOnly] [NotReplicated]
- **PhysicsSendKbps**: `float` [ReadOnly] [NotReplicated]
- **PhysicsStepTime**: `float` [ReadOnly] [NotReplicated]
- **PhysicsStepTimeMs**: `float` [ReadOnly] [NotReplicated] [Deprecated]
- **PrimitivesCount**: `int` [ReadOnly] [NotReplicated]
- **RenderCPUFrameTime**: `float` [ReadOnly] [NotReplicated]
- **RenderGPUFrameTime**: `float` [ReadOnly] [NotReplicated]
- **SceneDrawcallCount**: `int` [ReadOnly] [NotReplicated]
- **SceneTriangleCount**: `int` [ReadOnly] [NotReplicated]
- **ShadowsDrawcallCount**: `int` [ReadOnly] [NotReplicated]
- **ShadowsTriangleCount**: `int` [ReadOnly] [NotReplicated]
- **UI2DDrawcallCount**: `int` [ReadOnly] [NotReplicated]
- **UI2DTriangleCount**: `int` [ReadOnly] [NotReplicated]
- **UI3DDrawcallCount**: `int` [ReadOnly] [NotReplicated]
- **UI3DTriangleCount**: `int` [ReadOnly] [NotReplicated]

## Methods

- **GetBrowserTrackerId**() -> `string`
- **GetHarmonyQualityLevel**() -> `int`
- **GetMemoryCategoryNames**() -> `Array`
- **GetMemoryUsageMbAllCategories**() -> `Array`
- **GetMemoryUsageMbForTag**(`tag: DeveloperMemoryTag`) -> `float`
- **GetPaginatedMemoryByTexture**(`queryType: TextureQueryType`, `pageIndex: int`, `pageSize: int`) -> `Dictionary` [Yields]
- **GetTotalMemoryUsageMb**() -> `float`
- **ResetHarmonyMemoryTarget**() -> `null`
- **SetHarmonyMemoryTarget**(`targetMB: int`) -> `null`
