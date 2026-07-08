---
title: HopperBin
type: class
superclass: BackpackItem
tags: [Deprecated]
---

# HopperBin

**Inherits from:** `Class.BackpackItem` > `Class.Model` > `Class.PVInstance` > `Class.Instance` > `Class.Object`

**Tags:** [Deprecated]

## Description

HopperBins are an outdated system for creating tools that can be used by a
player. In place of HopperBins, please use `Class.Tool` instead.

Historically, only HopperBins worked without a 'Handle' `Class.Part`, but this
is no longer the case thanks to the `Class.Tool.RequiresHandle` property of
Tools.

> **Deprecated:** This deprecated class has been replaced by `Class.Tool`. Please use Tool for
new work instead.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.HopperBin.Active` | `bool` |  |
| `Class.HopperBin.BinType` | `Enum.BinType` |  |

## Methods

### `Class.HopperBin:Disable`

``Disable()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.HopperBin:ToggleSelect`

``ToggleSelect()`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.HopperBin.Deselected`

Fires with: ()

### `Class.HopperBin.Selected`

Fires with: (mouse: `Class.Instance`)
