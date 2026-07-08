---
title: Platform
type: class
superclass: Part
tags: [NotCreatable]
---

# Platform

Historically a form of `Class.Seat` that wouldn't place the player in a
sitting pose. This object is no longer create-able and cannot be used by
developers.

**Inherits from:** `Class.Part` > `Class.FormFactorPart` > `Class.BasePart` > `Class.PVInstance` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

The Platform object creates a brick that when touched by a `Class.Player` will
anchor their torso to the brick. This allows for the creation of vehicles that
players can stand in and not be flung about the cabin/deck of the vehicle.

The Platform is almost identical to the `Class.Seat` object, except that
instead of sitting down the player will be standing while locked in place.
Good for ships.

The Platform object is very useful for making people's characters staying in
one spot while they move around, such as a ship or truck. When a player
touches the Platform a `Class.Weld` constraint is created, so they are
'attached' to the Platform and can't move until that weld is broken. It can be
removed by hitting the spacebar, when the player jumps to exit the Platform.

> **Deprecated:** Historically a form of `Class.Seat` that wouldn't place the player in a
sitting pose. This object is no longer create-able and cannot be used by
developers.
