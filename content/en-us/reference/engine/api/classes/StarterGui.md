---
title: StarterGui
type: class
superclass: BasePlayerGui
tags: [NotCreatable, Service]
---

# StarterGui

**Inherits**: BasePlayerGui > Instance > Object

**Tags**: NotCreatable, Service

## Properties

- **ClipsDescendantsSupportsRotation**: `RolloutState` [NotScriptable]
- **ProcessUserInput**: `bool` [Hidden] [NotReplicated] (Security: Read=PluginSecurity, Write=PluginSecurity)
- **ResetPlayerGuiOnSpawn**: `bool` [Deprecated]
- **RtlTextSupport**: `RtlTextSupport` [NotScriptable]
- **ScreenOrientation**: `ScreenOrientation`
- **ShowDevelopmentGui**: `bool`
- **StudioDefaultStyleSheet**: `StyleSheet` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **StudioInsertWidgetLayerCollectorAutoLinkStyleSheet**: `StyleSheet` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **VirtualCursorMode**: `VirtualCursorMode` [NotScriptable]

## Methods

- **GetCore**(`parameterName: string`) -> `Variant` [Yields]
- **GetCoreGuiEnabled**(`coreGuiType: CoreGuiType`) -> `bool`
- **RegisterGetCore**(`parameterName: string`, `getFunction: Function`) -> `null`
- **RegisterSetCore**(`parameterName: string`, `setFunction: Function`) -> `null`
- **SetCore**(`parameterName: string`, `value: Variant`) -> `null`
- **SetCoreGuiEnabled**(`coreGuiType: CoreGuiType`, `enabled: bool`) -> `null`

## Events

- **CoreGuiChangedSignal**(`coreGuiType: CoreGuiType`, `enabled: bool`)
