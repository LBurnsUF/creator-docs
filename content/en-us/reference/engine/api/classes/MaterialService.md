---
title: MaterialService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# MaterialService

The game service responsible for managing materials.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

MaterialService is the game service responsible for managing materials. It is
the container for global `Class.MaterialVariant` instances.
`Class.MaterialVariant` can be child or descendant of MaterialService. For
each base Material type, MaterialService internally keeps a set of
MaterialVariant references. `Class.MaterialVariant.Name` is the key to access
it. The `Class.MaterialVariant.Name` and `Class.MaterialVariant.BaseMaterial`
are combined to work as an identifier. If more than one MaterialVariant object
has the same name and BaseMaterial under MaterialService, only one of them can
be used.

MaterialService has some (Material)Name properties. Assigning a
MaterialVariant Name replaces the built-in material with the specified
MaterialVariant. If the MaterialService can't find a matching MaterialVariant,
it falls back to built-in material. Note BaseMaterial should also match, for
example, a MaterialVariant with BaseMaterial Grass can only be assigned to
MaterialService.GrassName, not AsphaltName or any other names. These
properties are not scriptable but can read and write using
`Class.MaterialService:GetBaseMaterialOverride()` and
`Class.MaterialService:SetBaseMaterialOverride()` function.

MaterialService has a `Class.MaterialService.Use2022Materials` property that
switches between legacy materials and new materials introduced in year 2022.
Because legacy and user-generated (new) terrain materials use different
encoding, using legacy terrain materials and MaterialVariant at the same time
has a performance penalty. If your game is using pre-2022 terrain materials,
avoid overriding any built-in materials. Migrate to 2022 materials if
possible.

## Properties

| Property | Type | Description |
|----------|------|-------------|
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

``GetBaseMaterialOverride(material: `Enum.Material`)`` -> `string`

### `Class.MaterialService:GetIsMaterialActionAsToolEnabled`

``GetIsMaterialActionAsToolEnabled()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.MaterialService:GetMaterialOverrideChanged`

``GetMaterialOverrideChanged(material: `Enum.Material`)`` -> `Datatype.RBXScriptSignal`
   {security: RobloxScriptSecurity}

### `Class.MaterialService:GetMaterialVariant`

``GetMaterialVariant(material: `Enum.Material`, name: `string`)`` -> `Class.MaterialVariant`

### `Class.MaterialService:GetOverrideStatus`

``GetOverrideStatus(material: `Enum.Material`)`` -> `Enum.PropertyStatus`
   {security: RobloxScriptSecurity}

### `Class.MaterialService:SetBaseMaterialOverride`

``SetBaseMaterialOverride(material: `Enum.Material`, name: `string`)`` -> `null`

### `Class.MaterialService:SetCurrentMaterial`

``SetCurrentMaterial(baseMaterial: `Enum.Material`, materialVariant: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MaterialService:ToggleMaterialFillToolEnabled`

``ToggleMaterialFillToolEnabled()`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.MaterialService.MaterialFillToolEnabledChanged`

Fires with: (shouldEnable: `bool`)

### `Class.MaterialService.OverrideStatusChanged`

Fires with: (material: `Enum.Material`)
