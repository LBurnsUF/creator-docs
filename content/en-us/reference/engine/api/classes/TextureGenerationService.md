---
title: TextureGenerationService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# TextureGenerationService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **CancelGenerationRequest**(`jobUuid: string`) -> `null`
- **CreatePartGroup**(`instances: Instances`) -> `TextureGenerationPartGroup`
- **GenerateTexture**(`previewJobId: string`) -> `Dictionary`
- **GetQuotasAsync**() -> `Dictionary` [Yields]
- **PreviewTexture**(`partGroup: TextureGenerationPartGroup`, `prompt: string`, `options: Dictionary`) -> `Dictionary`

## Events

- **GenerationNotificationSignal**(`notificationData: Dictionary`)
- **PreviewNotificationSignal**(`notificationData: Dictionary`)
