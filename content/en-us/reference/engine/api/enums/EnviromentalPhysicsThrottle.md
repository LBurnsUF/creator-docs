---
title: EnviromentalPhysicsThrottle
type: enum
---

# `Enum.EnviromentalPhysicsThrottle`

Used to control the throttle rate of Roblox's physics engine.

The `EnviromentalPhysicsThrottle` enum is used with
`Class.PhysicsSettings.PhysicsEnvironmentalThrottle`, controlling how
aggressively the engine skips physics simulation steps to reduce CPU load.

The `Enum.EnviromentalPhysicsThrottle` enum has 7 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.EnviromentalPhysicsThrottle.DefaultAuto` | 0 | Automatically adjusts throttle level based on performance. |
| `Enum.EnviromentalPhysicsThrottle.Disabled` | 1 | No throttling; every physics step runs. |
| `Enum.EnviromentalPhysicsThrottle.Always` | 2 | Maximum throttling; physics is effectively frozen. |
| `Enum.EnviromentalPhysicsThrottle.Skip2` | 3 | Runs 1 out of every 2 steps (50% reduction). If `Class.Workspace.PhysicsSteppingMethod` is set to `E |
| `Enum.EnviromentalPhysicsThrottle.Skip4` | 4 | Runs 1 out of every 4 steps (75% reduction). If `Class.Workspace.PhysicsSteppingMethod` is set to `E |
| `Enum.EnviromentalPhysicsThrottle.Skip8` | 5 | Runs 1 out of every 8 steps (87.5% reduction). If `Class.Workspace.PhysicsSteppingMethod` is set to  |
| `Enum.EnviromentalPhysicsThrottle.Skip16` | 6 | Runs 1 out of every 16 steps (93.75% reduction). If `Class.Workspace.PhysicsSteppingMethod` is set t |
