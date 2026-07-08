---
title: VehicleSeat
type: class
superclass: BasePart
---

# VehicleSeat

A seat object that can be used to control a vehicle.

**Inherits from:** `Class.BasePart` > `Class.PVInstance` > `Class.Instance` > `Class.Object`

## Description

The `VehicleSeat` objects welds a player to the seat when the player touches
the seat. It then forwards the movement inputs to any connected motor joints,
allowing control of a vehicle.

While `VehicleSeat` is great for making simple vehicles they do have some
limitations. Movement control will only detect motors connected directly to
the vehicle seat, or through another rigid connection. This means that if you
have a wheel connected to a beam which is then welded to the seat it will work
fine, however if you have the wheel connected to a part, which is connected by
a hinge to the rest of the car, it will not work.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.VehicleSeat.AreHingesDetected` | `int` | [ReadOnly] [NotReplicated] |
| `Class.VehicleSeat.Disabled` | `bool` |  |
| `Class.VehicleSeat.HeadsUpDisplay` | `bool` |  |
| `Class.VehicleSeat.MaxSpeed` | `float` |  |
| `Class.VehicleSeat.Occupant` | `Class.Humanoid` | [ReadOnly] [NotReplicated] |
| `Class.VehicleSeat.Steer` | `int` | [NotReplicated] |
| `Class.VehicleSeat.SteerFloat` | `float` |  |
| `Class.VehicleSeat.Throttle` | `int` | [NotReplicated] |
| `Class.VehicleSeat.ThrottleFloat` | `float` |  |
| `Class.VehicleSeat.Torque` | `float` |  |
| `Class.VehicleSeat.TurnSpeed` | `float` |  |

## Methods

### `Class.VehicleSeat:Sit`

``Sit(humanoid: `Class.Instance`)`` -> `null`
