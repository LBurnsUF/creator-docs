---
title: BaseWrap
type: class
superclass: Instance
tags: [NotCreatable]
---

# BaseWrap

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.BaseWrap.CageMeshContent` | `Datatype.Content` |  {write: PluginSecurity} |
| `Class.BaseWrap.CageMeshId` | `Datatype.ContentId` |  {write: PluginSecurity} |
| `Class.BaseWrap.CageOrigin` | `Datatype.CFrame` |  {write: PluginSecurity} |
| `Class.BaseWrap.CageOriginWorld` | `Datatype.CFrame` | [ReadOnly] [NotReplicated] |
| `Class.BaseWrap.HSRAssetId` | `Datatype.ContentId` |  {read: RobloxScriptSecurity, write: RobloxSecurity} |
| `Class.BaseWrap.ImportOrigin` | `Datatype.CFrame` |  {write: PluginSecurity} |
| `Class.BaseWrap.ImportOriginWorld` | `Datatype.CFrame` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.BaseWrap:GetCageOffset`

``GetCageOffset()`` → `Datatype.Vector3`
   {security: RobloxScriptSecurity}

### `Class.BaseWrap:GetFaces`

``GetFaces(cageType: `Enum.CageType`)`` → `Array`
   {security: RobloxScriptSecurity}

### `Class.BaseWrap:GetUVs`

``GetUVs(cageType: `Enum.CageType`)`` → `Array`
   {security: RobloxScriptSecurity}

### `Class.BaseWrap:GetVertices`

``GetVertices(cageType: `Enum.CageType`)`` → `Array`
   {security: RobloxScriptSecurity}

### `Class.BaseWrap:IsHSRReady`

``IsHSRReady()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.BaseWrap:ModifyVertices`

``ModifyVertices(cageType: `Enum.CageType`, vertices: `Array`)`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.BaseWrap.VerticesModified`

Fires with: (vertices: `Array`)
