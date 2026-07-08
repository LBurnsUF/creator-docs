---
title: ForceField
type: class
superclass: Instance
---

# ForceField

Protects a `Class.Humanoid` from taking damage dealt through the
`Class.Humanoid:TakeDamage()` method and protects `Class.BasePart|BaseParts`
from having their joints broken due to an `Class.Explosion`.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

A **ForceField** protects a `Class.Humanoid` from taking damage dealt through
the `Class.Humanoid:TakeDamage()` method and protects
`Class.BasePart|BaseParts` from having their joints broken due to an
`Class.Explosion`. A new **ForceField** is created when a character spawns on
a `Class.SpawnLocation` and the `Class.SpawnLocation.Duration` property is
greater than zero.

#### Damage and Joints

A **ForceField** influences the instance it's parented to. When parented to a
`Class.Model`, it protects all of the `Class.BasePart|BaseParts` descending
from that model. If parented to a `Class.BasePart`, the part's joints will
only be protected if both the part and the part it's connected to also contain
a **ForceField**.

**ForceField** only protects `Class.Humanoid|Humanoids` from damage dealt by
the `Class.Humanoid:TakeDamage()` method. Humanoids can still be damaged by
setting `Class.Humanoid.Health` directly. For this reason, it's advised that
you use `Class.Humanoid:TakeDamage()` to assign damage while accounting for
force field protection.

#### Visualization

When `Class.ForceField.Visible` is set to true, a particle effect is created.
A number of rules determine where this effect will be emitted from:

- When parented to a `Class.Model`, if the model includes a `Class.Humanoid`
  named **Humanoid** with `Class.Humanoid.RigType` set to R15, the effect will
  be emitted from the part named **UpperTorso**. Otherwise, the effect will be
  emitted from the part named **Torso**.
- When parented to a `Class.BasePart` the effect will be emitted from the
  part's `Class.BasePart.Position`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ForceField.Visible` | `bool` |  |
