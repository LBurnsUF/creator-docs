---
title: MLService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# MLService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.MLService:CreateSessionAsync`

``CreateSessionAsync(assetId: `string`)`` → `Class.MLSession`
  [Yields]

### `Class.MLService:GetNPCInferenceSpecAsync`

``GetNPCInferenceSpecAsync(server: `string`, port: `int`)`` → `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.MLService:IsPostProcessReady`

``IsPostProcessReady()`` → `bool`

### `Class.MLService:LoadPostProcessModelAsync`

``LoadPostProcessModelAsync(assetId: `int64`)`` → `null`
  [Yields]

### `Class.MLService:RunNPCInferenceAsync`

``RunNPCInferenceAsync(server: `string`, port: `int`, features: `Dictionary`)`` → `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.MLService:SetPostProcessEnabled`

``SetPostProcessEnabled(enabled: `bool`)`` → `null`
