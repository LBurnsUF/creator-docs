---
title: HumanoidStateType
type: enum
---

# `Enum.HumanoidStateType`

Describes the physics control states within the Humanoid.

Identifies, reads and sets the physics control state of a `Class.Humanoid`.
`Class.Humanoid:GetState()` and `Class.Humanoid:ChangeState()` methods, as
well as the `Class.Humanoid.StateChanged` event currently use this Enum.

Some states only allow manual setting, and allow a developer to make the
Humanoid relinquish control of its character.

When altering the Humanoid of a player, this should be done from a
`Class.LocalScript` ran by that player on their local client. Certain states
only work when set by the owner process (client or server). (Dead for example)

The `Enum.HumanoidStateType` enum has 17 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.HumanoidStateType.FallingDown` | 0 | The Humanoid has been tripped, and will attempt to get up in a few moments. |
| `Enum.HumanoidStateType.Ragdoll` | 1 | (Deprecated) The Humanoid has been hit by a fast moving object (uncontrolled falling). _The Humanoid |
| `Enum.HumanoidStateType.GettingUp` | 2 | The Humanoid is getting back on their feet after FallingDown or Ragdoll. |
| `Enum.HumanoidStateType.Jumping` | 3 | The Humanoid just jumped. (Check `Class.Humanoid.Jump`). This state lasts only briefly. This state n |
| `Enum.HumanoidStateType.Swimming` | 4 | The Humanoid is currently swimming in `Class.Terrain` water. |
| `Enum.HumanoidStateType.Freefall` | 5 | The Humanoid is currently freefalling (jumped from a height or fell off a ledge). |
| `Enum.HumanoidStateType.Flying` | 6 | When set, the Humanoid won't be animated, as with the `Class.Humanoid.PlatformStand` property. This  |
| `Enum.HumanoidStateType.Landed` | 7 | The Humanoid touched the ground after a Freefall. This state lasts only briefly. |
| `Enum.HumanoidStateType.Running` | 8 | Currently running while on the ground. |
| `Enum.HumanoidStateType.RunningNoPhysics` | 10 | (Deprecated) Currently running and not near other physical objects. |
| `Enum.HumanoidStateType.StrafingNoPhysics` | 11 | Not currently used with default Humanoid. Cannot be set with `Class.Humanoid:ChangeState()`. |
| `Enum.HumanoidStateType.Climbing` | 12 | The Humanoid is climbing (e.g. up a `Class.TrussPart` or ladder). |
| `Enum.HumanoidStateType.Seated` | 13 | The Humanoid is currently sitting in a Seat or VehicleSeat. Check the `Class.Humanoid.Sit` property. |
| `Enum.HumanoidStateType.PlatformStanding` | 14 | The Humanoid is platformstanding. Check the `Class.Humanoid.PlatformStand` property. |
| `Enum.HumanoidStateType.Dead` | 15 | The Humanoid died. Changing a Humanoid's state to this state will kill it. |
| `Enum.HumanoidStateType.Physics` | 16 | The Humanoid doesn't apply any force on its own and will not automatically transition to any other s |
| `Enum.HumanoidStateType.None` | 18 | Unusable placeholder in case an unknown state gets triggered internally. |
