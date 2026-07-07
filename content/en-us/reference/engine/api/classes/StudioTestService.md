---
title: StudioTestService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# StudioTestService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.StudioTestService.EditModeActive` | `bool` |  {security: PluginSecurity} |

## Methods

### `Class.StudioTestService:AddPlayers`

``AddPlayers(numPlayers: `int`)`` → `null`

### `Class.StudioTestService:CanLeaveTest`

``CanLeaveTest()`` → `bool`

### `Class.StudioTestService:EndTest`

``EndTest(value: `Variant`)`` → `null`

### `Class.StudioTestService:ExecuteMultiplayerTestAsync`

``ExecuteMultiplayerTestAsync(numPlayers: `int`, args: `Variant`)`` → `Variant`
  [Yields] {security: PluginSecurity}

### `Class.StudioTestService:ExecutePlayModeAsync`

``ExecutePlayModeAsync(args: `Variant`)`` → `Variant`
  [Yields] {security: PluginSecurity}

### `Class.StudioTestService:ExecuteRunModeAsync`

``ExecuteRunModeAsync(args: `Variant`)`` → `Variant`
  [Yields] {security: PluginSecurity}

### `Class.StudioTestService:GetTestArgs`

``GetTestArgs()`` → `Variant`

### `Class.StudioTestService:LeaveTest`

``LeaveTest()`` → `null`
