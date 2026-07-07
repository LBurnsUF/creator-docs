---
title: VirtualInput
type: class
superclass: Object
tags: [NotCreatable, NotReplicated]
---

# VirtualInput

**Inherits from:** `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Methods

### `Class.VirtualInput:SendKey`

``SendKey(isPressed: `bool`, keyCode: `Enum.KeyCode`, isRepeatedKey: `bool`)`` → `null`

### `Class.VirtualInput:SendMouseButton`

``SendMouseButton(position: `Datatype.Vector2`, button: `Enum.UserInputType`, isDown: `bool`, repeatCount: `int`)`` → `null`

### `Class.VirtualInput:SendMouseDelta`

``SendMouseDelta(positionDelta: `Datatype.Vector2`)`` → `null`

### `Class.VirtualInput:SendMousePosition`

``SendMousePosition(position: `Datatype.Vector2`)`` → `null`

### `Class.VirtualInput:SendPointerAction`

``SendPointerAction(position: `Datatype.Vector2`, pointerAction: `Dictionary`)`` → `null`

### `Class.VirtualInput:SendTextInput`

``SendTextInput(text: `string`)`` → `null`
