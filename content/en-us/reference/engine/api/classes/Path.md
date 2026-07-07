---
title: Path
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# Path

**Inherits**: Instance > Object

**Tags**: NotCreatable, NotReplicated

## Properties

- **Status**: `PathStatus` [ReadOnly] [NotReplicated]

## Methods

- **CheckOcclusionAsync**(`start: int`) -> `int` [Yields]
- **ComputeAsync**(`start: Vector3`, `finish: Vector3`) -> `null` [Yields]
- **GetPointCoordinates**() -> `Array` [Deprecated]
- **GetWaypoints**() -> `Array`

## Events

- **Blocked**(`blockedWaypointIdx: int`)
- **Unblocked**(`unblockedWaypointIdx: int`)
