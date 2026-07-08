---
title: PredictionStatus
type: enum
---

# `Enum.PredictionStatus`

Enum used with `Class.RunService:GetPredictionStatus()` to check the status of
a specific instance.

Enum used with `Class.RunService:GetPredictionStatus()` to check the status of
a specific instance.

This prediction status can be used to determine whether any associated scripts
should run. If the status is `Authoritative` or `Predicted`, such scripts
should run, since the local node is either the authority for the instance or
is predicting it. If the status is `None`, such scripts do not need to run.

The `Enum.PredictionStatus` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.PredictionStatus.Authoritative` | 0 | This instance is authoritative. |
| `Enum.PredictionStatus.Predicted` | 1 | This instance is being predicted. |
| `Enum.PredictionStatus.None` | 2 | The instance will not be resimulated; classic simulation rules apply instead. |
