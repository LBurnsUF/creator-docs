---
title: RopeConstraint
type: class
superclass: Constraint
---

# RopeConstraint

Simulates rope dynamics, preventing two attachments from separating further
than a defined length.

**Inherits from:** `Class.Constraint` > `Class.Instance` > `Class.Object`

## Description

A **RopeConstraint** prevents two attachments from separating further than a
defined `Class.RopeConstraint.Length|Length`. The attachments can move closer
together than this length and both can freely rotate. This constraint can also
be powered to behave as a motorized winch.

When configuring this constraint, it may be helpful to study
[Roblox Units](../../../physics/units.md) to understand how Roblox units
compare to metric units.

#### Winch

If a rope's `Class.RopeConstraint.WinchEnabled|WinchEnabled` property is
enabled, it attempts to translate the attachments to a set separation
specified by `Class.RopeConstraint.WinchTarget|WinchTarget`, effectively the
target length of the rope in studs. This translation is controlled by
`Class.RopeConstraint.WinchSpeed|WinchSpeed`,
`Class.RopeConstraint.WinchResponsiveness|WinchResponsiveness`, and
`Class.RopeConstraint.WinchForce|WinchForce`.

Note that `Class.RopeConstraint.WinchSpeed|WinchSpeed` must be a **positive**
value, used to either contract or extend the rope length to
`Class.RopeConstraint.WinchTarget|WinchTarget`. Setting a negative speed will
revert to 0, not reverse the winch servo direction.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.RopeConstraint.CurrentDistance` | `float` | [ReadOnly] [NotReplicated] |
| `Class.RopeConstraint.Length` | `float` |  |
| `Class.RopeConstraint.Restitution` | `float` |  |
| `Class.RopeConstraint.Thickness` | `float` |  |
| `Class.RopeConstraint.WinchEnabled` | `bool` |  |
| `Class.RopeConstraint.WinchForce` | `float` |  |
| `Class.RopeConstraint.WinchResponsiveness` | `float` |  |
| `Class.RopeConstraint.WinchSpeed` | `float` |  |
| `Class.RopeConstraint.WinchTarget` | `float` |  |
