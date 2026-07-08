---
title: SpringConstraint
type: class
superclass: Constraint
---

# SpringConstraint

Simulates spring and damper behavior between two attachments.

**Inherits from:** `Class.Constraint` > `Class.Instance` > `Class.Object`

## Description

A **SpringConstraint** applies a force to its `Class.Attachment|Attachments`
based on spring and damper behavior. This constraint, along with a
`Class.CylindricalConstraint`, is ideal for building vehicle suspension.

Note that if this constraint attaches one part (**A**) to another part (**B**)
that is anchored or connected to an anchored part (**Z**), part **A** will not
be locally simulated when interacting with a player.

When configuring this constraint, it may be helpful to study
[Roblox Units](../../../physics/units.md) to understand how Roblox units
compare to metric units.

#### Free Length

`Class.SpringConstraint.FreeLength|FreeLength` defines the natural resting
length of the spring. If the attachments are further apart than the free
length, they are forced together; if the attachments are closer together than
the free length, they are forced apart.

#### Damping

The `Class.SpringConstraint.Damping|Damping` value controls how fast the
spring's oscillation dies down. A value of 0 allows the spring to oscillate
endlessly, while higher values bring the spring to a rest more quickly.

#### Stiffness

`Class.SpringConstraint.Stiffness|Stiffness` sets the strength of the spring.
Higher values create a spring that responds with more force when its
attachments are closer together or further apart than
`Class.SpringConstraint.FreeLength|FreeLength`.

#### Limits

Enabling the `Class.SpringConstraint.LimitsEnabled|LimitsEnabled` property
exposes the `Class.SpringConstraint.MinLength|MinLength` and
`Class.SpringConstraint.MaxLength|MaxLength` values for setting the minimum
and maximum length of the spring. If the spring's attachments reach these
limits, they stop moving apart from one another without restitution.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.SpringConstraint.Coils` | `float` |  |
| `Class.SpringConstraint.CurrentLength` | `float` | [ReadOnly] [NotReplicated] |
| `Class.SpringConstraint.Damping` | `float` |  |
| `Class.SpringConstraint.FreeLength` | `float` |  |
| `Class.SpringConstraint.LimitsEnabled` | `bool` |  |
| `Class.SpringConstraint.MaxForce` | `float` |  |
| `Class.SpringConstraint.MaxLength` | `float` |  |
| `Class.SpringConstraint.MinLength` | `float` |  |
| `Class.SpringConstraint.Radius` | `float` |  |
| `Class.SpringConstraint.Stiffness` | `float` |  |
| `Class.SpringConstraint.Thickness` | `float` |  |
