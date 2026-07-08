---
title: Model
type: class
superclass: PVInstance
---

# Model

Models are container objects, meaning they group objects together. They are
best used to hold collections of `Class.BasePart|BaseParts` and have a number
of functions that extend their functionality.

**Inherits from:** `Class.PVInstance` > `Class.Instance` > `Class.Object`

## Description

Models are container objects, meaning they group objects together. They are
best used to hold collections of `Class.BasePart|BaseParts` and have a number
of functions that extend their functionality.

Models are intended to represent **geometric** groupings. If your grouping has
no geometric interpretation, for instance a collection of
`Class.Script|Scripts`, use a `Class.Folder` instead.

Models whose constituent parts are joined together with joints (so that they
can move around or be destroyed via physics simulation) usually have a
`Class.Model.PrimaryPart|PrimaryPart` set, as it specifies which part within
the model the pivot and bounding box will "follow" as the model moves. Static
models which stay in one place do not benefit from having a primary part set.

Models have a wide range of applications, including Roblox player characters.
They also have a number of unique behaviors that are important to keep in
mind:

- When a `Class.Humanoid` and a `Class.Part` named **Head** are parented under
  a model, a name/health GUI will appear over the model; see
  [Character Name/Health Display](../../../characters/name-health-display.md)
  for details.
- If a part's position on the **Y** axis hits the
  `Class.Workspace.FallenPartsDestroyHeight` value, and it was the last object
  inside of a `Class.Model`, the model will be destroyed as well.
- When used in a place with `Class.Workspace.StreamingEnabled` set to true,
  the value of `Class.Model.ModelStreamingMode|ModelStreamingMode` controls
  various behaviors around how the model and any descendants are replicated
  and/or removed from clients. In addition, the value of
  `Class.Model.LevelOfDetail|LevelOfDetail` impacts rendering of the model.

As with all `Class.Instance` types, the fact that a parent `Class.Model` is
replicated to a client does not guarantee that all its children are
replicated. This is particularly important if these instances are being
accessed by code running on the client, such as in a `Class.LocalScript`.
Using `Class.Model.ModelStreamingMode|ModelStreamingMode` with values such as
`Enum.ModelStreamingMode|Atomic` can ensure that the entire model and all of
its descendants are present if the parent model exists on the client, or you
can use `Class.Instance:WaitForChild()|WaitForChild()` when atomicity is not
desired.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Model.LevelOfDetail` | `Enum.ModelLevelOfDetail` |  {security: PluginSecurity} |
| `Class.Model.ModelStreamingMode` | `Enum.ModelStreamingMode` |  |
| `Class.Model.PrimaryPart` | `Class.BasePart` |  |
| `Class.Model.Scale` | `float` | [NotReplicated] [NotScriptable] |
| `Class.Model.WorldPivot` | `Datatype.CFrame` | [NotReplicated] |

## Methods

### `Class.Model:AddPersistentPlayer`

``AddPersistentPlayer(playerInstance: `Class.Player`)`` -> `null`

### `Class.Model:BreakJoints`

``BreakJoints()`` -> `null`
  [Deprecated]

### `Class.Model:GetBoundingBox`

``GetBoundingBox()`` -> `[{'Category': 'DataType', 'Name': 'CFrame'}, {'Category': 'DataType', 'Name': 'Vector3'}]`

### `Class.Model:GetExtentsSize`

``GetExtentsSize()`` -> `Datatype.Vector3`

### `Class.Model:GetModelCFrame`

``GetModelCFrame()`` -> `Datatype.CFrame`
  [Deprecated]

### `Class.Model:GetModelSize`

``GetModelSize()`` -> `Datatype.Vector3`
  [Deprecated]

### `Class.Model:GetPersistentPlayers`

``GetPersistentPlayers()`` -> `Datatype.Instances`

### `Class.Model:GetPrimaryPartCFrame`

``GetPrimaryPartCFrame()`` -> `Datatype.CFrame`
  [Deprecated]

### `Class.Model:GetScale`

``GetScale()`` -> `float`

### `Class.Model:MakeJoints`

``MakeJoints()`` -> `null`
  [Deprecated]

### `Class.Model:MoveTo`

``MoveTo(position: `Datatype.Vector3`)`` -> `null`

### `Class.Model:RemovePersistentPlayer`

``RemovePersistentPlayer(playerInstance: `Class.Player`)`` -> `null`

### `Class.Model:ResetOrientationToIdentity`

``ResetOrientationToIdentity()`` -> `null`
  [Deprecated]

### `Class.Model:ScaleTo`

``ScaleTo(newScaleFactor: `float`)`` -> `null`

### `Class.Model:SetIdentityOrientation`

``SetIdentityOrientation()`` -> `null`
  [Deprecated]

### `Class.Model:SetPrimaryPartCFrame`

``SetPrimaryPartCFrame(cframe: `Datatype.CFrame`)`` -> `null`
  [Deprecated]

### `Class.Model:TranslateBy`

``TranslateBy(delta: `Datatype.Vector3`)`` -> `null`

### `Class.Model:breakJoints`

``breakJoints()`` -> `null`
  [Deprecated]

### `Class.Model:makeJoints`

``makeJoints()`` -> `null`
  [Deprecated]

### `Class.Model:move`

``move(location: `Datatype.Vector3`)`` -> `null`
  [Deprecated]

### `Class.Model:moveTo`

``moveTo(location: `Datatype.Vector3`)`` -> `null`
  [Deprecated]
