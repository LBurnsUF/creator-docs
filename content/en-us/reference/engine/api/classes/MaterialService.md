---
title: MaterialService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# MaterialService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.MaterialService.AsphaltName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.BasaltName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.BrickName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.CardboardName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.CarpetName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.CeramicTilesName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.ClayRoofTilesName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.CobblestoneName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.ConcreteName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.CorrodedMetalName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.CrackedLavaName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.DiamondPlateName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.FabricName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.FoilName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.GlacierName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.GraniteName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.GrassName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.GroundName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.IceName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.LeafyGrassName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.LeatherName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.LimestoneName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.MarbleName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.MetalName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.MudName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.PavementName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.PebbleName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.PlasterName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.PlasticName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.RockName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.RoofShinglesName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.RubberName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.SaltName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.SandName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.SandstoneName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.SlateName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.SmoothPlasticName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.SnowName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.Use2022Materials` | `bool` | [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.MaterialService.WoodName` | `string` | [NotScriptable] {security: RobloxSecurity} |
| `Class.MaterialService.WoodPlanksName` | `string` | [NotScriptable] {security: RobloxSecurity} |

## Methods

### `Class.MaterialService:GetBaseMaterialOverride`

``GetBaseMaterialOverride(material: `Enum.Material`)`` → `string`

### `Class.MaterialService:GetIsMaterialActionAsToolEnabled`

``GetIsMaterialActionAsToolEnabled()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.MaterialService:GetMaterialOverrideChanged`

``GetMaterialOverrideChanged(material: `Enum.Material`)`` → `Datatype.RBXScriptSignal`
   {security: RobloxScriptSecurity}

### `Class.MaterialService:GetMaterialVariant`

``GetMaterialVariant(material: `Enum.Material`, name: `string`)`` → `Class.MaterialVariant`

### `Class.MaterialService:GetOverrideStatus`

``GetOverrideStatus(material: `Enum.Material`)`` → `Enum.PropertyStatus`
   {security: RobloxScriptSecurity}

### `Class.MaterialService:SetBaseMaterialOverride`

``SetBaseMaterialOverride(material: `Enum.Material`, name: `string`)`` → `null`

### `Class.MaterialService:SetCurrentMaterial`

``SetCurrentMaterial(baseMaterial: `Enum.Material`, materialVariant: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.MaterialService:ToggleMaterialFillToolEnabled`

``ToggleMaterialFillToolEnabled()`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.MaterialService.MaterialFillToolEnabledChanged`

Fires with: (shouldEnable: `bool`)

### `Class.MaterialService.OverrideStatusChanged`

Fires with: (material: `Enum.Material`)
