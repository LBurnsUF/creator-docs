---
title: Stats
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# Stats

Performance metrics for a game.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

`Class.Stats` is a service that provides real-time performance information
about the current running game instance. Its primary purpose is to provide an
end point to measure where resources are being consumed, as well as how much
memory is being consumed overall.

The service also stores a tree of `Class.StatsItem` objects which can have
their values read by plugins.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Stats.ContactsCount` | `int` | [ReadOnly] [NotReplicated] |
| `Class.Stats.DataReceiveKbps` | `float` | [ReadOnly] [NotReplicated] |
| `Class.Stats.DataSendKbps` | `float` | [ReadOnly] [NotReplicated] |
| `Class.Stats.FrameTime` | `float` | [ReadOnly] [NotReplicated] |
| `Class.Stats.HeartbeatTime` | `float` | [ReadOnly] [NotReplicated] |
| `Class.Stats.HeartbeatTimeMs` | `float` | [ReadOnly] [NotReplicated] [Deprecated] |
| `Class.Stats.InstanceCount` | `int` | [ReadOnly] [NotReplicated] |
| `Class.Stats.MemoryTrackingEnabled` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.Stats.MovingPrimitivesCount` | `int` | [ReadOnly] [NotReplicated] |
| `Class.Stats.PhysicsReceiveKbps` | `float` | [ReadOnly] [NotReplicated] |
| `Class.Stats.PhysicsSendKbps` | `float` | [ReadOnly] [NotReplicated] |
| `Class.Stats.PhysicsStepTime` | `float` | [ReadOnly] [NotReplicated] |
| `Class.Stats.PhysicsStepTimeMs` | `float` | [ReadOnly] [NotReplicated] [Deprecated] |
| `Class.Stats.PrimitivesCount` | `int` | [ReadOnly] [NotReplicated] |
| `Class.Stats.RenderCPUFrameTime` | `float` | [ReadOnly] [NotReplicated] |
| `Class.Stats.RenderGPUFrameTime` | `float` | [ReadOnly] [NotReplicated] |
| `Class.Stats.SceneDrawcallCount` | `int` | [ReadOnly] [NotReplicated] |
| `Class.Stats.SceneTriangleCount` | `int` | [ReadOnly] [NotReplicated] |
| `Class.Stats.ShadowsDrawcallCount` | `int` | [ReadOnly] [NotReplicated] |
| `Class.Stats.ShadowsTriangleCount` | `int` | [ReadOnly] [NotReplicated] |
| `Class.Stats.UI2DDrawcallCount` | `int` | [ReadOnly] [NotReplicated] |
| `Class.Stats.UI2DTriangleCount` | `int` | [ReadOnly] [NotReplicated] |
| `Class.Stats.UI3DDrawcallCount` | `int` | [ReadOnly] [NotReplicated] |
| `Class.Stats.UI3DTriangleCount` | `int` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.Stats:GetBrowserTrackerId`

``GetBrowserTrackerId()`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.Stats:GetHarmonyQualityLevel`

``GetHarmonyQualityLevel()`` -> `int`

### `Class.Stats:GetMemoryCategoryNames`

``GetMemoryCategoryNames()`` -> `Array`

### `Class.Stats:GetMemoryUsageMbAllCategories`

``GetMemoryUsageMbAllCategories()`` -> `Array`

### `Class.Stats:GetMemoryUsageMbForTag`

``GetMemoryUsageMbForTag(tag: `Enum.DeveloperMemoryTag`)`` -> `float`

### `Class.Stats:GetPaginatedMemoryByTexture`

``GetPaginatedMemoryByTexture(queryType: `Enum.TextureQueryType`, pageIndex: `int`, pageSize: `int`)`` -> `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.Stats:GetTotalMemoryUsageMb`

``GetTotalMemoryUsageMb()`` -> `float`

### `Class.Stats:ResetHarmonyMemoryTarget`

``ResetHarmonyMemoryTarget()`` -> `null`

### `Class.Stats:SetHarmonyMemoryTarget`

``SetHarmonyMemoryTarget(targetMB: `int`)`` -> `null`
