---
title: TeleportOptions
type: class
superclass: Instance
---

# TeleportOptions

Optional input arguments to the `Class.TeleportService:TeleportAsync()`
function.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

This class is an optional parameter to the
`Class.TeleportService:TeleportAsync()` function that allows developers to
provide arguments for the teleport call.

Certain arguments in this class are not compatible with each other and cause
an error when passed to `Class.TeleportService:TeleportAsync()`:

- ReservedServerAccessCode + ServerInstanceId
- ShouldReserveServer + ServerInstanceId
- ShouldReserveServer + ReservedServerAccessCode

For more information on how to teleport players between servers, see
[Teleporting Between Places](../../../projects/teleport.md).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.TeleportOptions.ReservedServerAccessCode` | `string` |  |
| `Class.TeleportOptions.ServerInstanceId` | `string` |  |
| `Class.TeleportOptions.ShouldReserveServer` | `bool` |  |

## Methods

### `Class.TeleportOptions:GetTeleportData`

``GetTeleportData()`` -> `Variant`

### `Class.TeleportOptions:SetTeleportData`

``SetTeleportData(teleportData: `Variant`)`` -> `null`
