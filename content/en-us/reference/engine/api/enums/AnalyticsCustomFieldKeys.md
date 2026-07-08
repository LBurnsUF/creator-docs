---
title: AnalyticsCustomFieldKeys
type: enum
---

# `Enum.AnalyticsCustomFieldKeys`

Used to form a dictionary of custom fields to provide breakdowns in
Roblox-provided charts.

Used to form a dictionary of custom fields to provide breakdowns in
Roblox-provided charts. For example:

```lua
local customFields = {
	[Enum.AnalyticsCustomFieldKeys.CustomField01.Name] = "value1",
	[Enum.AnalyticsCustomFieldKeys.CustomField02.Name] = "value2",
	[Enum.AnalyticsCustomFieldKeys.CustomField03.Name] = "value3",
}
```

The `Enum.AnalyticsCustomFieldKeys` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.AnalyticsCustomFieldKeys.CustomField01` | 0 |  |
| `Enum.AnalyticsCustomFieldKeys.CustomField02` | 1 |  |
| `Enum.AnalyticsCustomFieldKeys.CustomField03` | 2 |  |
