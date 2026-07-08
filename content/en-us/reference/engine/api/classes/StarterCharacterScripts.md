---
title: StarterCharacterScripts
type: class
superclass: StarterPlayerScripts
tags: [NotCreatable]
---

# StarterCharacterScripts

Stores instances to be parented to a player's character when it spawns.

**Inherits from:** `Class.StarterPlayerScripts` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

The `Class.StarterCharacterScripts` container stores scripts to be parented to
a player's `Class.Player.Character` when it spawns. Unlike scripts stored in
the `Class.StarterPlayerScripts` folder, these scripts will not persist when
the character respawns.

If a `Class.LocalScript` named `Animate`, `Sound`, or `Health` is placed in
this container, it will replace the default script that manages character
animations, character sounds, and character health regeneration respectively.
