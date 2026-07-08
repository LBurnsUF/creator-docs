---
title: CaptureService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# CaptureService

A service which provides control over screenshot and video capture features.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

`CaptureService` is a client-side service that allows developers to control
how the screenshot and video capture feature integrates with their
experiences. It can be used to include preset moments where a capture is
automatically taken for a user, and that user can then save, share, or delete
the capture.

## Methods

### `Class.CaptureService:CanCaptureVideo`

``CanCaptureVideo()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.CaptureService:CaptureScreenshot`

``CaptureScreenshot(onCaptureReady: `Datatype.Function`)`` -> `null`

### `Class.CaptureService:CheckUploadCaptureStatusAsync`

``CheckUploadCaptureStatusAsync(token: `string`)`` -> `Tuple`
  [Yields]

### `Class.CaptureService:CreatePostAsync`

``CreatePostAsync(pathArr: `Array`, caption: `string`)`` -> `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.CaptureService:DeleteCapture`

``DeleteCapture(capturePath: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.CaptureService:DeleteCapturesAsync`

``DeleteCapturesAsync(pathArr: `Array`)`` -> `int64`
  [Yields] {security: RobloxScriptSecurity}

### `Class.CaptureService:DeleteVideoCapture`

``DeleteVideoCapture(videoCapture: `Class.VideoCapture`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.CaptureService:DeleteVideoCaptureAsync`

``DeleteVideoCaptureAsync(videoCapture: `Class.VideoCapture`)`` -> `bool`
  [Yields] {security: RobloxScriptSecurity}

### `Class.CaptureService:GetCaptureFilePathAsync`

``GetCaptureFilePathAsync(captureContent: `Datatype.Content`)`` -> `string`
  [Yields] {security: RobloxScriptSecurity}

### `Class.CaptureService:GetCaptureSizeAsync`

``GetCaptureSizeAsync(captureContent: `Datatype.Content`)`` -> `Datatype.Vector2`
  [Yields] {security: RobloxScriptSecurity}

### `Class.CaptureService:GetCaptureStorageSizeAsync`

``GetCaptureStorageSizeAsync(pathArr: `Array`)`` -> `int64`
  [Yields] {security: RobloxScriptSecurity}

### `Class.CaptureService:GetCaptureUploadDataAsync`

``GetCaptureUploadDataAsync(capturePath: `string`)`` -> `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.CaptureService:GetDeviceInfo`

``GetDeviceInfo()`` -> `Dictionary`

### `Class.CaptureService:GetScreenshotCaptureObject`

``GetScreenshotCaptureObject(capturePath: `string`)`` -> `Class.Capture`
   {security: RobloxScriptSecurity}

### `Class.CaptureService:InternalCheckPlayabilityAsync`

``InternalCheckPlayabilityAsync(universeId: `int64`)`` -> `bool`
  [Yields]

### `Class.CaptureService:InternalGetStartPlaceIdAsync`

``InternalGetStartPlaceIdAsync(universeId: `int64`)`` -> `int64`
  [Yields]

### `Class.CaptureService:IsCapturingVideo`

``IsCapturingVideo()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.CaptureService:OnCaptureBegan`

``OnCaptureBegan()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.CaptureService:OnCaptureEnded`

``OnCaptureEnded()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.CaptureService:OnCaptureObjectShared`

``OnCaptureObjectShared(capture: `Class.Capture`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.CaptureService:OnCapturePermissionsPromptFinished`

``OnCapturePermissionsPromptFinished(promptId: `int64`, wasAccepted: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.CaptureService:OnCaptureShared`

``OnCaptureShared(capturePath: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.CaptureService:OnSavePromptFinished`

``OnSavePromptFinished(promptId: `int64`, results: `Dictionary`)`` -> `null`
  [CustomLuaState] {security: RobloxScriptSecurity}

### `Class.CaptureService:OnSharePromptFinished`

``OnSharePromptFinished(promptId: `int64`, accepted: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.CaptureService:OnVideoCaptureShared`

``OnVideoCaptureShared(videoCapture: `Class.VideoCapture`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.CaptureService:PreCaptureShared`

``PreCaptureShared(capture: `Class.Capture`)`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.CaptureService:PreVideoCaptureShared`

``PreVideoCaptureShared(videoCapture: `Class.VideoCapture`)`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.CaptureService:PromptCaptureGalleryPermissionAsync`

``PromptCaptureGalleryPermissionAsync(captureGalleryPermission: `Enum.CaptureGalleryPermission`)`` -> `bool`
  [Yields]

### `Class.CaptureService:PromptSaveCapturesToGallery`

``PromptSaveCapturesToGallery(captures: `Array`, resultCallback: `Datatype.Function`)`` -> `null`

### `Class.CaptureService:PromptShareCapture`

``PromptShareCapture(captureContent: `Datatype.Content`, launchData: `string`, onAcceptedCallback: `Datatype.Function`, onDeniedCallback: `Datatype.Function`)`` -> `null`

### `Class.CaptureService:ReadCapturesFromGalleryAsync`

``ReadCapturesFromGalleryAsync(captureTypeFilters: `Array`, readFromAllEligibleExperiences: `bool`)`` -> `Tuple`
  [Yields]

### `Class.CaptureService:RetrieveCaptures`

``RetrieveCaptures()`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.CaptureService:SaveCaptureObjectToExternalStorage`

``SaveCaptureObjectToExternalStorage(capture: `Class.Capture`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.CaptureService:SaveCaptureToExternalStorage`

``SaveCaptureToExternalStorage(capturePath: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.CaptureService:SaveCapturesToExternalStorageAsync`

``SaveCapturesToExternalStorageAsync(pathArr: `Array`)`` -> `int64`
  [Yields] {security: RobloxScriptSecurity}

### `Class.CaptureService:SaveScreenshotCapture`

``SaveScreenshotCapture(additionalInfo: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.CaptureService:SaveVideoCaptureToExternalStorage`

``SaveVideoCaptureToExternalStorage(videoCapture: `Class.VideoCapture`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.CaptureService:StartUploadCaptureAsync`

``StartUploadCaptureAsync(capture: `Class.Capture`)`` -> `Tuple`
  [Yields]

### `Class.CaptureService:StartVideoCaptureAsync`

``StartVideoCaptureAsync(onCaptureReady: `Datatype.Function`, captureParams: `Dictionary`)`` -> `Enum.VideoCaptureStartedResult`
  [Yields]

### `Class.CaptureService:StartVideoCaptureInternalAsync`

``StartVideoCaptureInternalAsync()`` -> `Enum.VideoCaptureStartedResult`
  [Yields] {security: RobloxScriptSecurity}

### `Class.CaptureService:StopVideoCapture`

``StopVideoCapture()`` -> `null`

### `Class.CaptureService:StopVideoCaptureInternal`

``StopVideoCaptureInternal()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.CaptureService:TakeScreenshotCaptureAsync`

``TakeScreenshotCaptureAsync(onCaptureReady: `Datatype.Function`, captureParams: `Dictionary`)`` -> `null`

### `Class.CaptureService:UploadCaptureAndPostMoment`

``UploadCaptureAndPostMoment(capture: `Class.Capture`, momentMetadata: `Dictionary`, feedRegistrationInfo: `Dictionary`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.CaptureService:UploadCaptureAsync`

``UploadCaptureAsync(capture: `Class.Capture`)`` -> `Tuple`
  [Yields]

## Events

### `Class.CaptureService.CaptureBegan`

Fires with: (captureType: `Enum.CaptureType`)

### `Class.CaptureService.CaptureEnded`

Fires with: (captureType: `Enum.CaptureType`)

### `Class.CaptureService.CaptureObjectSavedInternal`

Fires with: (capture: `Class.Capture`, triggerSource: `string`)

### `Class.CaptureService.CaptureSaved`

Fires with: (captureInfo: `Dictionary`)
  [Deprecated]

### `Class.CaptureService.CaptureSavedInternal`

Fires with: (captureInfo: `Dictionary`, triggerSource: `string`)

### `Class.CaptureService.OpenCapturePermissionsPrompt`

Fires with: (promptId: `int64`, captureGalleryPermission: `Enum.CaptureGalleryPermission`)

### `Class.CaptureService.OpenSaveCapturesPrompt`

Fires with: (promptId: `int64`, captures: `Array`)

### `Class.CaptureService.OpenShareCapturePrompt`

Fires with: (promptId: `int64`, captureContent: `Variant`, launchData: `string`)

### `Class.CaptureService.UserCaptureSaved`

Fires with: (captureContentId: `Datatype.ContentId`)

### `Class.CaptureService.UserVideoCaptureFailed`

Fires with: (result: `Enum.VideoCaptureResult`)

### `Class.CaptureService.UserVideoCaptureStartFailed`

Fires with: (result: `Enum.VideoCaptureStartedResult`)

### `Class.CaptureService.VideoCaptureInProgress`

Fires with: (isInProgress: `bool`, captureTrigger: `string`)
