---
title: AvatarCreationService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# AvatarCreationService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **AutoSetupAvatarAsync**(`player: Player`, `autoSetupParams: Dictionary`, `progressCallback: Function?`) -> `string` [Yields]
- **CreateCageMeshPartsWithScaleForExportAsync**(`model: Model`) -> `Folder` [Yields]
- **DeserializeAvatarModel**(`serializedModel: string`) -> `Instance`
- **GenerateAvatar2DPreviewAsync**(`avatarGeneration2dPreviewParams: Dictionary`, `progressCallback: Function?`) -> `string` [Yields]
- **GenerateAvatarAsync**(`avatarGenerationParams: Dictionary`, `progressCallback: Function?`) -> `string` [Yields]
- **GetBatchTokenDetailsAsync**(`tokenIds: Array`) -> `Array` [Yields]
- **GetValidationRules**() -> `Dictionary` [CustomLuaState]
- **HandleSelfieConsentResult**(`consentAccepted: bool`) -> `null`
- **HandleSelfieQRResult**(`success: bool`, `resultString: string`) -> `null`
- **LoadAvatar2DPreviewAsync**(`previewId: string`) -> `EditableImage` [Yields]
- **LoadGeneratedAvatarAsync**(`generationId: string`) -> `HumanoidDescription` [Yields]
- **PrepareAvatarForPreviewAsync**(`humanoidModel: Model`) -> `null` [Yields]
- **PromptCreateAvatarAssetAsync**(`tokenId: string`, `player: Player`, `assetInstance: Instance`, `assetType: AvatarAssetType`) -> `Tuple` [Yields]
- **PromptCreateAvatarAsync**(`tokenId: string`, `player: Player`, `humanoidDescription: HumanoidDescription`) -> `Tuple` [Yields]
- **PromptSelectAvatarGenerationImageAsync**(`player: Player`) -> `string` [Yields]
- **RequestAvatarGenerationSessionAsync**(`player: Player`, `callback: Function`) -> `Tuple` [Yields]
- **ValidateUGCAccessoryAsync**(`player: Player`, `accessory: Instance`, `accessoryType: AccessoryType`) -> `Tuple` [Yields]
- **ValidateUGCBodyPartAsync**(`player: Player`, `instance: Instance`, `bodyPart: BodyPart`) -> `Tuple` [Yields]
- **ValidateUGCFullBodyAsync**(`player: Player`, `humanoidDescription: HumanoidDescription`) -> `Tuple` [Yields]

## Events

- **AvatarAssetModerationCompleted**(`assetId: int64`, `moderationStatus: ModerationStatus`)
- **AvatarModerationCompleted**(`outfitId: int64`, `moderationStatus: ModerationStatus`)
- **OpenSelfieConsent**()
- **OpenSelfieQRCode**(`url: string`, `jobId: string`)
- **UgcValidationFailure**(`guid: string`, `errorMessage: string`)
- **UgcValidationSuccess**(`guid: string`, `serializedModel: string`, `price: int64`)
