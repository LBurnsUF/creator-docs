---
title: Path
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# Path

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.Path.Status` | `Enum.PathStatus` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.Path:CheckOcclusionAsync`

``CheckOcclusionAsync(start: `int`)`` → `int`
  [Yields]

### `Class.Path:ComputeAsync`

``ComputeAsync(start: `Datatype.Vector3`, finish: `Datatype.Vector3`)`` → `null`
  [Yields]

### `Class.Path:GetPointCoordinates`

``GetPointCoordinates()`` → `Array`
  [Deprecated]

### `Class.Path:GetWaypoints`

``GetWaypoints()`` → `Array`

## Events

### `Class.Path.Blocked`

Fires with: (blockedWaypointIdx: `int`)

### `Class.Path.Unblocked`

Fires with: (unblockedWaypointIdx: `int`)
