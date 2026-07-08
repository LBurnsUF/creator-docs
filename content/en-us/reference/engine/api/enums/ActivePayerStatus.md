---
title: ActivePayerStatus
type: enum
---

# `Enum.ActivePayerStatus`

Describes a player's payer status bucket for the current experience.

The `ActivePayerStatus` enum describes a player's payer status bucket for the
current experience.

The `Enum.ActivePayerStatus` enum has 6 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.ActivePayerStatus.Unknown` | 0 | Segment data is unavailable. |
| `Enum.ActivePayerStatus.Never` | 1 | The player has not made a qualifying purchase in the experience. |
| `Enum.ActivePayerStatus.Lapsed` | 2 | The player has previously spent in the experience but is not currently an active payer. |
| `Enum.ActivePayerStatus.Casual50Percent` | 3 | The player is in the casual payer bucket for the experience. |
| `Enum.ActivePayerStatus.Intermediate35Percent` | 4 | The player is in the intermediate payer bucket for the experience. |
| `Enum.ActivePayerStatus.Top15Percent` | 5 | The player is in the top payer bucket for the experience. |
