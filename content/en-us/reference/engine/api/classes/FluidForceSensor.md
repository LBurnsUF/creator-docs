---
title: FluidForceSensor
type: class
superclass: SensorBase
---

# FluidForceSensor

**Inherits from:** `Class.SensorBase` > `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.FluidForceSensor.CenterOfPressure` | `Datatype.Vector3` | [ReadOnly] [NotReplicated] |
| `Class.FluidForceSensor.Force` | `Datatype.Vector3` | [ReadOnly] [NotReplicated] |
| `Class.FluidForceSensor.Torque` | `Datatype.Vector3` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.FluidForceSensor:EvaluateAsync`

``EvaluateAsync(linearVelocity: `Datatype.Vector3`, angularVelocity: `Datatype.Vector3`, cframe: `Datatype.CFrame`)`` → `Tuple`
  [Yields]
