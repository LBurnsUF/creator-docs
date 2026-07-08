---
title: SpawnLocation
type: class
superclass: Part
---

# SpawnLocation

`Class.SpawnLocation|SpawnLocations`, or "spawns" determine where a
`Class.Player` respawns when they die. They can be configured to allow only
certain players to use each spawn, using `Class.Team|Teams`. They also control
how `Class.ForceField|ForceFields` are set up for newly-spawned players.

**Inherits from:** `Class.Part` > `Class.FormFactorPart` > `Class.BasePart` > `Class.PVInstance` > `Class.Instance` > `Class.Object`

## Description

SpawnLocations, or "spawns" determine where a `Class.Player` respawns when
they die. They can be configured to allow only certain players to use each
spawn, using `Class.Team|Teams`. They also control how
`Class.ForceField|ForceFields` are set up for newly-spawned players.

SpawnLocations can be used as checkpoints, such as in an obstacle course,
using the `Class.SpawnLocation.AllowTeamChangeOnTouch` property, so that when
a player touches it, they will change teams to the SpawnLocation's team. In
this case, only the first `Class.Team` should have `Class.Team.AutoAssignable`
set to true, else players will not start at the first checkpoint.

Note if a SpawnLocation is added to the `Class.Workspace` in Studio with
`Class.SpawnLocation.Neutral` set to false a Team will be created
corresponding to `Class.SpawnLocation.TeamColor` if it does not already exist.
This behavior does not occur when spawns are created in-game using a
`Class.Script` or if the properties of the SpawnLocation are changed after
already being added. It is recommended that developers always set up their
teams manually and not rely on this behavior.

## Spawning Rules

There are several rules that come into play for a given SpawnLocation when a
player respawns:

- When `Class.SpawnLocation.Neutral` is set to false only
  `Class.Player|Players` with `Class.Player.TeamColor` matching
  `Class.SpawnLocation.TeamColor` will respawn above it
- When `Class.SpawnLocation.Neutral` is set to true any Player can spawn above
  it regardless of `Class.SpawnLocation.TeamColor`
- If multiple eligible spawns are available to a `Class.Player`, a random one
  will be chosen
- Players will spawn at different points on top of a SpawnLocation, but
  currently, they may still spawn on top of each other if they spawn right
  after one and other

See also:

- If you'd like to configure how long it takes for a player to respawn, take a
  look at the `Class.Players.RespawnTime|RespawnTime` property

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.SpawnLocation.AllowTeamChangeOnTouch` | `bool` |  |
| `Class.SpawnLocation.Duration` | `int` |  |
| `Class.SpawnLocation.Enabled` | `bool` |  |
| `Class.SpawnLocation.Neutral` | `bool` |  |
| `Class.SpawnLocation.TeamColor` | `Datatype.BrickColor` |  |
