---
title: PathfindingModifier
type: class
superclass: Instance
---

# PathfindingModifier

Modifiers used to represent space that has a higher or lower cost to be
traversed when creating paths using `Class.PathfindingService`.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

Pathfinding modifiers can be used to represent space that has a higher or
lower cost to be traversed. You can include pathfinding modifiers in the
`Class.PathfindingService:CreatePath()` parameters and compute smarter paths
across various materials or around defined regions. See
[Pathfinding](../../../characters/pathfinding.md#pathfinding-modifiers) for
details.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.PathfindingModifier.Label` | `string` |  |
| `Class.PathfindingModifier.PassThrough` | `bool` |  |
