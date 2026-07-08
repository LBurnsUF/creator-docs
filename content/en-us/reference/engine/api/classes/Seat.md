---
title: Seat
type: class
superclass: Part
---

# Seat

A type of `Class.BasePart` that characters can 'sit' in. When a character
touches an enabled Seat object, it will be attached to the part by a
`Class.Weld` and the default character scripts will play a sitting animation.

**Inherits from:** `Class.Part` > `Class.FormFactorPart` > `Class.BasePart` > `Class.PVInstance` > `Class.Instance` > `Class.Object`

## Description

A type of `Class.BasePart` that a player character can 'sit' in. When a
character touches an enabled Seat object, it will be attached to the part by a
`Class.Weld` and the default character scripts will play a sitting animation.

## How do Seats work?

When a model containing a `Class.Humanoid` and a `Class.BasePart` called
'HumanoidRootPart' (generally a player character) touches a seat, a
`Class.Weld` is created between the seat and the part. The
`Class.JointInstance.C0|C0` and `Class.JointInstance.C1|C1` properties are
configured so that the character is welded 2 studs above the seat. This weld
is named 'SeatWeld' and parented to the seat.

When sitting the `Class.Seat.Occupant` property is set to the `Class.Humanoid`
that is 'sitting' in the seat. Furthermore the `Class.Humanoid.SeatPart`
property of the humanoid is set to the seat.

A character can also be forced to sit in a seat using the `Class.Seat:Sit()`
function.

There are two ways for a character to get out of a seat. When a player jumps,
they are removed from the seat. However this can also be done manually by
destroying the seat weld, for example:

    seat:FindFirstChild("SeatWeld"):Destroy()

Note seats have a cooldown (currently 3 seconds) that is on a per-character
per-seat basis. This means once a character has gotten out of a seat they
cannot sit back on the same seat for 3 seconds. This cooldown behavior may
change and should not be relied upon by developers.

## What can Seats be used for?

Seats have a diverse range of uses, ranging from the obvious to the more
unconventional.

- Creating chairs or benches without the need for any programming
- Allowing characters to 'sit' in moving objects such as vehicles without
  getting flung around
- Creating interfaces that are controlled by the character in the seat using
  the `Class.Seat.Occupant` property

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Seat.Disabled` | `bool` |  |
| `Class.Seat.Occupant` | `Class.Humanoid` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.Seat:Sit`

``Sit(humanoid: `Class.Instance`)`` -> `null`
