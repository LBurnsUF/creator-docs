---
title: Explosion
type: class
superclass: Instance
---

# Explosion

Applies force to `Class.BasePart|BaseParts` within the explosion's
`Class.Explosion.BlastRadius`. Breaks `Class.JointInstance|JointInstances` and
`Class.WeldConstraint|WeldConstraints` between parts and kills
`Class.Humanoid` characters not protected by a `Class.ForceField`.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

An Explosion applies force to `Class.BasePart|BaseParts` within the
explosion's `Class.Explosion.BlastRadius|BlastRadius`. This force breaks
`Class.JointInstance|JointInstances` and
`Class.WeldConstraint|WeldConstraints` between parts and kills
`Class.Humanoid` characters not protected by a `Class.ForceField`.
`Class.Constraint|Constraints` will not be broken by an explosion.

If an `Class.Explosion` is parented anywhere in the data model while the
experience is running, it immediately sets off and, within a few seconds, it
becomes unparented. It is not destroyed with `Class.Instance:Destroy()` in
this case, so connections do not get disconnected and the parent is not
locked. As with all instances, keeping a strong reference an `Class.Explosion`
will prevent it from being garbage collected.

Note that an `Class.Explosion` must be a descendant of `Class.Workspace` for
the explosion visuals to play and the physical/damaging effects to have an
impact.

#### Explosion Effects

`Class.Humanoid|Humanoids` are killed by explosions, as the explosion breaks
the character `Class.Model` neck joint. Parenting a `Class.ForceField` to a
model will protect all of its children from the explosion kill effect.

If you do not want joints between `Class.BasePart|BaseParts` to be broken, or
you want to implement your own formula for damaging
`Class.Humanoid|Humanoids`, it's recommended that you set
`Class.Explosion.DestroyJointRadiusPercent|DestroyJointRadiusPercent` to 0 and
use the `Class.Explosion.Hit|Hit` event to handle the result of the explosion.

Explosions can also be configured to damage `Class.Terrain`, creating craters,
as configured through the `Class.Explosion.ExplosionType|ExplosionType`
property.

Note that the effect of an explosion is **not** disrupted by obstacles,
meaning that parts/terrain shielded behind other parts/terrain will still be
affected.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Explosion.BlastPressure` | `float` |  |
| `Class.Explosion.BlastRadius` | `float` |  |
| `Class.Explosion.DestroyJointRadiusPercent` | `float` |  |
| `Class.Explosion.ExplosionType` | `Enum.ExplosionType` |  |
| `Class.Explosion.LocalTransparencyModifier` | `float` | [Hidden] [NotReplicated] |
| `Class.Explosion.Position` | `Datatype.Vector3` |  |
| `Class.Explosion.TimeScale` | `float` |  |
| `Class.Explosion.Visible` | `bool` |  |

## Events

### `Class.Explosion.Hit`

Fires with: (part: `Class.BasePart`, distance: `float`)
