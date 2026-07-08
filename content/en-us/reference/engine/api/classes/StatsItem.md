---
title: StatsItem
type: class
superclass: Instance
tags: [NotCreatable]
---

# StatsItem

A single performance metric.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

A StatsItem is an internal measurement item that is created by the engine to
benchmark many of the backend components of Roblox. It cannot be created using
`Datatype.Instance.new()`, but its value can be read by plugins. They can be
found stored inside of the `Class.Stats` service.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.StatsItem.DisplayName` | `string` | [Hidden] [ReadOnly] [NotReplicated] {security: PluginSecurity} |

## Methods

### `Class.StatsItem:GetValue`

``GetValue()`` -> `double`
   {security: PluginSecurity}

### `Class.StatsItem:GetValueString`

``GetValueString()`` -> `string`
   {security: PluginSecurity}
