---
title: LineForce
type: class
superclass: Constraint
---

# LineForce

Applies a force along the theoretical line connecting its two
`Class.Attachment|Attachments`.

**Inherits from:** `Class.Constraint` > `Class.Instance` > `Class.Object`

## Description

The `LineForce` constraint applies a force along the theoretical line
connecting its two `Class.Attachment|Attachments`. As the end points
(attachments) move, the direction of force will change accordingly.

When configuring this constraint, it may be helpful to study
[Roblox Units](../../../physics/units.md) to understand how Roblox units
compare to metric units.

#### Force Location

By default, force is applied to either parent at its attachment location. If
desired, force can be focused at each parent's center of mass by enabling
`Class.LineForce.ApplyAtCenterOfMass|ApplyAtCenterOfMass`.

#### Inverse Square Law

When `Class.LineForce.InverseSquareLaw|InverseSquareLaw` is `true`, the force
magnitude is multiplied by the inverse square of the distance, meaning the
force will increase exponentially as the two attachments get closer together,
like magnets. When using this setting, it's recommended that you set a
`Class.LineForce.MaxForce|MaxForce` threshold to prevent infinite force if the
attachments align precisely.

#### Reactionary Force

By default, the constraint only applies force to
`Class.Constraint.Attachment0|Attachment0`, while
`Class.Constraint.Attachment1|Attachment1` remains unaffected. However, force
can be applied to both attachments in **equal and opposite directions** by
enabling `Class.LineForce.ReactionForceEnabled|ReactionForceEnabled`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.LineForce.ApplyAtCenterOfMass` | `bool` |  |
| `Class.LineForce.InverseSquareLaw` | `bool` |  |
| `Class.LineForce.Magnitude` | `float` |  |
| `Class.LineForce.MaxForce` | `float` |  |
| `Class.LineForce.ReactionForceEnabled` | `bool` |  |
