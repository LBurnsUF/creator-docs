---
title: VelocityMotor
type: class
superclass: JointInstance
---

# VelocityMotor

**Inherits from:** `Class.JointInstance` > `Class.Instance` > `Class.Object`

## Description

The VelocityMotor is a special type of joint that works similarly to a
`Class.Motor`, but it uses a `Class.MotorFeature` and a `Class.Hole` to create
the connection. In order for this object to work correctly:

- The VelocityMotor must be parented inside of a `Class.MotorFeature`
- The `Class.MotorFeature` needs to be parented inside of a `Class.BasePart`
- A `Class.Hole` needs to be parented inside of another `Class.BasePart`
- The VelocityMotor's `Class.VelocityMotor.Hole` property should be assigned
  to the hole you parented inside of the other part.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.VelocityMotor.CurrentAngle` | `float` |  |
| `Class.VelocityMotor.DesiredAngle` | `float` |  |
| `Class.VelocityMotor.Hole` | `Class.Hole` |  |
| `Class.VelocityMotor.MaxVelocity` | `float` |  |
