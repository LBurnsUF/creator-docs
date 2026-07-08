---
title: PermissionLevelShown
type: enum
---

# `Enum.PermissionLevelShown`

Used to set the highest permission level that APIs have to have in order to be
shown in the Object Browser.

Used to set the highest permission level that APIs have to have in order to be
shown in the Object Browser.

The `Enum.PermissionLevelShown` enum has 5 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.PermissionLevelShown.Game` | 0 | Member must have no security permissions in order to be shown. |
| `Enum.PermissionLevelShown.RobloxGame` | 1 | Member must have security permissions less than or equal to **RobloxPlaceSecurity** to be shown. |
| `Enum.PermissionLevelShown.RobloxScript` | 2 | Member must have security permissions less than or equal to **RobloxScriptSecurity** to be shown. |
| `Enum.PermissionLevelShown.Studio` | 3 | Member must have security permissions less than or equal to **LocalUserSecurity** to be shown. |
| `Enum.PermissionLevelShown.Roblox` | 4 | Member is shown no matter what security it has. |
