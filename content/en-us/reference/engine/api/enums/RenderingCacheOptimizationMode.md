---
title: RenderingCacheOptimizationMode
type: enum
---

# `Enum.RenderingCacheOptimizationMode`

Controls rendering cache optimization behavior.

Determines whether the renderer caches per-object rendering state to avoid
redundant per-frame work. This enum is used by
`Class.Workspace.RenderingCacheOptimizations`.

The `Enum.RenderingCacheOptimizationMode` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.RenderingCacheOptimizationMode.Default` | 0 | Uses the engine-default rendering cache state. |
| `Enum.RenderingCacheOptimizationMode.Disabled` | 1 | Rendering cache optimizations are disabled. |
| `Enum.RenderingCacheOptimizationMode.Enabled` | 2 | Rendering cache optimizations are enabled. |
