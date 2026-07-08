---
title: HumanoidHealthDisplayType
type: enum
---

# `Enum.HumanoidHealthDisplayType`

Controls under what circumstances the `Class.Humanoid` health bar is
displayed.

Controls when the `Class.Humanoid` health bar is displayed. This works in
conjunction with the `Class.Humanoid.MaxHealth` property which must have a
value higher than zero or the health bar doesn't display.

The `Enum.HumanoidHealthDisplayType` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.HumanoidHealthDisplayType.DisplayWhenDamaged` | 0 | The humanoid's health bar is only visible when the humanoid is not at full health (assuming `MaxHeal |
| `Enum.HumanoidHealthDisplayType.AlwaysOn` | 1 | The humanoid's health bar is always visible (assuming `MaxHealth` is greater than zero). |
| `Enum.HumanoidHealthDisplayType.AlwaysOff` | 2 | The humanoid's health bar is never visible. |
