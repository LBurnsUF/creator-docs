---
title: Animation
type: class
superclass: Instance
---

# Animation

References an animation asset which can be loaded by an
`Class.AnimationController`.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

An object that references an animation asset
(`Class.Animation.AnimationId|AnimationId`) which can be loaded by an
`Class.AnimationController`.

#### Loading an Animation on Client or Server

In order for `Class.AnimationTrack|AnimationTracks` to replicate correctly,
it's important to know when they should be loaded on the client or on the
server:

- If an `Class.Animator` is a descendant of a `Class.Humanoid` or
  `Class.AnimationController` in a player's `Class.Player.Character`,
  animations started on that player's client will be replicated to the server
  and other clients.

- If the `Class.Animator` is **not** a descendant of a player character, its
  animations must be loaded and started on the server to replicate.

The `Class.Animator` object must be initially created on the server and
replicated to clients for animation replication to work at all. If an
`Class.Animator` is created locally, then
`Class.AnimationTrack|AnimationTracks` loaded with that `Class.Animator` will
not replicate.

See also [Animation Editor](../../../animation/editor.md) and
[Using Animations](../../../animation/using.md) to learn how to create and add
pre-built or custom animations to your game.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Animation.AnimationContent` | `Datatype.Content` |  |
| `Class.Animation.AnimationId` | `Datatype.ContentId` |  |
