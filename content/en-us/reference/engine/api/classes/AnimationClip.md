---
title: AnimationClip
type: class
superclass: Instance
tags: [NotCreatable]
---

# AnimationClip

Represents all types of animation data that the Roblox animation system can
consume.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

The non-creatable `Class.AnimationClip` instance type represents abstract
animation data that can be fed to the Roblox animation system.
`Class.KeyframeSequence` and `Class.CurveAnimation` are two current instance
types that inherit from `Class.AnimationClip`.

There are different ways to represent animation data. To simplify the use of
Roblox's animation system, all such representations are their own instance
types but inherit from the `Class.AnimationClip` instance. Animation clips
published to Roblox via the [Animation Editor](../../../animation/editor.md)
can be loaded into the Roblox Engine using an `Class.Animation` instance.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AnimationClip.Guid` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.AnimationClip.Length` | `float` | [ReadOnly] [NotReplicated] |
| `Class.AnimationClip.Loop` | `bool` |  |
| `Class.AnimationClip.Priority` | `Enum.AnimationPriority` |  |
