---
title: SkateboardPlatform
type: class
superclass: Part
tags: [Deprecated]
---

# SkateboardPlatform

**Inherits from:** `Class.Part` > `Class.FormFactorPart` > `Class.BasePart` > `Class.PVInstance` > `Class.Instance` > `Class.Object`

**Tags:** [Deprecated]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.SkateboardPlatform.Controller` | `Class.SkateboardController` | [ReadOnly] [NotReplicated] |
| `Class.SkateboardPlatform.ControllingHumanoid` | `Class.Humanoid` | [ReadOnly] [NotReplicated] |
| `Class.SkateboardPlatform.Steer` | `int` |  |
| `Class.SkateboardPlatform.StickyWheels` | `bool` |  |
| `Class.SkateboardPlatform.Throttle` | `int` |  |

## Methods

### `Class.SkateboardPlatform:ApplySpecificImpulse`

``ApplySpecificImpulse(impulseWorld: `Datatype.Vector3`)`` → `null`

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
