---
title: ConfigService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ConfigService

A game service that gives access to in-experience configuration with updates
in real time.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

**ConfigService** exposes methods for getting `Class.ConfigSnapshot` objects.
Configs can only be accessed by game servers, so you can't use
`Class.ConfigService` within client scripts.

See [Experience configs](../../../production/configs.md) for an in-depth guide
on managing keys, deploying real-time updates, error handling, limits, and
more.

## Methods

### `Class.ConfigService:ClearTestingValue`

``ClearTestingValue(key: `string`)`` -> `null`

### `Class.ConfigService:GetConfigAsync`

``GetConfigAsync()`` -> `Class.ConfigSnapshot`
  [Yields]

### `Class.ConfigService:GetConfigForPlayerAsync`

``GetConfigForPlayerAsync(player: `Class.Player`)`` -> `Class.ConfigSnapshot`
  [Yields]

### `Class.ConfigService:SetTestingValue`

``SetTestingValue(key: `string`, value: `Variant`)`` -> `null`
