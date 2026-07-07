---
title: SoundService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# SoundService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.SoundService.AcousticSimulationEnabled` | `bool` |  |
| `Class.SoundService.AmbientReverb` | `Enum.ReverbType` |  |
| `Class.SoundService.AudioApiByDefault` | `Enum.RolloutState` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.SoundService.CharacterSoundsUseNewApi` | `Enum.RolloutState` |  {write: PluginSecurity} |
| `Class.SoundService.DefaultListenerLocation` | `Enum.ListenerLocation` |  {security: PluginSecurity} |
| `Class.SoundService.DiffractionEnabled` | `bool` |  |
| `Class.SoundService.DistanceFactor` | `float` |  |
| `Class.SoundService.DopplerScale` | `float` |  |
| `Class.SoundService.IsNewExpForAudioApiByDefault` | `bool` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.SoundService.ListenerCFrame` | `Datatype.CFrame` |  |
| `Class.SoundService.ListenerObject` | `Class.Instance` |  |
| `Class.SoundService.ListenerType` | `Enum.ListenerType` |  |
| `Class.SoundService.OcclusionEnabled` | `bool` |  |
| `Class.SoundService.RespectFilteringEnabled` | `bool` |  |
| `Class.SoundService.ReverbEnabled` | `bool` |  |
| `Class.SoundService.RolloffScale` | `float` |  |
| `Class.SoundService.VolumetricAudio` | `Enum.VolumetricAudio` | [NotScriptable] |

## Methods

### `Class.SoundService:BeginRecording`

``BeginRecording()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.SoundService:EndRecording`

``EndRecording()`` → `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.SoundService:GetAudioApiByDefault`

``GetAudioApiByDefault()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.SoundService:GetAudioInstances`

``GetAudioInstances()`` → `Array`
   {security: RobloxScriptSecurity}

### `Class.SoundService:GetInputDevice`

``GetInputDevice()`` → `Tuple`
   {security: RobloxScriptSecurity}

### `Class.SoundService:GetInputDevices`

``GetInputDevices()`` → `Tuple`
   {security: RobloxScriptSecurity}

### `Class.SoundService:GetListener`

``GetListener()`` → `Tuple`

### `Class.SoundService:GetMixerTime`

``GetMixerTime()`` → `double`

### `Class.SoundService:GetOutputDevice`

``GetOutputDevice()`` → `Tuple`
   {security: RobloxScriptSecurity}

### `Class.SoundService:GetOutputDevices`

``GetOutputDevices()`` → `Tuple`
   {security: RobloxScriptSecurity}

### `Class.SoundService:GetRecordingDevices`

``GetRecordingDevices()`` → `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.SoundService:GetSoundMemoryData`

``GetSoundMemoryData()`` → `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.SoundService:InsertAsset`

``InsertAsset(assetId: `Datatype.ContentId`, assetName: `string`, useSelection: `bool`)`` → `Datatype.Instances`
   {security: RobloxScriptSecurity}

### `Class.SoundService:OpenAttenuationCurveEditor`

``OpenAttenuationCurveEditor(selectedCurveObjects: `Datatype.Instances`)`` → `null`
   {security: PluginSecurity}

### `Class.SoundService:OpenDirectionalCurveEditor`

``OpenDirectionalCurveEditor(selectedCurveObjects: `Datatype.Instances`)`` → `null`
   {security: PluginSecurity}

### `Class.SoundService:PlayLocalSound`

``PlayLocalSound(sound: `Class.Instance`)`` → `null`

### `Class.SoundService:SetAudioApiByDefault`

``SetAudioApiByDefault(enabled: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SoundService:SetInputDevice`

``SetInputDevice(nameOrInstance: `Variant`, guidOrPin: `string`)`` → `null`

### `Class.SoundService:SetListener`

``SetListener(listenerType: `Enum.ListenerType`, listener: `Tuple`)`` → `null`

### `Class.SoundService:SetOutputDevice`

``SetOutputDevice(name: `string`, guid: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SoundService:SetRecordingDevice`

``SetRecordingDevice(deviceIndex: `int`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.SoundService:SetSoundEnabled`

``SetSoundEnabled(enabled: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.SoundService.AudioInstanceAdded`

Fires with: (instance: `Class.Instance`)

### `Class.SoundService.DeviceListChanged`

Fires with: (newDevices: `Tuple`)

### `Class.SoundService.OpenAttenuationCurveEditorSignal`

Fires with: (selectedCurveObjects: `Datatype.Instances`)

### `Class.SoundService.OpenAudioCompressorEditorSignal`

Fires with: (selectedCompressorObjects: `Datatype.Instances`)

### `Class.SoundService.OpenAudioEqualizerEditorSignal`

Fires with: (selectedEqualizerObjects: `Datatype.Instances`)

### `Class.SoundService.OpenDirectionalCurveEditorSignal`

Fires with: (selectedCurveObjects: `Datatype.Instances`)
