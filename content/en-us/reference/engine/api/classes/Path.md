---
title: Path
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# Path

Stores the result of paths created by `Class.PathfindingService:CreatePath()`.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

`Path` objects store the result of paths created by
`Class.PathfindingService:CreatePath()`.

Once a `Path` object is created, you can call
`Class.Path:ComputeAsync()|ComputeAsync()` with a starting point and ending
point. This will attempt to compute a valid path for a character to move
along, based on default or custom parameters passed to
`Class.PathfindingService:CreatePath()|CreatePath()`. If
`Class.Path:ComputeAsync()|ComputeAsync()` successfully finds a path, the
`Path` object will have a `Class.Path.Status|Status` value of
`Enum.PathStatus.Success`. Otherwise the status will be
`Enum.PathStatus.NoPath` which can occur if there are obstacles between the
two points (and no way around) or if the points are inside of solid objects.

In addition to `Class.Path:ComputeAsync()|ComputeAsync()`, `Path` objects have
the `Class.Path:GetWaypoints()|GetWaypoints()` method which returns a list of
waypoints representing the points a character should follow in sequence to get
from the beginning to the end of the path.

Finally, `Path` objects can be **connected** to the
`Class.Path.Blocked|Blocked` event which will fire if, at any time during the
path's existence, the path is blocked. Note that this can occur **behind** a
character moving along the path, not just in front of it.

See [Pathfinding](../../../characters/pathfinding.md) for details on
implementing character pathfinding.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Path.Status` | `Enum.PathStatus` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.Path:CheckOcclusionAsync`

``CheckOcclusionAsync(start: `int`)`` -> `int`
  [Yields]

### `Class.Path:ComputeAsync`

``ComputeAsync(start: `Datatype.Vector3`, finish: `Datatype.Vector3`)`` -> `null`
  [Yields]

### `Class.Path:GetPointCoordinates`

``GetPointCoordinates()`` -> `Array`
  [Deprecated]

### `Class.Path:GetWaypoints`

``GetWaypoints()`` -> `Array`

## Events

### `Class.Path.Blocked`

Fires with: (blockedWaypointIdx: `int`)

### `Class.Path.Unblocked`

Fires with: (unblockedWaypointIdx: `int`)
