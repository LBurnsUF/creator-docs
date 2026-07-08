---
title: PackagePermission
type: enum
---

# `Enum.PackagePermission`

Indicates the current user's or group roleset's permission to the package.

The `Enum.PackagePermission` indicates the current user's or group roleset's
permission to the package.

The `Enum.PackagePermission` enum has 6 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.PackagePermission.None` | 0 | Permission data is not available for the current user or group roleset. |
| `Enum.PackagePermission.NoAccess` | 1 | The current user or group roleset doesn't have access. |
| `Enum.PackagePermission.Revoked` | 2 | The current user's or group roleset's permission is revoked. |
| `Enum.PackagePermission.UseView` | 3 | The current user or group roleset can download a copy of the package from Roblox. |
| `Enum.PackagePermission.Edit` | 4 | The current user or group roleset can download a copy of the package from Roblox and publish package |
| `Enum.PackagePermission.Own` | 5 | The current user or group roleset can download a copy of the page from Roblox, publish package chang |
