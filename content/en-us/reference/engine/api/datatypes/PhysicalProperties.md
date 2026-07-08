---
title: PhysicalProperties
type: datatype
---

# `Datatype.PhysicalProperties`

Describes properties that affect the physical behavior of a `Class.BasePart`.

## Description

The `Datatype.PhysicalProperties` data type describes several physical
properties of a `Class.BasePart`:
`Datatype.PhysicalProperties.Density|Density`,
`Datatype.PhysicalProperties.Elasticity|Elasticity`, and
`Datatype.PhysicalProperties.Friction|Friction`. It is used in the
similarly-named `Class.BasePart.CustomPhysicalProperties` property.

#### Weighting Behavior

`Datatype.PhysicalProperties` also provides weightings properties,
`Datatype.PhysicalProperties.ElasticityWeight|ElasticityWeight` and
`Datatype.PhysicalProperties.FrictionWeight|FrictionWeight`. When two parts
interact, the friction and elasticity between them are determined in the same
way by the following pairwise weighted average function:

```lua
local function getActualFriction(partA, partB)
	return (partA.Friction * partA.FrictionWeight + partB.Friction * partB.FrictionWeight) / (partA.FrictionWeight + partB.FrictionWeight)
end
```

Although the formula above refers to the
`Datatype.PhysicalProperties.Friction|Friction` and
`Datatype.PhysicalProperties.FrictionWeight|FrictionWeight` of two parts,
**A** and **B**, the formula is used in the same manner when determining
`Datatype.PhysicalProperties.Elasticity|Elasticity`. Generally, when the
weight of **A** is much greater than that of **B**, the actual value will be
closer to **A**. If the weights are similar, the actual value will be close to
the midpoint between their individual values.

## Constructors

### `PhysicalProperties.new`

Returns a `Datatype.PhysicalProperties` container, with the density, friction, and elasticity specified for this material.

**Parameters:**

- `material`: `Material`

### `PhysicalProperties.new`

Returns a `Datatype.PhysicalProperties` container, with the specified density,
friction, and elasticity.

**Parameters:**

- `density`: `number`
- `friction`: `number`
- `elasticity`: `number`

### `PhysicalProperties.new`

Creates a `Datatype.PhysicalProperties` container with the specified density,
friction, elasticity, weight of friction, and weight of elasticity.

**Parameters:**

- `density`: `number`
- `friction`: `number`
- `elasticity`: `number`
- `frictionWeight`: `number`
- `elasticityWeight`: `number`

### `PhysicalProperties.new`

Creates a `Datatype.PhysicalProperties` container with the specified density,
friction, elasticity, weight of friction, weight of elasticity, and acoustic absorption.

**Parameters:**

- `density`: `number`
- `friction`: `number`
- `elasticity`: `number`
- `frictionWeight`: `number`
- `elasticityWeight`: `number`
- `acousticAbsorption`: `number`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `PhysicalProperties.AcousticAbsorption` | `number` | A value between `0` and `1` denoting how absorbent the material is to `Class.AudioEmitter/AudioEmitt |
| `PhysicalProperties.Density` | `number` | The mass per unit volume of the part. |
| `PhysicalProperties.Friction` | `number` | The deceleration of the part when rubbing against another part. |
| `PhysicalProperties.Elasticity` | `number` | The amount of energy retained when colliding with another part. |
| `PhysicalProperties.FrictionWeight` | `number` | The importance of the part's `Datatype.PhysicalProperties.Friction/Friction` property when calculati |
| `PhysicalProperties.ElasticityWeight` | `number` | The importance of the part's `Datatype.PhysicalProperties.Elasticity/Elasticity` property when calcu |

## API Usage (3 locations)

### Used as Property Type

- `Class.BasePart.CurrentPhysicalProperties`
- `Class.BasePart.CustomPhysicalProperties`
- `Class.MaterialVariant.CustomPhysicalProperties`
