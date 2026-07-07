---
title: VirtualInput
type: class
superclass: Object
tags: [NotCreatable, NotReplicated]
---

# VirtualInput

**Inherits**: Object

**Tags**: NotCreatable, NotReplicated

## Methods

- **SendKey**(`isPressed: bool`, `keyCode: KeyCode`, `isRepeatedKey: bool = false`) -> `null`
- **SendMouseButton**(`position: Vector2`, `button: UserInputType`, `isDown: bool`, `repeatCount: int = 0`) -> `null`
- **SendMouseDelta**(`positionDelta: Vector2`) -> `null`
- **SendMousePosition**(`position: Vector2`) -> `null`
- **SendPointerAction**(`position: Vector2`, `pointerAction: Dictionary`) -> `null`
- **SendTextInput**(`text: string`) -> `null`
