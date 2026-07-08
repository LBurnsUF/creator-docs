---
title: TweenStatus
type: enum
---

# `Enum.TweenStatus`

The completion status of a `Class.GuiObject` tween function.

Describes the completion status of a `Class.GuiObject` tween function.

Passed as an argument to the callback function provided to
`Class.GuiObject:TweenPosition()`, `Class.GuiObject:TweenSize()`, and
`Class.GuiObject:TweenSizeAndPosition()`.

Not to be confused for `Enum.PlaybackState` which is used with
`Class.TweenService`.

The `Enum.TweenStatus` enum has 2 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.TweenStatus.Canceled` | 0 | The tween was cancelled before completion. |
| `Enum.TweenStatus.Completed` | 1 | The Tween has successfully completed. |
