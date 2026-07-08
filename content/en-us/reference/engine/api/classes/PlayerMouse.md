---
title: PlayerMouse
type: class
superclass: Mouse
tags: [NotCreatable]
---

# PlayerMouse

The PlayerMouse behaves identically to the `Class.Mouse` object that is
obtained using `Class.Tool.Equipped`. Both PlayerMouse and `Class.Mouse` are
legacy APIs, superseded by `Class.UserInputService`.

**Inherits from:** `Class.Mouse` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

The PlayerMouse behaves identically to the `Class.Mouse` object that is
obtained using `Class.Tool.Equipped`. It can be accessed from
`Class.LocalScript|LocalScripts` using the local player's
`Class.Player:GetMouse()` method. Both PlayerMouse and `Class.Mouse` are
legacy APIs, superseded by `Class.UserInputService`.

The only difference between the PlayerMouse and the `Class.Mouse` object is
the PlayerMouse can be obtained using the `Class.Player:GetMouse()` method.

In most cases developers are advised to use the new `Class.UserInputService`.
However the PlayerMouse and Mouse objects remain supported for a number of
reasons. See [Input and Camera](../../../input/index.md) for more information
on customizing inputs in your experience.
