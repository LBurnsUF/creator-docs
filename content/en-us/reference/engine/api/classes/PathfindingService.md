---
title: PathfindingService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# PathfindingService

Used to find logical paths between two points.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

`PathfindingService` is used to find logical paths between two points,
ensuring that characters can move between the points without running into
walls or other obstacles. By default, the shortest path is calculated, but you
can implement pathfinding modifiers to compute smarter paths across various
materials, around defined regions, or through obstacles.

See [Pathfinding](../../../characters/pathfinding.md) for details on
implementing character pathfinding.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.PathfindingService.EmptyCutoff` | `float` | [NotReplicated] [Deprecated] |

## Methods

### `Class.PathfindingService:ComputeRawPathAsync`

``ComputeRawPathAsync(start: `Datatype.Vector3`, finish: `Datatype.Vector3`, maxDistance: `float`)`` -> `Class.Path`
  [Yields] [Deprecated]

### `Class.PathfindingService:ComputeSmoothPathAsync`

``ComputeSmoothPathAsync(start: `Datatype.Vector3`, finish: `Datatype.Vector3`, maxDistance: `float`)`` -> `Class.Path`
  [Yields] [Deprecated]

### `Class.PathfindingService:CreatePath`

``CreatePath(agentParameters: `Dictionary`)`` -> `Class.Path`

### `Class.PathfindingService:FindPathAsync`

``FindPathAsync(start: `Datatype.Vector3`, finish: `Datatype.Vector3`)`` -> `Class.Path`
  [Yields]
