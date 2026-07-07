---
title: PathfindingService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# PathfindingService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Properties

- **EmptyCutoff**: `float` [NotReplicated] [Deprecated]

## Methods

- **ComputeRawPathAsync**(`start: Vector3`, `finish: Vector3`, `maxDistance: float`) -> `Path` [Yields] [Deprecated]
- **ComputeSmoothPathAsync**(`start: Vector3`, `finish: Vector3`, `maxDistance: float`) -> `Path` [Yields] [Deprecated]
- **CreatePath**(`agentParameters: Dictionary = nil`) -> `Path`
- **FindPathAsync**(`start: Vector3`, `finish: Vector3`) -> `Path` [Yields]
