---
title: StarterPack
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# StarterPack

A container whose contents are copied into each player's `Class.Backpack` when
their player character spawns. It is generally used to hold
`Class.Tool|Tools`.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

`StarterPack` is a service-level container whose contents are copied into each
player's `Class.Backpack` when their player character spawns. It is generally
used to hold `Class.Tool|Tools` but it can also hold
`Class.LocalScript|LocalScripts` to ensure that each player gets a copy.

To ensure that certain `Class.Tool|Tools` are available to specific players
instead of **all** players (`StarterPack`), use player‑specific
`Class.StarterGear` containers or parent those `Class.Tool|Tools` directly to
player `Class.Backpack|Backpacks`.
