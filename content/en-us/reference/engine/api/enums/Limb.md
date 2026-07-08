---
title: Limb
type: enum
---

# `Enum.Limb`

Describes which limb a particular Instance belongs to (assuming the Instance
is part of a Humanoid).

Describes which limb a particular Instance belongs to (assuming the Instance
is part of a Humanoid). Passing an Instance to the Humanoid:GetLimb() function
will return the Limb for the Instance.

The `Enum.Limb` enum has 7 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.Limb.Head` | 0 | If the limb is a part of the Humanoid's Head. |
| `Enum.Limb.Torso` | 1 | If the limb is a part of the Humanoid's Torso. This includes UpperTorso and LowerTorso for R15 rigs. |
| `Enum.Limb.LeftArm` | 2 | If the limb is a part of the Humanoid's Left Arm. This includes UpperLeftArm, LowerLeftArm, and Left |
| `Enum.Limb.RightArm` | 3 | If the limb is a part of the Humanoid's Right Arm. This includes UpperRightArm, LowerRightArm and Ri |
| `Enum.Limb.LeftLeg` | 4 | If the limb is a part of the Humanoid's Left Leg. This includes UpperLeftLeg, LowerLeftLeg and LeftF |
| `Enum.Limb.RightLeg` | 5 | If the limb is a part of the Humanoid's Right Leg. This includes UpperRightLeg, LowerRightLeg, and R |
| `Enum.Limb.Unknown` | 6 | If a part is not a limb (e.g. running the `Class.Humanoid:GetLimb()` function and passing it an acce |
