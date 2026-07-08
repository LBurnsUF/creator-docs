---
title: ModelStreamingMode
type: enum
---

# `Enum.ModelStreamingMode`

Controls stream in and out behavior of a model.

Controls how model is streamed in and out when used in an experience that is
streaming enabled. Has no effect when experience is not streaming enabled.

The `Enum.ModelStreamingMode` enum has 5 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.ModelStreamingMode.Default` | 0 | Default behavior (subject to change). |
| `Enum.ModelStreamingMode.Atomic` | 1 | The `Class.Model` and all of its descendants are streamed in/out together. For streaming in, this ap |
| `Enum.ModelStreamingMode.Persistent` | 2 | Persistent models are sent as a complete atomic unit soon after the player joins and before the `Cla |
| `Enum.ModelStreamingMode.PersistentPerPlayer` | 3 | Behaves as a persistent model for players that have been added using `Class.Model:AddPersistentPlaye |
| `Enum.ModelStreamingMode.Nonatomic` | 4 | When a nonatomic model is streamed, descendants are also sent, except for part descendants. Nonatomi |
