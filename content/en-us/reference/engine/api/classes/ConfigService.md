---
title: ConfigService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ConfigService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.ConfigService:ClearTestingValue`

``ClearTestingValue(key: `string`)`` → `null`

### `Class.ConfigService:GetConfigAsync`

``GetConfigAsync()`` → `Class.ConfigSnapshot`
  [Yields]

### `Class.ConfigService:GetConfigForPlayerAsync`

``GetConfigForPlayerAsync(player: `Class.Player`)`` → `Class.ConfigSnapshot`
  [Yields]

### `Class.ConfigService:SetTestingValue`

``SetTestingValue(key: `string`, value: `Variant`)`` → `null`
