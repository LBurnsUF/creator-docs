---
title: TouchTransmitter
type: class
superclass: Instance
tags: [NotCreatable, NotBrowsable]
---

# TouchTransmitter

An internal object used by networking and replication code to transmit
`Class.BasePart.Touched` and `Class.BasePart.TouchEnded` events.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotBrowsable]

## Description

An internal object used by networking and replication code to transmit
`Class.BasePart.Touched` and `Class.BasePart.TouchEnded` events.

The TouchTransmitter object named 'TouchInterest' is created and parented to a
`Class.BasePart` when the `Class.BasePart.Touched` or
`Class.BasePart.TouchEnded` events are listened (connected) to.

Removing the TouchTransmitter will prevent the touched events from working.
The TouchTransmitter object can also be removed exclusively on the client.
This will prevent collisions from models the client has network ownership of
(such as the player's character) from registering.

Note, in almost all circumstances developers should disconnect the connection
using `Datatype.RBXScriptConnection:Disconnect()` method rather than removing
the TouchTransmitter. Otherwise the connection will not be cleaned up which
can cause performance issues over time.
