---
title: VideoFrame
type: class
superclass: GuiObject
---

# VideoFrame

A GUI object that renders a rectangle, like a `Class.Frame` does, with a
moving video image.

**Inherits from:** `Class.GuiObject` > `Class.GuiBase2d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Description

A VideoFrame renders a rectangle, like a `Class.Frame` does, with a moving
video image. The video must be from a file uploaded to the Roblox website.

The video is scaled to fit the entirety of the rectangle, but looks best when
displayed at its native resolution.

## 2D and 3D Sound

A VideoFrame placed underneath `Class.SurfaceGui` on a `Class.BasePart` will
emit its sound from that part's `Class.BasePart.Position`.

A VideoFrame exhibits the Doppler effect, meaning its frequency and pitch
varies with the relative motion of whatever part it is attached to.

The volume of the VideoFrame will be determined by the distance between the
client's sound listener (by default the `Class.Camera` position) and the
position of the VideoFrame's part.

A VideoFrame is considered **"global"** if it is not placed underneath
SurfaceGui on a BasePart. In this case, the sound will play at the same volume
throughout the entire place.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.VideoFrame.InternalVideoUsage` | `Enum.InternalVideoUsage` | [Hidden] |
| `Class.VideoFrame.IsLoaded` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.VideoFrame.Looped` | `bool` |  |
| `Class.VideoFrame.MaximumResolution` | `Enum.VideoSampleSize` | [Hidden] |
| `Class.VideoFrame.Playing` | `bool` | [NotReplicated] |
| `Class.VideoFrame.Resolution` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] |
| `Class.VideoFrame.RollOffMaxDistance` | `float` |  |
| `Class.VideoFrame.RollOffMinDistance` | `float` |  |
| `Class.VideoFrame.RollOffMode` | `Enum.RollOffMode` |  |
| `Class.VideoFrame.TimeLength` | `double` | [ReadOnly] [NotReplicated] |
| `Class.VideoFrame.TimePosition` | `double` | [NotReplicated] |
| `Class.VideoFrame.Video` | `Datatype.ContentId` |  |
| `Class.VideoFrame.VideoContent` | `Datatype.Content` |  |
| `Class.VideoFrame.Volume` | `float` |  |

## Methods

### `Class.VideoFrame:Pause`

``Pause()`` -> `null`

### `Class.VideoFrame:Play`

``Play()`` -> `null`

### `Class.VideoFrame:SetStudioPreview`

``SetStudioPreview(isPreview: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.VideoFrame.DidLoop`

Fires with: (video: `string`)

### `Class.VideoFrame.Ended`

Fires with: (video: `string`)

### `Class.VideoFrame.Loaded`

Fires with: (video: `string`)

### `Class.VideoFrame.Paused`

Fires with: (video: `string`)

### `Class.VideoFrame.Played`

Fires with: (video: `string`)
