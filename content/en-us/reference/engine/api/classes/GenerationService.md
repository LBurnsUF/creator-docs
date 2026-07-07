---
title: GenerationService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# GenerationService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Methods

### `Class.GenerationService:ConnectAsync`

``ConnectAsync(sessionId: `string`, sdp: `string`, type: `string`, relay: `string`)`` → `Tuple`
  [Yields]

### `Class.GenerationService:DisconnectAsync`

``DisconnectAsync(sessionId: `string`)`` → `bool`
  [Yields]

### `Class.GenerationService:GenerateMeshAsync`

``GenerateMeshAsync(inputs: `Dictionary`, player: `Class.Player`, options: `Dictionary`, intermediateResultCallback: `Datatype.Function`?)`` → `Tuple`
  [Yields]

### `Class.GenerationService:GenerateModelAsync`

``GenerateModelAsync(inputs: `Dictionary`, schema: `Dictionary`, options: `Dictionary?`)`` → `Tuple`
  [Yields]

### `Class.GenerationService:GetVideoGenSessionAsync`

``GetVideoGenSessionAsync()`` → `Tuple`
  [Yields]

### `Class.GenerationService:GetVideoGenTriggersAsync`

``GetVideoGenTriggersAsync(sessionId: `string`, lookbackSeconds: `int`)`` → `Dictionary`
  [Yields]

### `Class.GenerationService:InternalGenerateMeshAsync`

``InternalGenerateMeshAsync(inputs: `Dictionary`, userId: `int64`, options: `Dictionary`, intermediateResultCallback: `Datatype.Function`?)`` → `Tuple`
  [Yields] {security: RobloxScriptSecurity}

### `Class.GenerationService:LoadGeneratedMeshAsync`

``LoadGeneratedMeshAsync(generationId: `string`)`` → `Class.MeshPart`
  [Yields]

### `Class.GenerationService:LoadModelFromGlbAsync`

``LoadModelFromGlbAsync(glbPath: `string`)`` → `Class.Model`
  [Yields] {security: RobloxScriptSecurity}

### `Class.GenerationService:StartVideoGenSessionAsync`

``StartVideoGenSessionAsync(sessionId: `string`, prompt: `string`, imageData: `string`, imageS3Reference: `string`, triggers: `Dictionary`)`` → `bool`
  [Yields]

### `Class.GenerationService:UpdateVideoGenSessionPromptAsync`

``UpdateVideoGenSessionPromptAsync(sessionId: `string`, prompt: `string`, imageData: `string`, imageS3Reference: `string`, mode: `string`)`` → `bool`
  [Yields]

### `Class.GenerationService:UpdateVideoGenSessionTriggersAsync`

``UpdateVideoGenSessionTriggersAsync(sessionId: `string`, triggers: `Dictionary`)`` → `bool`
  [Yields]
