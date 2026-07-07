---
title: UIPageLayout
type: class
superclass: UIGridStyleLayout
---

# UIPageLayout

**Inherits**: UIGridStyleLayout > UILayout > UIComponent > UIBase > Instance > Object

## Properties

- **Animated**: `bool`
- **Circular**: `bool`
- **CurrentPage**: `GuiObject` [ReadOnly] [NotReplicated]
- **EasingDirection**: `EasingDirection`
- **EasingStyle**: `EasingStyle`
- **GamepadInputEnabled**: `bool`
- **Padding**: `UDim`
- **ScrollWheelInputEnabled**: `bool`
- **TouchInputEnabled**: `bool`
- **TweenTime**: `float`

## Methods

- **JumpTo**(`page: Instance`) -> `null`
- **JumpToIndex**(`index: int`) -> `null`
- **Next**() -> `null`
- **Previous**() -> `null`

## Events

- **PageEnter**(`page: Instance`)
- **PageLeave**(`page: Instance`)
- **Stopped**(`currentPage: Instance`)
