---
title: SkateboardPlatform
type: class
superclass: Part
tags: [Deprecated]
---

# SkateboardPlatform

A SkateboardPlatform can be used to create a skateboard. When characters get
on a skateboard, they are stuck to it until they press the escape key. Until
then, the character uses skateboard animations and travels faster than a
walking character.

**Inherits from:** `Class.Part` > `Class.FormFactorPart` > `Class.BasePart` > `Class.PVInstance` > `Class.Instance` > `Class.Object`

**Tags:** [Deprecated]

## Description

A SkateboardPlatform can be used to create a skateboard. When characters get
on a skateboard, they are stuck to it until they press the escape key. Until
then, the character uses skateboard animations and travels faster than a
walking character.

> **Deprecated:** The SkateboardPlatform object has been deprecated and is no longer supported
by Roblox. Developers looking to create skateboards or similar vehicles are
advised to program their own systems. Additionally, the `Class.VehicleSeat`
object can be used to quickly create simple vehicles.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.SkateboardPlatform.Controller` | `Class.SkateboardController` | [ReadOnly] [NotReplicated] |
| `Class.SkateboardPlatform.ControllingHumanoid` | `Class.Humanoid` | [ReadOnly] [NotReplicated] |
| `Class.SkateboardPlatform.Steer` | `int` |  |
| `Class.SkateboardPlatform.StickyWheels` | `bool` |  |
| `Class.SkateboardPlatform.Throttle` | `int` |  |

## Methods

### `Class.SkateboardPlatform:ApplySpecificImpulse`

``ApplySpecificImpulse(impulseWorld: `Datatype.Vector3`)`` -> `null`

## Events

### `Class.SkateboardPlatform.Equipped`

Fires with: (humanoid: `Class.Instance`, skateboardController: `Class.Instance`)

### `Class.SkateboardPlatform.MoveStateChanged`

Fires with: (newState: `Enum.MoveState`, oldState: `Enum.MoveState`)

### `Class.SkateboardPlatform.Unequipped`

Fires with: (humanoid: `Class.Instance`)

### `Class.SkateboardPlatform.equipped`

Fires with: (humanoid: `Class.Instance`, skateboardController: `Class.Instance`)
  [Deprecated]

### `Class.SkateboardPlatform.unequipped`

Fires with: (humanoid: `Class.Instance`)
  [Deprecated]
