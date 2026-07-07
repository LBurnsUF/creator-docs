---
title: CaptureService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# CaptureService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **CanCaptureVideo**() -> `bool`
- **CaptureScreenshot**(`onCaptureReady: Function`) -> `null`
- **CheckUploadCaptureStatusAsync**(`token: string`) -> `Tuple` [Yields]
- **CreatePostAsync**(`pathArr: Array`, `caption: string`) -> `Dictionary` [Yields]
- **DeleteCapture**(`capturePath: string`) -> `null`
- **DeleteCapturesAsync**(`pathArr: Array`) -> `int64` [Yields]
- **DeleteVideoCapture**(`videoCapture: VideoCapture`) -> `null`
- **DeleteVideoCaptureAsync**(`videoCapture: VideoCapture`) -> `bool` [Yields]
- **GetCaptureFilePathAsync**(`captureContent: Content`) -> `string` [Yields]
- **GetCaptureSizeAsync**(`captureContent: Content`) -> `Vector2` [Yields]
- **GetCaptureStorageSizeAsync**(`pathArr: Array`) -> `int64` [Yields]
- **GetCaptureUploadDataAsync**(`capturePath: string`) -> `Dictionary` [Yields]
- **GetDeviceInfo**() -> `Dictionary`
- **GetScreenshotCaptureObject**(`capturePath: string`) -> `Capture`
- **InternalCheckPlayabilityAsync**(`universeId: int64`) -> `bool` [Yields]
- **InternalGetStartPlaceIdAsync**(`universeId: int64`) -> `int64` [Yields]
- **IsCapturingVideo**() -> `bool`
- **OnCaptureBegan**() -> `null`
- **OnCaptureEnded**() -> `null`
- **OnCaptureObjectShared**(`capture: Capture`) -> `null`
- **OnCapturePermissionsPromptFinished**(`promptId: int64`, `wasAccepted: bool`) -> `null`
- **OnCaptureShared**(`capturePath: string`) -> `null`
- **OnSavePromptFinished**(`promptId: int64`, `results: Dictionary`) -> `null` [CustomLuaState]
- **OnSharePromptFinished**(`promptId: int64`, `accepted: bool`) -> `null`
- **OnVideoCaptureShared**(`videoCapture: VideoCapture`) -> `null`
- **PreCaptureShared**(`capture: Capture`) -> `string`
- **PreVideoCaptureShared**(`videoCapture: VideoCapture`) -> `string`
- **PromptCaptureGalleryPermissionAsync**(`captureGalleryPermission: CaptureGalleryPermission`) -> `bool` [Yields]
- **PromptSaveCapturesToGallery**(`captures: Array`, `resultCallback: Function`) -> `null`
- **PromptShareCapture**(`captureContent: Content`, `launchData: string`, `onAcceptedCallback: Function`, `onDeniedCallback: Function`) -> `null`
- **ReadCapturesFromGalleryAsync**(`captureTypeFilters: Array = {}`, `readFromAllEligibleExperiences: bool = false`) -> `Tuple` [Yields]
- **RetrieveCaptures**() -> `Array`
- **SaveCaptureObjectToExternalStorage**(`capture: Capture`) -> `null`
- **SaveCaptureToExternalStorage**(`capturePath: string`) -> `null`
- **SaveCapturesToExternalStorageAsync**(`pathArr: Array`) -> `int64` [Yields]
- **SaveScreenshotCapture**(`additionalInfo: string = `) -> `null`
- **SaveVideoCaptureToExternalStorage**(`videoCapture: VideoCapture`) -> `null`
- **StartUploadCaptureAsync**(`capture: Capture`) -> `Tuple` [Yields]
- **StartVideoCaptureAsync**(`onCaptureReady: Function`, `captureParams: Dictionary = nil`) -> `VideoCaptureStartedResult` [Yields]
- **StartVideoCaptureInternalAsync**() -> `VideoCaptureStartedResult` [Yields]
- **StopVideoCapture**() -> `null`
- **StopVideoCaptureInternal**() -> `null`
- **TakeScreenshotCaptureAsync**(`onCaptureReady: Function`, `captureParams: Dictionary = nil`) -> `null`
- **UploadCaptureAndPostMoment**(`capture: Capture`, `momentMetadata: Dictionary = nil`, `feedRegistrationInfo: Dictionary = nil`) -> `null`
- **UploadCaptureAsync**(`capture: Capture`) -> `Tuple` [Yields]

## Events

- **CaptureBegan**(`captureType: CaptureType`)
- **CaptureEnded**(`captureType: CaptureType`)
- **CaptureObjectSavedInternal**(`capture: Capture`, `triggerSource: string`)
- **CaptureSaved**(`captureInfo: Dictionary`) [Deprecated]
- **CaptureSavedInternal**(`captureInfo: Dictionary`, `triggerSource: string`)
- **OpenCapturePermissionsPrompt**(`promptId: int64`, `captureGalleryPermission: CaptureGalleryPermission`)
- **OpenSaveCapturesPrompt**(`promptId: int64`, `captures: Array`)
- **OpenShareCapturePrompt**(`promptId: int64`, `captureContent: Variant`, `launchData: string`)
- **UserCaptureSaved**(`captureContentId: ContentId`)
- **UserVideoCaptureFailed**(`result: VideoCaptureResult`)
- **UserVideoCaptureStartFailed**(`result: VideoCaptureStartedResult`)
- **VideoCaptureInProgress**(`isInProgress: bool`, `captureTrigger: string`)
