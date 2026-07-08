---
title: RecommendationPreferenceTargetType
type: enum
---

# `Enum.RecommendationPreferenceTargetType`

The kind of entity a preference signal targets when logged via
`Class.RecommendationService.LogPreferenceEvent|LogPreferenceEvent`.
Determines how the `targetId` parameter is interpreted.

The `Enum.RecommendationPreferenceTargetType` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.RecommendationPreferenceTargetType.User` | 0 | The target is another Roblox user. The `targetId` is the user key. |
| `Enum.RecommendationPreferenceTargetType.Universe` | 1 | The target is a universe. The `targetId` is the universe ID as a string. |
| `Enum.RecommendationPreferenceTargetType.CustomTag` | 2 | The target is a custom content tag. The `targetId` is the tag string. |
