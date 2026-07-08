---
title: MaterialVariant
type: class
superclass: Instance
---

# MaterialVariant

Represent a variant of a Material.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

Using MaterialVariant objects can expand the variety of materials in an
experience. MaterialVariant has properties that can define the appearance of a
material. Its name can be set in MaterialService to globally override a
built-in material, or set in the `Class.BasePart.MaterialVariant` property to
change certain Parts. MaterialVariant objects only work as descendants of
MaterialService.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.MaterialVariant.AlphaMode` | `Enum.AlphaMode` |  |
| `Class.MaterialVariant.BaseMaterial` | `Enum.Material` |  {write: PluginSecurity} |
| `Class.MaterialVariant.ColorMap` | `Datatype.ContentId` |  {security: PluginSecurity} |
| `Class.MaterialVariant.ColorMapContent` | `Datatype.Content` |  {security: PluginSecurity} |
| `Class.MaterialVariant.CustomPhysicalProperties` | `Datatype.PhysicalProperties` |  |
| `Class.MaterialVariant.EmissiveMaskContent` | `Datatype.Content` |  {security: PluginSecurity} |
| `Class.MaterialVariant.EmissiveStrength` | `float` |  |
| `Class.MaterialVariant.EmissiveTint` | `Datatype.Color3` |  |
| `Class.MaterialVariant.MaterialPattern` | `Enum.MaterialPattern` |  |
| `Class.MaterialVariant.MetalnessMap` | `Datatype.ContentId` |  {security: PluginSecurity} |
| `Class.MaterialVariant.MetalnessMapContent` | `Datatype.Content` |  {security: PluginSecurity} |
| `Class.MaterialVariant.NormalMap` | `Datatype.ContentId` |  {security: PluginSecurity} |
| `Class.MaterialVariant.NormalMapContent` | `Datatype.Content` |  {security: PluginSecurity} |
| `Class.MaterialVariant.RoughnessMap` | `Datatype.ContentId` |  {security: PluginSecurity} |
| `Class.MaterialVariant.RoughnessMapContent` | `Datatype.Content` |  {security: PluginSecurity} |
| `Class.MaterialVariant.StudsPerTile` | `float` |  |
