---
title: ContentId
type: datatype
---

# `Datatype.ContentId`

Used in 108 locations across the Roblox API.

## Used as Property Type

- `Class.AdGui.FallbackImage`
- `Class.Animation.AnimationId`
- `Class.AudioPlayer.Asset`
- `Class.BackpackItem.TextureId`
- `Class.BaseScript.LinkedSource`
- `Class.BaseWrap.CageMeshId`
- `Class.BaseWrap.HSRAssetId`
- `Class.Beam.Texture`
- `Class.ClickDetector.CursorIcon`
- `Class.Decal.ColorMap`
- `Class.Decal.MetalnessMap`
- `Class.Decal.NormalMap`
- `Class.Decal.RoughnessMap`
- `Class.Decal.Texture`
- `Class.Decal.TexturePack`
- `Class.DragDetector.ActivatedCursorIcon`
- `Class.FileMesh.MeshId`
- `Class.FileMesh.TextureId`
- `Class.FloorWire.Texture`
- `Class.ImageButton.HoverImage`
- `Class.ImageButton.Image`
- `Class.ImageButton.PressedImage`
- `Class.ImageHandleAdornment.Image`
- `Class.ImageLabel.Image`
- `Class.MaterialVariant.ColorMap`
- `Class.MaterialVariant.MetalnessMap`
- `Class.MaterialVariant.NormalMap`
- `Class.MaterialVariant.RoughnessMap`
- `Class.MeshPart.MeshId`
- `Class.MeshPart.TextureID`
- `Class.ModuleScript.LinkedSource`
- `Class.Mouse.Icon`
- `Class.PackageLink.PackageId`
- `Class.Pants.PantsTemplate`
- `Class.ParticleEmitter.Texture`
- `Class.PluginToolbarButton.Icon`
- `Class.ScreenshotHud.CameraButtonIcon`
- `Class.ScrollingFrame.BottomImage`
- `Class.ScrollingFrame.MidImage`
- `Class.ScrollingFrame.TopImage`
- ...and 26 more

## Used as Parameter Type

- `Class.AnimationClipProvider:GetAnimationClip` (parameter `assetId`)
- `Class.AnimationClipProvider:GetAnimationClipAsync` (parameter `assetId`)
- `Class.AnimationClipProvider:GetClipEvaluatorAsync` (parameter `assetId`)
- `Class.Animator:GetTrackByAnimationId` (parameter `animationId`)
- `Class.CaptureService:UserCaptureSaved` (parameter `captureContentId`)
- `Class.ContentProvider:AssetFetchFailed` (parameter `assetId`)
- `Class.ContentProvider:GetAssetFetchStatus` (parameter `contentId`)
- `Class.ContentProvider:GetAssetFetchStatusChangedSignal` (parameter `contentId`)
- `Class.ContentProvider:Preload` (parameter `contentId`)
- `Class.ContentProvider:RegisterEncryptedAsset` (parameter `assetId`)
- `Class.ContentProvider:RegisterSessionEncryptedAsset` (parameter `contentId`)
- `Class.ContentProvider:UnregisterEncryptedAsset` (parameter `assetId`)
- `Class.DataModel:GetObjects` (parameter `url`)
- `Class.DataModel:GetObjectsAllOrNone` (parameter `url`)
- `Class.DataModel:GetObjectsAsync` (parameter `url`)
- `Class.DataModel:InsertObjectsAndJoinIfLegacyAsync` (parameter `url`)
- `Class.DataModel:Load` (parameter `url`)
- `Class.GeometryService:HashMeshAsync` (parameter `meshId`)
- `Class.HeightmapImporterService:GetHeightmapPreviewAsync` (parameter `heightmapAssetId`)
- `Class.HeightmapImporterService:ImportHeightmap` (parameter `colormapAssetId`)
- `Class.HeightmapImporterService:ImportHeightmap` (parameter `heightmapAssetId`)
- `Class.HeightmapImporterService:IsValidColormap` (parameter `colormapAssetId`)
- `Class.HeightmapImporterService:IsValidHeightmap` (parameter `heightmapAssetId`)
- `Class.InsertService:CreateMeshPartAsync` (parameter `meshId`)
- `Class.InsertService:LoadPackageAssetAsync` (parameter `url`)
- `Class.KeyframeSequenceProvider:GetKeyframeSequence` (parameter `assetId`)
- `Class.KeyframeSequenceProvider:GetKeyframeSequenceAsync` (parameter `assetId`)
- `Class.SafetyService:ScreenshotContentReady` (parameter `contentId`)
- `Class.SoundService:InsertAsset` (parameter `assetId`)
- `Class.StudioAssetService:AutoSetupAvatarAsync` (parameter `modelId`)
- `Class.StudioAssetService:RequestAvatarAutosetupAsync` (parameter `meshId`)
- `Class.StudioAssetService:RequestAvatarAutosetupAsync` (parameter `textureId`)
- `Class.TextService:GetFamilyInfoAsync` (parameter `assetId`)
- `Class.UGCValidationService:FetchAssetWithFormat` (parameter `url`)

## Used as Return Type

- `Class.AnimationClipProvider:RegisterActiveAnimationClip`
- `Class.AnimationClipProvider:RegisterAnimationClip`
- `Class.File:GetTemporaryId`
- `Class.KeyframeSequenceProvider:RegisterActiveKeyframeSequence`
- `Class.KeyframeSequenceProvider:RegisterKeyframeSequence`
- `Class.PublishService:PublishCageMeshAsync`
- `Class.UserInputService:GetImageForKeyCode`
- `Class.ViewportFrame:CaptureSnapshotAsync`
