---
title: MaterialService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# MaterialService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Properties

- **AsphaltName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **BasaltName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **BrickName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **CardboardName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **CarpetName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **CeramicTilesName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **ClayRoofTilesName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **CobblestoneName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **ConcreteName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **CorrodedMetalName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **CrackedLavaName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **DiamondPlateName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **FabricName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **FoilName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **GlacierName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **GraniteName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **GrassName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **GroundName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **IceName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **LeafyGrassName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **LeatherName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **LimestoneName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **MarbleName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **MetalName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **MudName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **PavementName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **PebbleName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **PlasterName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **PlasticName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **RockName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **RoofShinglesName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **RubberName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **SaltName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **SandName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **SandstoneName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **SlateName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **SmoothPlasticName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **SnowName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **Use2022Materials**: `bool` [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **WoodName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **WoodPlanksName**: `string` [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)

## Methods

- **GetBaseMaterialOverride**(`material: Material`) -> `string`
- **GetIsMaterialActionAsToolEnabled**() -> `bool`
- **GetMaterialOverrideChanged**(`material: Material`) -> `RBXScriptSignal`
- **GetMaterialVariant**(`material: Material`, `name: string`) -> `MaterialVariant`
- **GetOverrideStatus**(`material: Material`) -> `PropertyStatus`
- **SetBaseMaterialOverride**(`material: Material`, `name: string`) -> `null`
- **SetCurrentMaterial**(`baseMaterial: Material`, `materialVariant: string`) -> `null`
- **ToggleMaterialFillToolEnabled**() -> `null`

## Events

- **MaterialFillToolEnabledChanged**(`shouldEnable: bool`)
- **OverrideStatusChanged**(`material: Material`)
