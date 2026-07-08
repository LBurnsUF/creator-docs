---
title: AdAvailabilityResult
type: enum
---

# `Enum.AdAvailabilityResult`

The `Enum.AdAvailabilityResult` enum has 7 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.AdAvailabilityResult.IsAvailable` | 1 | An ad is available to show the user. |
| `Enum.AdAvailabilityResult.DeviceIneligible` | 2 | The device is ineligible to receive ads. |
| `Enum.AdAvailabilityResult.ExperienceIneligible` | 3 | The experience is ineligible to receive ads. Check if its eligibility has been revoked. |
| `Enum.AdAvailabilityResult.InternalError` | 4 | An unspecified internal error occurred. Try fetching the ad again. |
| `Enum.AdAvailabilityResult.NoFill` | 5 | There are no ads available to fill your ad request. You might have hit the ad frequency limit. |
| `Enum.AdAvailabilityResult.PlayerIneligible` | 6 | The user is ineligible to receive ads during this session. The user might be under 13 or located in  |
| `Enum.AdAvailabilityResult.PublisherIneligible` | 7 | The publisher is ineligible to receive ads because they have not met the publisher eligibility requi |
