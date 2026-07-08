---
title: AnalyticsLogLevel
type: enum
---

# `Enum.AnalyticsLogLevel`

This enum is used as an argument in `Class.AnalyticsService.LogEvent` to
describe the error severity level.

The `Enum.AnalyticsLogLevel` enum has 6 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.AnalyticsLogLevel.Trace` | 0 | Trace is the noisiest level, rarely (if ever) enabled for a production app. |
| `Enum.AnalyticsLogLevel.Debug` | 1 | Used for debugging. |
| `Enum.AnalyticsLogLevel.Information` | 2 |  |
| `Enum.AnalyticsLogLevel.Warning` | 3 | Used for warning. |
| `Enum.AnalyticsLogLevel.Error` | 4 | When functionality is unavailable or expectations broken. |
| `Enum.AnalyticsLogLevel.Fatal` | 5 | The most critical level, Fatal events demand immediate attention. |
