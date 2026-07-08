---
title: ExperienceEventStatus
type: enum
---

# `Enum.ExperienceEventStatus`

Represents the lifecycle state of an experience event returned by
`Class.SocialService`.

The `Enum.ExperienceEventStatus` enum has 5 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.ExperienceEventStatus.Active` | 0 | The event is currently published and available. |
| `Enum.ExperienceEventStatus.Cancelled` | 1 | The event has been cancelled and will not occur. |
| `Enum.ExperienceEventStatus.Moderated` | 2 | The event has been removed by moderation. |
| `Enum.ExperienceEventStatus.Unpublished` | 3 | The event has been unpublished by the creator. |
| `Enum.ExperienceEventStatus.Unknown` | 4 | The event status could not be determined. |
