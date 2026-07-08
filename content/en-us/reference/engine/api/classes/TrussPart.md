---
title: TrussPart
type: class
superclass: BasePart
---

# TrussPart

Similar to a `Class.Part` but with a different visual
`Class.TrussPart.Style|Style` and the important distinction that default
characters are able to climb it.

**Inherits from:** `Class.BasePart` > `Class.PVInstance` > `Class.Instance` > `Class.Object`

## Description

A `TrussPart` is similar to a `Class.Part` but with a different visual
`Class.TrussPart.Style|Style` and the important distinction that default
characters are able to climb it.

This part type has significantly more restrictive size limitations than other
parts; it must be `2*2*n` studs where `n` is a multiple of `2` with a maximum
of `512`.

Additionally, this part type does not support styling through the addition of
`Class.Decal|Decals` or `Class.Texture|Textures`. If you wish to create a
textured and "climbable" `Class.BasePart` but also utilize the climbing
behavior of `TrussPart`, consider setting the
`Class.BasePart.Transparency|Transparency` of the `TrussPart` to `1` to make
it invisible, set `Class.BasePart.CanCollide|CanCollide` on the
`Class.BasePart` to `false`, and then align the climbable surface of the
mesh/model with that of the `TrussPart`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.TrussPart.Style` | `Enum.Style` | [NotReplicated] |
