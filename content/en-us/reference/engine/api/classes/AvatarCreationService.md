---
title: AvatarCreationService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# AvatarCreationService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Methods

### `Class.AvatarCreationService:AutoSetupAvatarAsync`

``AutoSetupAvatarAsync(player: `Class.Player`, autoSetupParams: `Dictionary`, progressCallback: `Datatype.Function`?)`` → `string`
  [Yields]

### `Class.AvatarCreationService:CreateCageMeshPartsWithScaleForExportAsync`

``CreateCageMeshPartsWithScaleForExportAsync(model: `Class.Model`)`` → `Class.Folder`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AvatarCreationService:DeserializeAvatarModel`

``DeserializeAvatarModel(serializedModel: `string`)`` → `Class.Instance`
   {security: RobloxScriptSecurity}

### `Class.AvatarCreationService:GenerateAvatar2DPreviewAsync`

``GenerateAvatar2DPreviewAsync(avatarGeneration2dPreviewParams: `Dictionary`, progressCallback: `Datatype.Function`?)`` → `string`
  [Yields]

### `Class.AvatarCreationService:GenerateAvatarAsync`

``GenerateAvatarAsync(avatarGenerationParams: `Dictionary`, progressCallback: `Datatype.Function`?)`` → `string`
  [Yields]

### `Class.AvatarCreationService:GetBatchTokenDetailsAsync`

``GetBatchTokenDetailsAsync(tokenIds: `Array`)`` → `Array`
  [Yields]

### `Class.AvatarCreationService:GetValidationRules`

``GetValidationRules()`` → `Dictionary`
  [CustomLuaState]

### `Class.AvatarCreationService:HandleSelfieConsentResult`

``HandleSelfieConsentResult(consentAccepted: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarCreationService:HandleSelfieQRResult`

``HandleSelfieQRResult(success: `bool`, resultString: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarCreationService:LoadAvatar2DPreviewAsync`

``LoadAvatar2DPreviewAsync(previewId: `string`)`` → `Class.EditableImage`
  [Yields]

### `Class.AvatarCreationService:LoadGeneratedAvatarAsync`

``LoadGeneratedAvatarAsync(generationId: `string`)`` → `Class.HumanoidDescription`
  [Yields]

### `Class.AvatarCreationService:PrepareAvatarForPreviewAsync`

``PrepareAvatarForPreviewAsync(humanoidModel: `Class.Model`)`` → `null`
  [Yields]

### `Class.AvatarCreationService:PromptCreateAvatarAssetAsync`

``PromptCreateAvatarAssetAsync(tokenId: `string`, player: `Class.Player`, assetInstance: `Class.Instance`, assetType: `Enum.AvatarAssetType`)`` → `Tuple`
  [Yields]

### `Class.AvatarCreationService:PromptCreateAvatarAsync`

``PromptCreateAvatarAsync(tokenId: `string`, player: `Class.Player`, humanoidDescription: `Class.HumanoidDescription`)`` → `Tuple`
  [Yields]

### `Class.AvatarCreationService:PromptSelectAvatarGenerationImageAsync`

``PromptSelectAvatarGenerationImageAsync(player: `Class.Player`)`` → `string`
  [Yields]

### `Class.AvatarCreationService:RequestAvatarGenerationSessionAsync`

``RequestAvatarGenerationSessionAsync(player: `Class.Player`, callback: `Datatype.Function`)`` → `Tuple`
  [Yields]

### `Class.AvatarCreationService:ValidateUGCAccessoryAsync`

``ValidateUGCAccessoryAsync(player: `Class.Player`, accessory: `Class.Instance`, accessoryType: `Enum.AccessoryType`)`` → `Tuple`
  [Yields]

### `Class.AvatarCreationService:ValidateUGCBodyPartAsync`

``ValidateUGCBodyPartAsync(player: `Class.Player`, instance: `Class.Instance`, bodyPart: `Enum.BodyPart`)`` → `Tuple`
  [Yields]

### `Class.AvatarCreationService:ValidateUGCFullBodyAsync`

``ValidateUGCFullBodyAsync(player: `Class.Player`, humanoidDescription: `Class.HumanoidDescription`)`` → `Tuple`
  [Yields]

## Events

### `Class.AvatarCreationService.AvatarAssetModerationCompleted`

Fires with: (assetId: `int64`, moderationStatus: `Enum.ModerationStatus`)

### `Class.AvatarCreationService.AvatarModerationCompleted`

Fires with: (outfitId: `int64`, moderationStatus: `Enum.ModerationStatus`)

### `Class.AvatarCreationService.OpenSelfieConsent`

Fires with: ()

### `Class.AvatarCreationService.OpenSelfieQRCode`

Fires with: (url: `string`, jobId: `string`)

### `Class.AvatarCreationService.UgcValidationFailure`

Fires with: (guid: `string`, errorMessage: `string`)

### `Class.AvatarCreationService.UgcValidationSuccess`

Fires with: (guid: `string`, serializedModel: `string`, price: `int64`)
