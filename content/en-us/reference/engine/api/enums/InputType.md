---
title: InputType
type: enum
---

# `Enum.InputType`

The InputType Enum controls the SurfaceInputs of `Class.Part`.

The InputType Enum controls the SurfaceInputs of `Class.Part`. Several
parameters here are left-overs from 2005, before Roblox was a multiplayer
game, and are used by `Class.Part.BackSurfaceInput`,
`Class.Part.BottomSurfaceInput`, `Class.Part.FrontSurfaceInput`,
`Class.Part.LeftSurfaceInput`, `Class.Part.RightSurfaceInput`,
`Class.Part.TopSurfaceInput`.

The `Enum.InputType` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.InputType.NoInput` | 0 | Behaves like a weld and does nothing. |
| `Enum.InputType.Constant` | 12 | Rotate at a constant velocity of `Class.BasePart` `ParamB`. |
| `Enum.InputType.Sin` | 13 | Rotate at a velocity of: `ParamA * math.sin(workspace.DistributedGameTime * ParamB)`, where `Class.B |
