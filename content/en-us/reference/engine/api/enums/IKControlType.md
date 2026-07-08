---
title: IKControlType
type: enum
---

# `Enum.IKControlType`

Used on `Class.IKControl` to specify their `Class.IKControl.Type|Type`, to
change their behavior.

Used on `Class.IKControl` to specify their `Class.IKControl.Type|Type`, to
change their behavior.

The `Enum.IKControlType` enum has 4 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.IKControlType.Transform` | 0 | It is a full 6-DoF constraint. Aligns the `Class.IKControl.EndEffector/EndEffector` `Datatype.CFrame |
| `Enum.IKControlType.Position` | 1 | Aligns the `Class.IKControl.EndEffector/EndEffector` position to that of the `Class.IKControl.Target |
| `Enum.IKControlType.Rotation` | 2 | Aligns the `Class.IKControl.EndEffector/EndEffector` rotation to that of the `Class.IKControl.Target |
| `Enum.IKControlType.LookAt` | 3 | Moves and orients the whole chain to make the forward axis on the `Class.IKControl.EndEffector/EndEf |
