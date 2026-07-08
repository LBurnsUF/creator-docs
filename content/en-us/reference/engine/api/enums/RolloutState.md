---
title: RolloutState
type: enum
---

# `Enum.RolloutState`

A three-phase rollout state used to opt in or out of engine features.

Several `Class.Workspace` properties use `RolloutState` to support a
three-phase rollout pattern, where a feature is initially opt-in (`Default`
equals disabled), then opt-out (`Default` equals enabled), and finally always
on. `Default` always tracks the current engine-wide phase.

The `Enum.RolloutState` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.RolloutState.Default` | 0 | Uses the engine-wide rollout default, which changes as the feature progresses through its rollout ph |
| `Enum.RolloutState.Disabled` | 1 | Opts out of the feature regardless of the engine-wide rollout phase. |
| `Enum.RolloutState.Enabled` | 2 | Opts in to the feature regardless of the engine-wide rollout phase. |
