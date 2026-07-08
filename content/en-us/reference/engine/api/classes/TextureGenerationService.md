---
title: TextureGenerationService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# TextureGenerationService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.TextureGenerationService:CancelGenerationRequest`

``CancelGenerationRequest(jobUuid: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.TextureGenerationService:CreatePartGroup`

``CreatePartGroup(instances: `Datatype.Instances`)`` -> `Class.TextureGenerationPartGroup`
   {security: RobloxScriptSecurity}

### `Class.TextureGenerationService:GenerateTexture`

``GenerateTexture(previewJobId: `string`)`` -> `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.TextureGenerationService:GetQuotasAsync`

``GetQuotasAsync()`` -> `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.TextureGenerationService:PreviewTexture`

``PreviewTexture(partGroup: `Class.TextureGenerationPartGroup`, prompt: `string`, options: `Dictionary`)`` -> `Dictionary`
   {security: RobloxScriptSecurity}

## Events

### `Class.TextureGenerationService.GenerationNotificationSignal`

Fires with: (notificationData: `Dictionary`)

### `Class.TextureGenerationService.PreviewNotificationSignal`

Fires with: (notificationData: `Dictionary`)
