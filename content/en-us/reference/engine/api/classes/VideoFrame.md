---
title: VideoFrame
type: class
superclass: GuiObject
---

# VideoFrame

**Inherits from:** `Class.GuiObject` > `Class.GuiBase2d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
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

``Pause()`` → `null`

### `Class.VideoFrame:Play`

``Play()`` → `null`

### `Class.VideoFrame:SetStudioPreview`

``SetStudioPreview(isPreview: `bool`)`` → `null`
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
