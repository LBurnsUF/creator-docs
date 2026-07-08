---
title: AnalyticsProgressionStatus
type: enum
---

# `Enum.AnalyticsProgressionStatus`

This enum is used as an argument in
`Class.AnalyticsService:FirePlayerProgressionEvent()` to describe the status
of progression.

This enum is used as an argument in
`Class.AnalyticsService:FirePlayerProgressionEvent()` to describe the status
of progression.

The `Enum.AnalyticsProgressionStatus` enum has 5 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.AnalyticsProgressionStatus.Default` | 0 | Default status. Used for an undefined status. |
| `Enum.AnalyticsProgressionStatus.Begin` | 1 | Indicates the beginning of progression. |
| `Enum.AnalyticsProgressionStatus.Complete` | 2 | Indicates the progression completed. |
| `Enum.AnalyticsProgressionStatus.Abandon` | 3 | Indicates the progression abandoned. |
| `Enum.AnalyticsProgressionStatus.Fail` | 4 | Indicates the progression failed. |
