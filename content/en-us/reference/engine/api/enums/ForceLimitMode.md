---
title: ForceLimitMode
type: enum
---

# `Enum.ForceLimitMode`

The **ForceLimitMode** enum determines how the maximum force for a constraint
is specified and how that limit is enforced by the constraint.

This enum is used to determine how the maximum force for a constraint is
specified and how that limit will be enforced by the constraint.

The `Enum.ForceLimitMode` enum has 2 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.ForceLimitMode.Magnitude` | 0 | A single number is used to specify the magnitude of the maximum constraint force. The constraint wil |
| `Enum.ForceLimitMode.PerAxis` | 1 | A vector is used to specify the maximum force value along each axis of a given reference frame. The  |
