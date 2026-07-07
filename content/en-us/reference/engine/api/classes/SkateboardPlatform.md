---
title: SkateboardPlatform
type: class
superclass: Part
tags: [Deprecated]
---

# SkateboardPlatform

**Inherits**: Part > FormFactorPart > BasePart > PVInstance > Instance > Object

**Tags**: Deprecated

## Properties

- **Controller**: `SkateboardController` [ReadOnly] [NotReplicated]
- **ControllingHumanoid**: `Humanoid` [ReadOnly] [NotReplicated]
- **Steer**: `int`
- **StickyWheels**: `bool`
- **Throttle**: `int`

## Methods

- **ApplySpecificImpulse**(`impulseWorld: Vector3`) -> `null`

## Events

- **Equipped**(`humanoid: Instance`, `skateboardController: Instance`)
- **MoveStateChanged**(`newState: MoveState`, `oldState: MoveState`)
- **Unequipped**(`humanoid: Instance`)
- **equipped**(`humanoid: Instance`, `skateboardController: Instance`) [Deprecated]
- **unequipped**(`humanoid: Instance`) [Deprecated]
