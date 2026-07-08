---
title: Flag
type: class
superclass: Tool
tags: [Deprecated]
---

# Flag

The Flag object helps you make 'capture the flag' style games.

**Inherits from:** `Class.Tool` > `Class.BackpackItem` > `Class.Model` > `Class.PVInstance` > `Class.Instance` > `Class.Object`

**Tags:** [Deprecated]

## Description

The Flag is a unit spawned with a `Class.FlagStand` object, and will respawn
when captured. When a player touches this object's Handle, which must be a
child of the Flag object, which is a Part named "Handle", the flag will be
added to the player's backpack and will appear in their hand. A player cannot
select other weapons while carrying a flag, and can drop the flag at anytime
by pressing "Backspace" on the keyboard. If the player carrying a flag steps
onto another FlagStand of a different team color, the flag will be removed
from the player's backpack and a point will be added to the user's
leaderstats, if provided. The flag will then regenerate at the originating
flag stand.

> **Deprecated:** The `Class.Flag` and `Class.FlagStand` objects were created to allow
developers to make 'capture the flag' style games quickly. However they have
been deprecated and developers are advised to design their own systems which
will be more flexible and reliable.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Flag.TeamColor` | `Datatype.BrickColor` |  |
