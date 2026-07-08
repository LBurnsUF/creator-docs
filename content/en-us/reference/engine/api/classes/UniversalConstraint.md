---
title: UniversalConstraint
type: class
superclass: Constraint
---

# UniversalConstraint

Ensures two axes on two bodies remain perpendicular.

**Inherits from:** `Class.Constraint` > `Class.Instance` > `Class.Object`

## Description

A **UniversalConstraint** ensures two axes on two bodies remain perpendicular.
Contextually, this constraint is more restrictive than a
`Class.BallSocketConstraint` but less restrictive than a
`Class.HingeConstraint` by one degree of freedom.

Example applications of this constraint include transmitting power between the
transmission and drive shafts of cars, robotics, and more.

When configuring this constraint, it may be helpful to study
[Roblox Units](../../../physics/units.md) to understand how Roblox units
compare to metric units.

#### Limits

Enabling the `Class.UniversalConstraint.LimitsEnabled|LimitsEnabled` property
exposes the `Class.UniversalConstraint.MaxAngle|MaxAngle` limit to restrict
tilt within a cone, as well as
`Class.UniversalConstraint.Restitution|Restitution` which defines the
elasticity of the attachments when they reach the limit.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.UniversalConstraint.LimitsEnabled` | `bool` |  |
| `Class.UniversalConstraint.MaxAngle` | `float` |  |
| `Class.UniversalConstraint.Radius` | `float` |  |
| `Class.UniversalConstraint.Restitution` | `float` |  |
