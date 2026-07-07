---
title: Model
type: class
superclass: PVInstance
---

# Model

**Inherits**: PVInstance > Instance > Object

## Properties

- **LevelOfDetail**: `ModelLevelOfDetail` (Security: Read=PluginSecurity, Write=PluginSecurity)
- **ModelStreamingMode**: `ModelStreamingMode`
- **PrimaryPart**: `BasePart`
- **Scale**: `float` [NotReplicated] [NotScriptable]
- **WorldPivot**: `CFrame` [NotReplicated]

## Methods

- **AddPersistentPlayer**(`playerInstance: Player = nil`) -> `null`
- **BreakJoints**() -> `null` [Deprecated]
- **GetBoundingBox**() -> `[{'Category': 'DataType', 'Name': 'CFrame'}, {'Category': 'DataType', 'Name': 'Vector3'}]`
- **GetExtentsSize**() -> `Vector3`
- **GetModelCFrame**() -> `CFrame` [Deprecated]
- **GetModelSize**() -> `Vector3` [Deprecated]
- **GetPersistentPlayers**() -> `Instances`
- **GetPrimaryPartCFrame**() -> `CFrame` [Deprecated]
- **GetScale**() -> `float`
- **MakeJoints**() -> `null` [Deprecated]
- **MoveTo**(`position: Vector3`) -> `null`
- **RemovePersistentPlayer**(`playerInstance: Player = nil`) -> `null`
- **ResetOrientationToIdentity**() -> `null` [Deprecated]
- **ScaleTo**(`newScaleFactor: float`) -> `null`
- **SetIdentityOrientation**() -> `null` [Deprecated]
- **SetPrimaryPartCFrame**(`cframe: CFrame`) -> `null` [Deprecated]
- **TranslateBy**(`delta: Vector3`) -> `null`
- **breakJoints**() -> `null` [Deprecated]
- **makeJoints**() -> `null` [Deprecated]
- **move**(`location: Vector3`) -> `null` [Deprecated]
- **moveTo**(`location: Vector3`) -> `null` [Deprecated]
