---
title: ControllerPartSensor
type: class
superclass: ControllerSensor
---

# ControllerPartSensor

A `Class.SensorBase` that outputs data about another `Class.BasePart` based on
`Class.Humanoid` floor and ladder detection logic.

**Inherits from:** `Class.ControllerSensor` > `Class.SensorBase` > `Class.Instance` > `Class.Object`

## Description

A `Class.SensorBase` that outputs data about another `Class.BasePart` based on
`Class.Humanoid` floor and ladder detection logic. It is primarily used for
sending data to a character controller. Using a `Class.ControllerPartSensor`
allows you to detect `Class.BasePart|BaseParts` in the same manner as the
`Class.Humanoid` uses for detecting floors and ladders.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ControllerPartSensor.HitFrame` | `Datatype.CFrame` |  |
| `Class.ControllerPartSensor.HitNormal` | `Datatype.Vector3` |  |
| `Class.ControllerPartSensor.LadderSearchHeight` | `float` |  |
| `Class.ControllerPartSensor.LadderSearchOffset` | `float` |  |
| `Class.ControllerPartSensor.SearchDistance` | `float` |  |
| `Class.ControllerPartSensor.SensedMaterial` | `Enum.Material` |  |
| `Class.ControllerPartSensor.SensedPart` | `Class.BasePart` |  |
| `Class.ControllerPartSensor.SensorMode` | `Enum.SensorMode` |  |
