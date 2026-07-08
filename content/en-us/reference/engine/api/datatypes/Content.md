---
title: Content
type: datatype
---

# `Datatype.Content`

Represents a reference to asset content stored externally or as an object
within the place.

## Description

The `Content` data type represents a reference to asset content stored
externally or as an object within the place, wrapping a single value of one of
the supported `Enum.ContentSourceType` values.

##### Warning

Replication is not yet supported for `Datatype.Content.Object|Object` values.
When an `Class.Instance` with a `Datatype.Content` property containing a
`Datatype.Content.Object|Object` value is replicated, an unusable placeholder
`Class.Object` of the same type will be used instead of the `Class.Object`
itself, and any attempt to read or write the contents of that placeholder
object will throw. These placeholder objects will render as a cyan and magenta
checkerboard pattern.

This will be replaced with standard replication behavior in the future. For
now, do not use `Class.EditableImage` or `Class.EditableMesh` as
`Datatype.Content` on the server on an `Class.Instance` that can replicate to
clients.

## Constructors

### `Content.fromUri`

Returns a new `Content` with an [asset URI](../../../projects/assets/index.md#asset-uris) `string` value referencing content external to the place.

`Datatype.Content.SourceType` will be `Enum.ContentSourceType|Uri`, and `Datatype.Content.Uri` will contain a non‑`nil` `string` value.

If `uri` is empty, `Datatype.Content.none` will be returned instead.

**Parameters:**

- `uri`: `string` - The [asset URI](../../../projects/assets/index.md#asset-uris) string.

### `Content.fromAssetId`

Returns a new `Content` from a numeric asset ID. This is a convenience
constructor equivalent to calling
`Content.fromUri("rbxassetid://" .. tostring(assetId))`.

`Datatype.Content.SourceType` will be `Enum.ContentSourceType|Uri`, and
`Datatype.Content.Uri` will contain the formatted `rbxassetid://` URI string.

If `assetId` is `0`, `Datatype.Content.none` will be returned instead.

Throws if `assetId` is non‑finite, for example `Library.math.huge()` or `0/0`.

**Parameters:**

- `assetId`: `number` - The numeric asset ID.

### `Content.fromObject`

Returns a new `Content` with a strong reference to an `Class.Object`.

`Datatype.Content.SourceType` will be `Enum.ContentSourceType|Object`, and `Datatype.Content.Object` will contain a non‑`nil` `Class.Object` reference.

`Datatype.Content.Object` references are **strong** references that hold **shared ownership** of the `Class.Object`. Any `Datatype.Content.Object` reference will extend the lifetime of that `Class.Object` and prevent it from being garbage collected.

Throws if `object` is `nil`.

**Parameters:**

- `object`: `Object` - The `Class.Object` to reference.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Content.none` | `Content` | An empty `Content` value with `Datatype.Content.SourceType` of `Enum.ContentSourceType/None`. |
| `Content.SourceType` | `Enum.ContentSourceType` | The source type of the contained value. |
| `Content.Uri` | `string?` | A URI `string` if `Datatype.Content.SourceType` is `Enum.ContentSourceType/Uri`, otherwise `nil`. |
| `Content.Object` | `Object?` | A reference to a non-`nil` `Class.Object` if `Datatype.Content.SourceType` is `Enum.ContentSourceTyp |
| `Content.Opaque` | `Opaque?` | A reference to a non-`nil` `Opaque` content if `Datatype.Content.SourceType` is `Enum.ContentSourceT |

## API Usage (82 locations)

### Used as Property Type

- `Class.AdGui.FallbackImageContent`
- `Class.Animation.AnimationContent`
- `Class.AudioPlayer.AudioContent`
- `Class.BackpackItem.TextureContent`
- `Class.BaseWrap.CageMeshContent`
- `Class.Beam.TextureContent`
- `Class.CharacterMesh.BaseTextureContent`
- `Class.CharacterMesh.MeshContent`
- `Class.CharacterMesh.OverlayTextureContent`
- `Class.ClickDetector.CursorIconContent`
- `Class.Decal.ColorMapContent`
- `Class.Decal.MetalnessMapContent`
- `Class.Decal.NormalMapContent`
- `Class.Decal.RoughnessMapContent`
- `Class.Decal.TextureContent`
- `Class.DragDetector.ActivatedCursorIconContent`
- `Class.FileMesh.MeshContent`
- `Class.FileMesh.TextureContent`
- `Class.ImageButton.HoverImageContent`
- `Class.ImageButton.ImageContent`
- `Class.ImageButton.PressedImageContent`
- `Class.ImageHandleAdornment.ImageContent`
- `Class.ImageLabel.ImageContent`
- `Class.MaterialVariant.ColorMapContent`
- `Class.MaterialVariant.EmissiveMaskContent`
- `Class.MaterialVariant.MetalnessMapContent`
- `Class.MaterialVariant.NormalMapContent`
- `Class.MaterialVariant.RoughnessMapContent`
- `Class.MeshPart.MeshContent`
- `Class.MeshPart.TextureContent`
- `Class.Mouse.IconContent`
- `Class.PackageLink.PackageContent`
- `Class.Pants.PantsTemplateContent`
- `Class.ParticleEmitter.TextureContent`
- `Class.PluginToolbarButton.IconContent`
- `Class.ScreenshotHud.CameraButtonIconContent`
- `Class.ScrollingFrame.BottomImageContent`
- `Class.ScrollingFrame.MidImageContent`
- `Class.ScrollingFrame.TopImageContent`
- `Class.Shirt.ShirtTemplateContent`
- ...and 29 more

### Used as Parameter Type

- `Class.AssetService:CanEditAssetAsync` (parameter `content`)
- `Class.AssetService:CreateDataModelContentAsync` (parameter `content`)
- `Class.AssetService:CreateEditableImageAsync` (parameter `content`)
- `Class.AssetService:CreateEditableMeshAsync` (parameter `content`)
- `Class.AssetService:CreateMeshPartAsync` (parameter `meshContent`)
- `Class.AssetService:GetOpaqueContentMetadataMap` (parameter `opaqueContent`)
- `Class.CaptureService:GetCaptureFilePathAsync` (parameter `captureContent`)
- `Class.CaptureService:GetCaptureSizeAsync` (parameter `captureContent`)
- `Class.CaptureService:PromptShareCapture` (parameter `captureContent`)
- `Class.ModerationService:CreateReviewableContentKey` (parameter `content`)
- `Class.VideoService:CreateVideoSamplerAsync` (parameter `content`)
- `Class.WrapDeformer:SetCageMeshContent` (parameter `content`)

### Used as Return Type

- `Class.AudioRecorder:GetTemporaryContent`
