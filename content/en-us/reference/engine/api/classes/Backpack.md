---
title: Backpack
type: class
superclass: Instance
---

# Backpack

A container object that holds a player's inventory. Any `Class.Tool` in a
player's `Backpack` will be displayed in their inventory at the bottom of the
screen.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`Class.Tool` objects in the `Backpack` container make up the player's
inventory and display as icon buttons at the bottom of the screen. See
[in‑game tools](../../../players/tools.md) for more information.

When a player's character spawns, the contents of `Class.StarterPack` and the
player's `Class.StarterGear` clone to `Backpack`. When the character dies, the
client destroys the `Backpack` and replaces it with a new one, populated again
with the contents of `Class.StarterPack` and `Class.StarterGear`.

To disable the default Roblox inventory GUI and replace it with your own, call
`Class.StarterGui:SetCoreGuiEnabled()` in a `Class.LocalScript` as outlined in
[disable&nbsp;default&nbsp;UI](../../../players/disable-ui.md).

`Backpack` can be accessed from both the client and the server:

```lua
local Players = game:GetService("Players")

-- Accessing Backpack from a server script
local backpack = Players.PlayerName.Backpack

-- Accessing Backpack from a client script
local backpack = Players.LocalPlayer.Backpack
```
