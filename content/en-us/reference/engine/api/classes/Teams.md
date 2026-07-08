---
title: Teams
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# Teams

The Teams service holds a game's `Class.Team` objects. `Class.Team` objects
must be parented to the Teams service.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

The Teams service holds a game's `Class.Team` objects. `Class.Team` objects
must be parented to the Teams service.

Teams offer a range of features that are useful to developers. These can
broadly be divided into features that work out-of-the-box and features
developers can program into their game.

**Built-in team behavior** The following functionality of Teams exists by
default and does not require the developer to program any custom behavior.

- When part of a Team, the name above a player's character `Class.Model` will
  be colored to the `Class.Team.TeamColor`
- Changing `Class.Player.TeamColor` will cause `Class.Player.Team` switch to
  the Team with the corresponding `Class.Team.TeamColor`
- When using the default player list users will be grouped and displayed by
  team
- Setting `Class.Player.Neutral` to true will cause the `Class.Player` to be
  dis-associated with the team, but will not change `Class.Player.Team` or
  `Class.Player.TeamColor`
- When a `Class.Player` joins a game, they will be allocated to the team with
  `Class.Team.AutoAssignable` set to true that has the fewest players. If no
  auto assignable team is available, `Class.Player.Neutral` will be set to
  true
- When `Class.SpawnLocation.Neutral` is set to false, only players whose
  `Class.Player.TeamColor` matches `Class.SpawnLocation.TeamColor` can spawn
  on that `Class.SpawnLocation`
- When `Class.SpawnLocation.AllowTeamChangeOnTouch` is set to true, a player's
  `Class.Player.TeamColor` will change to `Class.SpawnLocation.TeamColor` when
  their character touches the `Class.SpawnLocation`

**Optional extended team behavior** Many developers chose to add the following
features to teams in their own code.

- Implement checks for team in weapon code to prevent team killing
- Implement doors or other features that only certain teams can use
- Periodically reassign teams to maintain team balance

## Methods

### `Class.Teams:GetTeams`

``GetTeams()`` -> `Datatype.Instances`

### `Class.Teams:RebalanceTeams`

``RebalanceTeams()`` -> `null`
  [Deprecated]
