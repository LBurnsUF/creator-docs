---
title: FormFactor
type: enum
---

# `Enum.FormFactor`

The FormFactor Enum for `Class.FormFactorPart.FormFactor`.

Minimum size along a given axis is 1 \* RateOfIncrease for that axis, except
in the case of the "Custom" FormFactor, which has a minimum size of 0.2 along
all axes.

The `Enum.FormFactor` enum has 4 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.FormFactor.Symmetric` | 0 | Increases by a rate of 1 along all axes. |
| `Enum.FormFactor.Brick` | 1 | Increases by a rate of 1 along the x- and z- axes, 1.2 along the y-axis. |
| `Enum.FormFactor.Plate` | 2 | Increases by a rate of 1 along the x- and z- axes, 0.4 along the y-axis. |
| `Enum.FormFactor.Custom` | 3 | Increases by a rate as low as .001 along all axes. |
