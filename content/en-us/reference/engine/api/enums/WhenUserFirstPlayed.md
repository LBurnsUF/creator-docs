---
title: WhenUserFirstPlayed
type: enum
---

# `Enum.WhenUserFirstPlayed`

Describes when a player first played the current experience, represented as a
bucket.

The `WhenUserFirstPlayed` enum describes when a player first played the
current experience, represented as a bucket.

The `Enum.WhenUserFirstPlayed` enum has 6 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.WhenUserFirstPlayed.Unknown` | 0 | Segment data is unavailable. |
| `Enum.WhenUserFirstPlayed.Days0To30` | 1 | The player first played the experience within the last 30 days. |
| `Enum.WhenUserFirstPlayed.Days31To90` | 2 | The player first played the experience between 31 and 90 days ago. |
| `Enum.WhenUserFirstPlayed.Days91To180` | 3 | The player first played the experience between 91 and 180 days ago. |
| `Enum.WhenUserFirstPlayed.Days181To365` | 4 | The player first played the experience between 181 and 365 days ago. |
| `Enum.WhenUserFirstPlayed.Days366Plus` | 5 | The player first played the experience more than 365 days ago. |
