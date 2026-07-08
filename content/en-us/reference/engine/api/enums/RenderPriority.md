---
title: RenderPriority
type: enum
---

# `Enum.RenderPriority`

A list of standard reserved values in BindToRenderStep.

A list of standard reserved values in BindToRenderStep.

See `Class.RunService:BindToRenderStep()` for the proper usage, as the enum
itself isn't used.

The `Enum.RenderPriority` enum has 5 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.RenderPriority.First` | 0 | This should run first. |
| `Enum.RenderPriority.Input` | 100 | This should run as second. |
| `Enum.RenderPriority.Camera` | 200 | This should run after Input. |
| `Enum.RenderPriority.Character` | 300 | This should run after Camera. |
| `Enum.RenderPriority.Last` | 2000 | This should run as last, after Character. |
