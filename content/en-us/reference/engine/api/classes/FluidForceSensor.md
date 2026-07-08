---
title: FluidForceSensor
type: class
superclass: SensorBase
---

# FluidForceSensor

A `Class.SensorBase` that outputs `Class.FluidForceSensor.Force|Force`,
`Class.FluidForceSensor.Torque|Torque` and
`Class.FluidForceSensor.CenterOfPressure|CenterOfPressure`.

**Inherits from:** `Class.SensorBase` > `Class.Instance` > `Class.Object`

## Description

`FluidForceSensor` is a `Class.SensorBase` which outputs the results of fluid
force simulation from the last physics frame for the part it is attached to.
The sensor outputs the `Class.FluidForceSensor.Force|Force`,
`Class.FluidForceSensor.Torque|Torque` and
`Class.FluidForceSensor.CenterOfPressure|CenterOfPressure` which were computed
by the fluid force simulation on the last physics frame.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.FluidForceSensor.CenterOfPressure` | `Datatype.Vector3` | [ReadOnly] [NotReplicated] |
| `Class.FluidForceSensor.Force` | `Datatype.Vector3` | [ReadOnly] [NotReplicated] |
| `Class.FluidForceSensor.Torque` | `Datatype.Vector3` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.FluidForceSensor:EvaluateAsync`

``EvaluateAsync(linearVelocity: `Datatype.Vector3`, angularVelocity: `Datatype.Vector3`, cframe: `Datatype.CFrame`)`` -> `Tuple`
  [Yields]
