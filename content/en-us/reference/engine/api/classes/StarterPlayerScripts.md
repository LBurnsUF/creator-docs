---
title: StarterPlayerScripts
type: class
superclass: Instance
tags: [NotCreatable]
---

# StarterPlayerScripts

A container for objects to be copied to a Player's PlayerScripts when they
join a game.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

`Class.StarterPlayerScripts` is a container object located within the
`Class.StarterPlayer` service. It can contain `Class.LocalScript|LocalScripts`
and other objects to be copied to the `Class.PlayerScripts` container once
when a `Class.Player` joins the game. For example, if you want to create
special effects on the client when certain conditions are met, you can place a
`Class.LocalScript` within this container to do that.

When an experience is run, this object will also house the default
multi-platform Roblox control scripts for the camera and character. If
`Class.LocalScript|LocalScripts` named `CameraScript` or `ControlScript` are
placed within this container, they will **replace** the Roblox defaults for
those scripts respectively. If desired, you can add empty
`Class.LocalScript|LocalScripts` for each of these to disable them altogether;
this is useful for experiences that do not follow the typical control
paradigms of a Roblox experience.
