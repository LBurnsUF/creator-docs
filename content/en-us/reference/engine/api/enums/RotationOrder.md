---
title: RotationOrder
type: enum
---

# `Enum.RotationOrder`

The order of rotation axes used for Euler angles encoding of rotations.

Euler angles encode a rotation in 3D space via a sequence of three rotations
along the X, Y, and Z axes. The `RotationOrder` enum specifies the order in
which the engine performs these rotations.

To help visualize the many rotation orders, you can test them manually in
Studio with the [Rotate](../../../parts#rotate) tool or by inserting
`Library.task.wait()` statements between individual rotations of a cube with a
unique face:

```lua
local Workspace = game:GetService("Workspace")

local cube = Workspace.Cube
local rx, ry, rz = math.rad(90), math.rad(90), math.rad(90)

task.wait(5)
cube.CFrame *= CFrame.fromEulerAngles(rx, 0, 0)  -- X
task.wait(5)
cube.CFrame *= CFrame.fromEulerAngles(0, ry, 0)  -- Y
task.wait(5)
cube.CFrame *= CFrame.fromEulerAngles(0, 0, rz)  -- Z
```

An equivalent operation is:

```lua
local Workspace = game:GetService("Workspace")

local cube = Workspace.Cube
local rx, ry, rz = math.rad(90), math.rad(90), math.rad(90)

cube.CFrame = CFrame.fromEulerAngles(rx, ry, rz, Enum.RotationOrder.XYZ)
```

The `Enum.RotationOrder` enum has 6 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.RotationOrder.XYZ` | 0 | X, Y, Z order. |
| `Enum.RotationOrder.XZY` | 1 | X, Z, Y order. |
| `Enum.RotationOrder.YZX` | 2 | Y, Z, X order. |
| `Enum.RotationOrder.YXZ` | 3 | Y, X, Z order. |
| `Enum.RotationOrder.ZXY` | 4 | Z, X, Y order. |
| `Enum.RotationOrder.ZYX` | 5 | Z, Y, X order. |
