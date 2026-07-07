---
title: SoundService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# SoundService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Properties

- **AcousticSimulationEnabled**: `bool`
- **AmbientReverb**: `ReverbType`
- **AudioApiByDefault**: `RolloutState` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **CharacterSoundsUseNewApi**: `RolloutState` (Security: Read=None, Write=PluginSecurity)
- **DefaultListenerLocation**: `ListenerLocation` (Security: Read=PluginSecurity, Write=PluginSecurity)
- **DiffractionEnabled**: `bool`
- **DistanceFactor**: `float`
- **DopplerScale**: `float`
- **IsNewExpForAudioApiByDefault**: `bool` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **ListenerCFrame**: `CFrame`
- **ListenerObject**: `Instance`
- **ListenerType**: `ListenerType`
- **OcclusionEnabled**: `bool`
- **RespectFilteringEnabled**: `bool`
- **ReverbEnabled**: `bool`
- **RolloffScale**: `float`
- **VolumetricAudio**: `VolumetricAudio` [NotScriptable]

## Methods

- **BeginRecording**() -> `bool`
- **EndRecording**() -> `Dictionary` [Yields]
- **GetAudioApiByDefault**() -> `bool`
- **GetAudioInstances**() -> `Array`
- **GetInputDevice**() -> `Tuple`
- **GetInputDevices**() -> `Tuple`
- **GetListener**() -> `Tuple`
- **GetMixerTime**() -> `double`
- **GetOutputDevice**() -> `Tuple`
- **GetOutputDevices**() -> `Tuple`
- **GetRecordingDevices**() -> `Dictionary` [Yields]
- **GetSoundMemoryData**() -> `Dictionary`
- **InsertAsset**(`assetId: ContentId`, `assetName: string`, `useSelection: bool = true`) -> `Instances`
- **OpenAttenuationCurveEditor**(`selectedCurveObjects: Instances`) -> `null`
- **OpenDirectionalCurveEditor**(`selectedCurveObjects: Instances`) -> `null`
- **PlayLocalSound**(`sound: Instance`) -> `null`
- **SetAudioApiByDefault**(`enabled: bool`) -> `null`
- **SetInputDevice**(`nameOrInstance: Variant`, `guidOrPin: string`) -> `null`
- **SetListener**(`listenerType: ListenerType`, `listener: Tuple`) -> `null`
- **SetOutputDevice**(`name: string`, `guid: string`) -> `null`
- **SetRecordingDevice**(`deviceIndex: int`) -> `bool`
- **SetSoundEnabled**(`enabled: bool`) -> `null`

## Events

- **AudioInstanceAdded**(`instance: Instance`)
- **DeviceListChanged**(`newDevices: Tuple`)
- **OpenAttenuationCurveEditorSignal**(`selectedCurveObjects: Instances`)
- **OpenAudioCompressorEditorSignal**(`selectedCompressorObjects: Instances`)
- **OpenAudioEqualizerEditorSignal**(`selectedEqualizerObjects: Instances`)
- **OpenDirectionalCurveEditorSignal**(`selectedCurveObjects: Instances`)
