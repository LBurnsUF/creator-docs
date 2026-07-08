---
title: RecommendationPreferenceType
type: enum
---

# `Enum.RecommendationPreferenceType`

The type of preference signal logged via
`Class.RecommendationService.LogPreferenceEvent|LogPreferenceEvent`.
Preference signals capture follow, unfollow, mute, and unmute actions toward
another user, a universe, or a custom content tag, and are used by the
recommendation engine to personalize future results.

The `Enum.RecommendationPreferenceType` enum has 4 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.RecommendationPreferenceType.AddFollow` | 0 | The user started following the target. |
| `Enum.RecommendationPreferenceType.RemoveFollow` | 1 | The user stopped following the target. |
| `Enum.RecommendationPreferenceType.AddMute` | 2 | The user muted the target. |
| `Enum.RecommendationPreferenceType.RemoveMute` | 3 | The user unmuted a previously muted target. |
