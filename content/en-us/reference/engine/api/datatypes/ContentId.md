---
title: ContentId
type: datatype
---

# ContentId (DataType)

Used in 108 locations across the API.

## Used as Property Type

- AdGui.FallbackImage
- Animation.AnimationId
- AudioPlayer.Asset
- BackpackItem.TextureId
- BaseScript.LinkedSource
- BaseWrap.CageMeshId
- BaseWrap.HSRAssetId
- Beam.Texture
- ClickDetector.CursorIcon
- Decal.ColorMap
- Decal.MetalnessMap
- Decal.NormalMap
- Decal.RoughnessMap
- Decal.Texture
- Decal.TexturePack
- DragDetector.ActivatedCursorIcon
- FileMesh.MeshId
- FileMesh.TextureId
- FloorWire.Texture
- ImageButton.HoverImage
- ImageButton.Image
- ImageButton.PressedImage
- ImageHandleAdornment.Image
- ImageLabel.Image
- MaterialVariant.ColorMap
- MaterialVariant.MetalnessMap
- MaterialVariant.NormalMap
- MaterialVariant.RoughnessMap
- MeshPart.MeshId
- MeshPart.TextureID
- ...and 36 more

## Used as Parameter Type

- AnimationClipProvider.GetAnimationClip(assetId)
- AnimationClipProvider.GetAnimationClipAsync(assetId)
- AnimationClipProvider.GetClipEvaluatorAsync(assetId)
- Animator.GetTrackByAnimationId(animationId)
- CaptureService.UserCaptureSaved(captureContentId)
- ContentProvider.AssetFetchFailed(assetId)
- ContentProvider.GetAssetFetchStatus(contentId)
- ContentProvider.GetAssetFetchStatusChangedSignal(contentId)
- ContentProvider.Preload(contentId)
- ContentProvider.RegisterEncryptedAsset(assetId)
- ContentProvider.RegisterSessionEncryptedAsset(contentId)
- ContentProvider.UnregisterEncryptedAsset(assetId)
- DataModel.GetObjects(url)
- DataModel.GetObjectsAllOrNone(url)
- DataModel.GetObjectsAsync(url)
- DataModel.InsertObjectsAndJoinIfLegacyAsync(url)
- DataModel.Load(url)
- GeometryService.HashMeshAsync(meshId)
- HeightmapImporterService.GetHeightmapPreviewAsync(heightmapAssetId)
- HeightmapImporterService.ImportHeightmap(colormapAssetId)
- HeightmapImporterService.ImportHeightmap(heightmapAssetId)
- HeightmapImporterService.IsValidColormap(colormapAssetId)
- HeightmapImporterService.IsValidHeightmap(heightmapAssetId)
- InsertService.CreateMeshPartAsync(meshId)
- InsertService.LoadPackageAssetAsync(url)
- KeyframeSequenceProvider.GetKeyframeSequence(assetId)
- KeyframeSequenceProvider.GetKeyframeSequenceAsync(assetId)
- SafetyService.ScreenshotContentReady(contentId)
- SoundService.InsertAsset(assetId)
- StudioAssetService.AutoSetupAvatarAsync(modelId)
- ...and 4 more

## Used as Return Type

- AnimationClipProvider.RegisterActiveAnimationClip
- AnimationClipProvider.RegisterAnimationClip
- File.GetTemporaryId
- KeyframeSequenceProvider.RegisterActiveKeyframeSequence
- KeyframeSequenceProvider.RegisterKeyframeSequence
- PublishService.PublishCageMeshAsync
- UserInputService.GetImageForKeyCode
- ViewportFrame.CaptureSnapshotAsync
