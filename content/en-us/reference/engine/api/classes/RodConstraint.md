---
title: RodConstraint
type: class
superclass: Constraint
---

# RodConstraint

Keeps two attachments separated by its defined
`Class.RodConstraint.Length|Length`.

**Inherits from:** `Class.Constraint` > `Class.Instance` > `Class.Object`

## Description

A **RodConstraint** keeps two attachments separated by its defined
`Class.RodConstraint.Length|Length`. By default, both attachments can rotate
freely, although you can enable limits to restrict rotational tilt.

Note that if this constraint attaches one part (**A**) to another part (**B**)
that is anchored or connected to an anchored part (**Z**), part **A** will not
be locally simulated when interacting with a player.

#### Limits

You can limit rotation of the attachments within a cone, independently of each
other, by enabling the `Class.RodConstraint.LimitsEnabled|LimitsEnabled`
property and setting `Class.RodConstraint.LimitAngle0|LimitAngle0` and
`Class.RodConstraint.LimitAngle1|LimitAngle1` respectively.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.RodConstraint.CurrentDistance` | `float` | [ReadOnly] [NotReplicated] |
| `Class.RodConstraint.Length` | `float` |  |
| `Class.RodConstraint.LimitAngle0` | `float` |  |
| `Class.RodConstraint.LimitAngle1` | `float` |  |
| `Class.RodConstraint.LimitsEnabled` | `bool` |  |
| `Class.RodConstraint.Thickness` | `float` |  |
