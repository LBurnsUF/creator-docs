---
title: BaseWrap
type: class
superclass: Instance
tags: [NotCreatable]
---

# BaseWrap

**Inherits**: Instance > Object

**Tags**: NotCreatable

## Properties

- **CageMeshContent**: `Content` (Security: Read=None, Write=PluginSecurity)
- **CageMeshId**: `ContentId` (Security: Read=None, Write=PluginSecurity)
- **CageOrigin**: `CFrame` (Security: Read=None, Write=PluginSecurity)
- **CageOriginWorld**: `CFrame` [ReadOnly] [NotReplicated]
- **HSRAssetId**: `ContentId` (Security: Read=RobloxScriptSecurity, Write=RobloxSecurity)
- **ImportOrigin**: `CFrame` (Security: Read=None, Write=PluginSecurity)
- **ImportOriginWorld**: `CFrame` [ReadOnly] [NotReplicated]

## Methods

- **GetCageOffset**() -> `Vector3`
- **GetFaces**(`cageType: CageType`) -> `Array`
- **GetUVs**(`cageType: CageType`) -> `Array`
- **GetVertices**(`cageType: CageType`) -> `Array`
- **IsHSRReady**() -> `bool`
- **ModifyVertices**(`cageType: CageType`, `vertices: Array`) -> `null`

## Events

- **VerticesModified**(`vertices: Array`)
