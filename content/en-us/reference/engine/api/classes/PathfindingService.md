---
title: PathfindingService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# PathfindingService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.PathfindingService.EmptyCutoff` | `float` | [NotReplicated] [Deprecated] |

## Methods

### `Class.PathfindingService:ComputeRawPathAsync`

``ComputeRawPathAsync(start: `Datatype.Vector3`, finish: `Datatype.Vector3`, maxDistance: `float`)`` → `Class.Path`
  [Yields] [Deprecated]

### `Class.PathfindingService:ComputeSmoothPathAsync`

``ComputeSmoothPathAsync(start: `Datatype.Vector3`, finish: `Datatype.Vector3`, maxDistance: `float`)`` → `Class.Path`
  [Yields] [Deprecated]

### `Class.PathfindingService:CreatePath`

``CreatePath(agentParameters: `Dictionary`)`` → `Class.Path`

### `Class.PathfindingService:FindPathAsync`

``FindPathAsync(start: `Datatype.Vector3`, finish: `Datatype.Vector3`)`` → `Class.Path`
  [Yields]
