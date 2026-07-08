---
title: Skin
type: class
superclass: CharacterAppearance
tags: [Deprecated]
---

# Skin

Historically changed the colors of body parts to match the
`Class.Skin.SkinColor` property. Superseded by the `Class.BodyColors` class.

**Inherits from:** `Class.CharacterAppearance` > `Class.Instance` > `Class.Object`

**Tags:** [Deprecated]

## Description

The Skin object, when placed into a humanoid model, will change the colors all
body parts of the torso, head, etc, to value of the `Class.Skin.SkinColor`
property.

Superseded by the `Class.BodyColors` class.

> **Deprecated:** This object has been deprecated and superseded by `Class.BodyColors`. The Skin
object does not function on R15 characters and should not be used for new
work. `Class.BodyColors` functions with R15 characters and allows the colors
of each limb to be set individually.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Skin.SkinColor` | `Datatype.BrickColor` |  |
