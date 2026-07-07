---
title: AssetImportSession
type: class
superclass: ImportSession
tags: [NotCreatable, NotReplicated]
---

# AssetImportSession

**Inherits**: ImportSession > Instance > Object

**Tags**: NotCreatable, NotReplicated

## Methods

- **ApplyPreset**(`preset: Dictionary`) -> `null`
- **CreatePresetFromData**(`importData: Instance`) -> `Dictionary`
- **GetImportTree**() -> `Instance`
- **GetKeyframeSequences**() -> `Instances`
- **GetKeyframeSequencesForSelectedRestPose**(`modelInstance: Instance`, `restPoseSource: RestPoseModel`) -> `Instances`
- **GetKeyframeSequencesForSelectedRestPoseWithClip**(`modelInstance: Instance`, `restPoseSource: RestPoseModel`, `animationIndex: int`) -> `Instances`
- **GetRigVisualization**(`importDataInstance: Instance`) -> `Instance`
- **GetUploadStatus**() -> `Dictionary`
- **HasAnimation**() -> `bool`
- **IsAvatar**() -> `bool`
- **IsGltf**() -> `bool`
- **IsR15**() -> `bool`
- **Reset**() -> `null`
- **usesCustomRestPoseLua**() -> `bool`
