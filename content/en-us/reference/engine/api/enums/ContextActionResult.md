---
title: ContextActionResult
type: enum
---

# `Enum.ContextActionResult`

Describes whether a contextual action should sink or pass input events.

`ContextActionResult` controls the behavior of multiple bound actions. It
gives the option of controlling whether or not a bound action should sink or
pass the input event, meaning other things (including other bound actions) can
process it.

The `Enum.ContextActionResult` enum has 2 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.ContextActionResult.Sink` | 0 | If `functionToBind` from `Class.ContextActionService:BindAction()` returns `Enum.ContextActionResult |
| `Enum.ContextActionResult.Pass` | 1 | If `functionToBind` from `Class.ContextActionService:BindAction()` returns `Enum.ContextActionResult |
