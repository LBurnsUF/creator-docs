---
title: WrapLayer
type: class
superclass: BaseWrap
---

# WrapLayer

The WrapLayer object defines a 3D accessory's inner and outer surfaces and
other properties related to layering accessories. These surfaces, or the Inner
Cage and Outer Cage, are similar to collision boxes, and describe the surfaces
of which other 3D accessories can be placed without clipping or breaking.

**Inherits from:** `Class.BaseWrap` > `Class.Instance` > `Class.Object`

## Description

The WrapLayer object defines a 3D accessory's inner and outer surfaces and
other properties related to layering accessories. These surfaces, or the Inner
Cage and Outer Cage, are similar to collision boxes, and describe the surfaces
of which other 3D accessories can be placed without clipping or breaking.

Internally, WrapLayer also uses the UV layout of the Inner and Outer cages to
match coordinates to another 3D object's cage. This powers the deformation of
objects around differently shaped avatars and underlying accessories.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.WrapLayer.AutoSkin` | `Enum.WrapLayerAutoSkin` |  |
| `Class.WrapLayer.BindOffset` | `Datatype.CFrame` |  {write: PluginSecurity} |
| `Class.WrapLayer.Color` | `Datatype.Color3` | [NotReplicated] [NotScriptable] |
| `Class.WrapLayer.DebugMode` | `Enum.WrapLayerDebugMode` | [NotReplicated] [NotScriptable] |
| `Class.WrapLayer.Enabled` | `bool` |  |
| `Class.WrapLayer.MaxSize` | `Datatype.Vector3` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.WrapLayer.Offset` | `Datatype.Vector3` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.WrapLayer.Order` | `int` |  |
| `Class.WrapLayer.Puffiness` | `float` | [Deprecated] |
| `Class.WrapLayer.ReferenceMeshContent` | `Datatype.Content` |  {write: PluginSecurity} |
| `Class.WrapLayer.ReferenceMeshId` | `Datatype.ContentId` |  {write: PluginSecurity} |
| `Class.WrapLayer.ReferenceOrigin` | `Datatype.CFrame` |  {write: PluginSecurity} |
| `Class.WrapLayer.ReferenceOriginWorld` | `Datatype.CFrame` | [ReadOnly] [NotReplicated] |
| `Class.WrapLayer.ShrinkFactor` | `float` | [Deprecated] {write: PluginSecurity} |
