---
title: ModelStreamingBehavior
type: enum
---

# `Enum.ModelStreamingBehavior`

Controls how `Class.Model|Models` are sent to clients in experiences with
instance streaming enabled.

Controls how `Class.Model|Models` are replicated in experiences when instance
[streaming](../../../workspace/streaming/index.md) is enabled. Only affects
models with `Class.Model.ModelStreamingMode|ModelStreamingMode` set to
`Enum.ModelStreamingMode|Default`/`Enum.ModelStreamingMode|Nonatomic`.

The `Enum.ModelStreamingBehavior` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.ModelStreamingBehavior.Default` | 0 | Default behavior (subject to change). |
| `Enum.ModelStreamingBehavior.Legacy` | 1 | Models are sent when their parent is sent, typically during player join. Models are never streamed o |
| `Enum.ModelStreamingBehavior.Improved` | 2 | Models are never sent during player join. See [model streaming controls](../../../workspace/streamin |
