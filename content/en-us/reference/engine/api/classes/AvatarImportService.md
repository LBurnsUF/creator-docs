---
title: AvatarImportService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# AvatarImportService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **ImportFBXAnimationFromFilePathUserMayChooseModel**(`fbxFilePath: string`, `selectedRig: Instance`, `userChooseModelThenImportCB: Function`) -> `Instance` [Yields]
- **ImportFBXAnimationUserMayChooseModel**(`selectedRig: Instance`, `userChooseModelThenImportCB: Function`) -> `Instance` [Yields]
- **ImportFbxRigWithoutSceneLoad**(`isR15: bool = true`) -> `Instance` [Yields]
- **ImportLoadedFBXAnimation**(`useFBXModel: bool`) -> `Instance` [Yields]
- **LoadRigAndDetectType**(`promptR15Callback: Function`) -> `Instance` [Yields]
