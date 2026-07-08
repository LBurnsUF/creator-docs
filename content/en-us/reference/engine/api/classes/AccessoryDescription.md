---
title: AccessoryDescription
type: class
superclass: Instance
---

# AccessoryDescription

Describes the appearance of an `Class.Accessory` for the
`Class.HumanoidDescription`.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

**AccessoryDescription** is an object that stores the description for an
`Class.Accessory`. It is meant to be placed underneath a
`Class.HumanoidDescription` in order to work with
`Class.Humanoid:ApplyDescriptionAsync()`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AccessoryDescription.AccessoryType` | `Enum.AccessoryType` |  |
| `Class.AccessoryDescription.AssetId` | `int64` |  |
| `Class.AccessoryDescription.Instance` | `Class.Instance` |  |
| `Class.AccessoryDescription.IsLayered` | `bool` |  |
| `Class.AccessoryDescription.Order` | `int` |  |
| `Class.AccessoryDescription.Position` | `Datatype.Vector3` |  |
| `Class.AccessoryDescription.Puffiness` | `float` | [Deprecated] |
| `Class.AccessoryDescription.Rotation` | `Datatype.Vector3` |  |
| `Class.AccessoryDescription.Scale` | `Datatype.Vector3` |  |

## Methods

### `Class.AccessoryDescription:GetAppliedInstance`

``GetAppliedInstance()`` -> `Class.Instance`
