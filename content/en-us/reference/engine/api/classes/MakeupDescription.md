---
title: MakeupDescription
type: class
superclass: Instance
---

# MakeupDescription

Describes the appearance of a makeup item for the `Class.HumanoidDescription`.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`MakeupDescription` is an object that stores the description for a makeup
item. It is meant to be placed underneath a `Class.HumanoidDescription` in
order to work with `Class.Humanoid:ApplyDescriptionAsync()`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.MakeupDescription.AssetId` | `int64` |  |
| `Class.MakeupDescription.Instance` | `Class.Instance` |  |
| `Class.MakeupDescription.MakeupType` | `Enum.MakeupType` |  |
| `Class.MakeupDescription.Order` | `int` |  |

## Methods

### `Class.MakeupDescription:GetAppliedInstance`

``GetAppliedInstance()`` -> `Class.Instance`
