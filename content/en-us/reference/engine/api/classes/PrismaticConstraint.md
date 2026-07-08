---
title: PrismaticConstraint
type: class
superclass: SlidingBallConstraint
---

# PrismaticConstraint

Constraint which creates a rigid joint between two
`Class.Attachment|Attachments`, allowing them to slide along one axis but not
rotate.

**Inherits from:** `Class.SlidingBallConstraint` > `Class.Constraint` > `Class.Instance` > `Class.Object`

## Description

A **PrismaticConstraint** creates a rigid joint between two
`Class.Attachment|Attachments`, allowing them to slide along one axis but not
rotate. This constrains the attachments so that their **X** axes are collinear
but pointing in opposite directions. It also constrains the attachments so
that their **Y** axes are parallel.

This constraint inherits many properties from `Class.SlidingBallConstraint`
including `Class.SlidingBallConstraint.ActuatorType|ActuatorType`,
`Class.SlidingBallConstraint.LimitsEnabled|LimitsEnabled`,
`Class.SlidingBallConstraint.Velocity|Velocity`, and more. Please refer to
`Class.SlidingBallConstraint` for details on configuring a
`Class.PrismaticConstraint`.

When configuring this constraint, it may be helpful to study
[Roblox Units](../../../physics/units.md) to understand how Roblox units
compare to metric units.
