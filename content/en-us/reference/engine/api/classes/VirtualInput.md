---
title: VirtualInput
type: class
superclass: Object
tags: [NotCreatable, NotReplicated]
---

# VirtualInput

Simulates mouse, keyboard, and pointer input as if it were performed by a real
player.

**Inherits from:** `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

`Class.VirtualInput` simulates mouse, keyboard, and pointer input as if it
were performed by a real player. It is intended for **testing purposes only**
and can only be obtained by calling
`Class.UserInputService:CreateVirtualInput()`.

All input methods throw a runtime error if the simulated input would interact
with Roblox's built-in UI (`Class.CoreGui`), such as the top bar, chat window,
or escape menu. This prevents automation tests from accidentally interfering
with system UI that players depend on.

## Methods

### `Class.VirtualInput:SendKey`

``SendKey(isPressed: `bool`, keyCode: `Enum.KeyCode`, isRepeatedKey: `bool`)`` -> `null`

### `Class.VirtualInput:SendMouseButton`

``SendMouseButton(position: `Datatype.Vector2`, button: `Enum.UserInputType`, isDown: `bool`, repeatCount: `int`)`` -> `null`

### `Class.VirtualInput:SendMouseDelta`

``SendMouseDelta(positionDelta: `Datatype.Vector2`)`` -> `null`

### `Class.VirtualInput:SendMousePosition`

``SendMousePosition(position: `Datatype.Vector2`)`` -> `null`

### `Class.VirtualInput:SendPointerAction`

``SendPointerAction(position: `Datatype.Vector2`, pointerAction: `Dictionary`)`` -> `null`

### `Class.VirtualInput:SendTextInput`

``SendTextInput(text: `string`)`` -> `null`
