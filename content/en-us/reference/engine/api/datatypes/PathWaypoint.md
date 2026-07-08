---
title: PathWaypoint
type: datatype
---

# `Datatype.PathWaypoint`

A description of the steps required to reach the next waypoint in a path.

## Description

The `PathWaypoint` data type is constructed by a `Enum.PathWaypointAction`
action, `Datatype.Vector3` position, and `Library.string` label which is used
by the `Class.PathfindingService` to create points along a generated path.

## Constructors

### `PathWaypoint.new`

Returns a `Datatype.PathWaypoint` object from the given `Datatype.Vector3` position, `Enum.PathWaypointAction` action, and optional string label.

**Parameters:**

- `position`: `Vector3` - The 3D position of the waypoint.
- `action`: `PathWaypointAction` - The action to perform at the waypoint.
- `label`: `string` - The name of the navigation area that generates the waypoint.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `PathWaypoint.Action` | `PathWaypointAction` | The action to perform at this waypoint. |
| `PathWaypoint.Position` | `Vector3` | The 3D position of this waypoint. |
| `PathWaypoint.Label` | `string` | The name of the navigation area that generates this waypoint. |
