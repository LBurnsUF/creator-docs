---
title: Model
type: class
superclass: PVInstance
---

# Model

**Inherits from:** `Class.PVInstance` > `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.Model.LevelOfDetail` | `Enum.ModelLevelOfDetail` |  {security: PluginSecurity} |
| `Class.Model.ModelStreamingMode` | `Enum.ModelStreamingMode` |  |
| `Class.Model.PrimaryPart` | `Class.BasePart` |  |
| `Class.Model.Scale` | `float` | [NotReplicated] [NotScriptable] |
| `Class.Model.WorldPivot` | `Datatype.CFrame` | [NotReplicated] |

## Methods

### `Class.Model:AddPersistentPlayer`

``AddPersistentPlayer(playerInstance: `Class.Player`)`` → `null`

### `Class.Model:BreakJoints`

``BreakJoints()`` → `null`
  [Deprecated]

### `Class.Model:GetBoundingBox`

``GetBoundingBox()`` → `[{'Category': 'DataType', 'Name': 'CFrame'}, {'Category': 'DataType', 'Name': 'Vector3'}]`

### `Class.Model:GetExtentsSize`

``GetExtentsSize()`` → `Datatype.Vector3`

### `Class.Model:GetModelCFrame`

``GetModelCFrame()`` → `Datatype.CFrame`
  [Deprecated]

### `Class.Model:GetModelSize`

``GetModelSize()`` → `Datatype.Vector3`
  [Deprecated]

### `Class.Model:GetPersistentPlayers`

``GetPersistentPlayers()`` → `Datatype.Instances`

### `Class.Model:GetPrimaryPartCFrame`

``GetPrimaryPartCFrame()`` → `Datatype.CFrame`
  [Deprecated]

### `Class.Model:GetScale`

``GetScale()`` → `float`

### `Class.Model:MakeJoints`

``MakeJoints()`` → `null`
  [Deprecated]

### `Class.Model:MoveTo`

``MoveTo(position: `Datatype.Vector3`)`` → `null`

### `Class.Model:RemovePersistentPlayer`

``RemovePersistentPlayer(playerInstance: `Class.Player`)`` → `null`

### `Class.Model:ResetOrientationToIdentity`

``ResetOrientationToIdentity()`` → `null`
  [Deprecated]

### `Class.Model:ScaleTo`

``ScaleTo(newScaleFactor: `float`)`` → `null`

### `Class.Model:SetIdentityOrientation`

``SetIdentityOrientation()`` → `null`
  [Deprecated]

### `Class.Model:SetPrimaryPartCFrame`

``SetPrimaryPartCFrame(cframe: `Datatype.CFrame`)`` → `null`
  [Deprecated]

### `Class.Model:TranslateBy`

``TranslateBy(delta: `Datatype.Vector3`)`` → `null`

### `Class.Model:breakJoints`

``breakJoints()`` → `null`
  [Deprecated]

### `Class.Model:makeJoints`

``makeJoints()`` → `null`
  [Deprecated]

### `Class.Model:move`

``move(location: `Datatype.Vector3`)`` → `null`
  [Deprecated]

### `Class.Model:moveTo`

``moveTo(location: `Datatype.Vector3`)`` → `null`
  [Deprecated]
