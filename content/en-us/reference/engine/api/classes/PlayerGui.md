---
title: PlayerGui
type: class
superclass: BasePlayerGui
tags: [NotCreatable, PlayerReplicated]
---

# PlayerGui

A container that holds a player's UI.

**Inherits from:** `Class.BasePlayerGui` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [PlayerReplicated]

## Description

The `PlayerGui` container stores objects that create the player's GUI. If a
`Class.ScreenGui` is a descendant of `PlayerGui`, any `Class.GuiObject` inside
that `Class.ScreenGui` displays on the player's screen. Any
`Class.LocalScript` will also run if it is inserted into a `PlayerGui`.

When a player first joins the experience, their `PlayerGui` is automatically
inserted into their `Class.Player` object. When the player's
`Class.Player.Character` spawns for the first time, all of the contents of
`Class.StarterGui` are automatically copied into the player's `PlayerGui`. If
`Class.StarterGui.ResetPlayerGuiOnSpawn` is set to `true`, all the contents of
a player's `PlayerGui` are cleared and replaced with the contents of
`Class.StarterGui` every time the player's character respawns.

Note that if `Class.Players.CharacterAutoLoads` is set to `false`, the
character won't spawn and `Class.StarterGui` contents won't copy over until
`Class.Player:LoadCharacterAsync()` is called.

If you need to control a player's UI container during playtime, for example to
show/hide a specific `Class.ScreenGui` or any of its children, access it as
follows from a `Class.LocalScript`:

```lua
local Players = game:GetService("Players")

local player = Players.LocalPlayer
local playerGui = player.PlayerGui
```

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.PlayerGui.CurrentScreenOrientation` | `Enum.ScreenOrientation` | [ReadOnly] [NotReplicated] |
| `Class.PlayerGui.ScreenOrientation` | `Enum.ScreenOrientation` |  |
| `Class.PlayerGui.SelectionImageObject` | `Class.GuiObject` |  |

## Methods

### `Class.PlayerGui:GetTopbarTransparency`

``GetTopbarTransparency()`` -> `float`
  [Deprecated]

### `Class.PlayerGui:SetTopbarTransparency`

``SetTopbarTransparency(transparency: `float`)`` -> `null`
  [Deprecated]

## Events

### `Class.PlayerGui.TopbarTransparencyChangedSignal`

Fires with: (transparency: `float`)
  [Deprecated]
