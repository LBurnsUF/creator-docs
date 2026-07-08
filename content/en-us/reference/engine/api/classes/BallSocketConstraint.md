---
title: BallSocketConstraint
type: class
superclass: Constraint
---

# BallSocketConstraint

Forces its two attachments into the same position and allows them to freely
rotate about all three axes, with optional limits to restrict both tilt and
twist.

**Inherits from:** `Class.Constraint` > `Class.Instance` > `Class.Object`

## Description

A `BallSocketConstraint` constrains its `Class.Attachment|Attachments` so that
they occupy the same position. By default it allows both attachments to freely
rotate about all of their axes, but if
`Class.BallSocketConstraint.LimitsEnabled|LimitsEnabled` is `true`, the
attachments can only rotate in a limited cone.

Note that if this constraint attaches one part (**A**) to another part (**B**)
that is anchored or connected to an anchored part (**Z**), part **A** will not
be locally simulated when interacting with a player.

When configuring this constraint, it may be helpful to study
[Roblox Units](../../../physics/units.md) to understand how Roblox units
compare to metric units.

#### Limits

You can set limits to restrict both **tilt** and **twist** of a ball socket,
similar to how a human's head can tilt and turn within a limited axial range.
Enabling the `Class.BallSocketConstraint.LimitsEnabled|LimitsEnabled` property
exposes the `Class.BallSocketConstraint.UpperAngle|UpperAngle` value to
restrict **tilt** within a cone; it also exposes the
`Class.BallSocketConstraint.TwistLimitsEnabled|TwistLimitsEnabled` property
which, when enabled, lets you restrict **twist** rotation through the
`Class.BallSocketConstraint.TwistLowerAngle|TwistLowerAngle` and
`Class.BallSocketConstraint.TwistUpperAngle|TwistUpperAngle` limits.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.BallSocketConstraint.EnableSkinning` | `bool` |  {security: RobloxScriptSecurity} |
| `Class.BallSocketConstraint.LimitsEnabled` | `bool` |  |
| `Class.BallSocketConstraint.MaxFrictionTorque` | `float` |  |
| `Class.BallSocketConstraint.Radius` | `float` |  |
| `Class.BallSocketConstraint.Restitution` | `float` |  |
| `Class.BallSocketConstraint.TwistLimitsEnabled` | `bool` |  |
| `Class.BallSocketConstraint.TwistLowerAngle` | `float` |  |
| `Class.BallSocketConstraint.TwistUpperAngle` | `float` |  |
| `Class.BallSocketConstraint.UpperAngle` | `float` |  |
