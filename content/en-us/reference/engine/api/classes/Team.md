---
title: Team
type: class
superclass: Instance
---

# Team

The `Class.Team` class represents a faction in a Roblox place. The only valid
parent for a Team is in the `Class.Teams` service.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

The `Class.Team` class represents a faction in a Roblox place. The only valid
parent for a Team is in the `Class.Teams` service. Teams offer a range of
features that are useful to developers that can be divided into two rough
groups:

- Features that work 'out of the box'
- Features developers can program into their game.

**Built-in Team Behavior**

The following functionality of Teams exists by default and does not require
the developer to program any custom behavior.

- When part of a Team, the name above a player's character `Class.Model` will
  be colored to the `Class.Team.TeamColor`
- Changing `Class.Player.TeamColor` will cause `Class.Player.Team` to switch
  to the Team with the corresponding `Class.Team.TeamColor`
- When using the default player list users will be grouped and displayed
  together as a team
- Setting `Class.Player.Neutral` to true will cause the `Class.Player` to be
  disassociated with the team, but it will not change `Class.Player.Team` or
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

**Optional Extended Team Behaviors**

Many developers chose to add the following features to teams in their own
code.

- Implement checks in weapon code to prevent friendly fire.
- Implement checks in doors or other features that allow only certain teams to
  use them
- Periodically reassign teams to maintain team balance

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Team.AutoAssignable` | `bool` |  |
| `Class.Team.AutoColorCharacters` | `bool` | [NotReplicated] [Deprecated] |
| `Class.Team.ChildOrder` | `int` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.Team.Score` | `int` | [NotReplicated] [Deprecated] |
| `Class.Team.TeamColor` | `Datatype.BrickColor` |  |

## Methods

### `Class.Team:GetPlayers`

``GetPlayers()`` -> `Datatype.Instances`

## Events

### `Class.Team.PlayerAdded`

Fires with: (player: `Class.Player`)

### `Class.Team.PlayerRemoved`

Fires with: (player: `Class.Player`)
