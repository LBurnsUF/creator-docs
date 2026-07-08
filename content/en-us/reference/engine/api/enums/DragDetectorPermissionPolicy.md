---
title: DragDetectorPermissionPolicy
type: enum
---

# `Enum.DragDetectorPermissionPolicy`

Used to control the permission level for which players can interact with a
`Class.DragDetector`.

Used to control the permission level for which players can interact with a
`Class.DragDetector` through its
`Class.DragDetector.PermissionPolicy|PermissionPolicy` property.

The `Enum.DragDetectorPermissionPolicy` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.DragDetectorPermissionPolicy.Nobody` | 0 | No players can interact with the `Class.DragDetector`. |
| `Enum.DragDetectorPermissionPolicy.Everybody` | 1 | All players can interact with the `Class.DragDetector`. |
| `Enum.DragDetectorPermissionPolicy.Scriptable` | 2 | Invokes the function registered via `Class.DragDetector:SetPermissionPolicyFunction()`, enabling/dis |
