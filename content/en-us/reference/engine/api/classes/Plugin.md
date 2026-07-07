---
title: Plugin
type: class
superclass: Instance
tags: [NotCreatable]
---

# Plugin

**Inherits**: Instance > Object

**Tags**: NotCreatable

## Properties

- **CollisionEnabled**: `bool` [ReadOnly] [NotReplicated]
- **DisableUIDragDetectorDrags**: `bool` (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **GridSize**: `float` [ReadOnly] [NotReplicated]
- **HostDataModelType**: `StudioDataModelType` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **HostDataModelTypeIsCurrent**: `bool` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **IsDebuggable**: `bool` (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **MultipleDocumentInterfaceInstance**: `MultipleDocumentInterfaceInstance` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **UsesAssetInsertionDrag**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **Activate**(`exclusiveMouse: bool`) -> `null`
- **CreateDockWidgetPluginGui**(`pluginGuiId: string`, `dockWidgetPluginGuiInfo: DockWidgetPluginGuiInfo`) -> `DockWidgetPluginGui` [Yields] [Deprecated]
- **CreateDockWidgetPluginGuiAsync**(`pluginGuiId: string`, `dockWidgetPluginGuiInfo: DockWidgetPluginGuiInfo`) -> `DockWidgetPluginGui` [Yields]
- **CreatePluginAction**(`actionId: string`, `text: string`, `statusTip: string`, `iconName: string = `, `allowBinding: bool = true`) -> `PluginAction`
- **CreatePluginMenu**(`id: string`, `title: string = `, `icon: string = `) -> `PluginMenu`
- **CreateQWidgetPluginGui**(`pluginGuiId: string`, `pluginGuiOptions: Dictionary`) -> `QWidgetPluginGui` [Yields]
- **CreateToolbar**(`name: string`) -> `PluginToolbar`
- **Deactivate**() -> `null`
- **FinishFullLoading**() -> `null`
- **GetItem**(`key: string`, `defaultValue: Variant`) -> `Variant`
- **GetJoinMode**() -> `JointCreationMode`
- **GetMouse**() -> `PluginMouse`
- **GetPluginComponent**(`name: string`) -> `Variant` [CustomLuaState]
- **GetSelectedRibbonTool**() -> `RibbonTool`
- **GetSetting**(`key: string`) -> `Variant`
- **GetStudioUserId**() -> `int64` [Deprecated]
- **GetUri**() -> `Dictionary`
- **ImportFbxAnimation**(`rigModel: Instance`, `isR15: bool = true`) -> `Instance` [Yields] [Deprecated]
- **ImportFbxAnimationAsync**(`rigModel: Instance`, `isR15: bool = true`) -> `Instance` [Yields]
- **ImportFbxRig**(`isR15: bool = true`) -> `Instance` [Yields] [Deprecated]
- **ImportFbxRigAsync**(`isR15: bool = true`) -> `Instance` [Yields]
- **Intersect**(`objects: Instances`) -> `Instance`
- **Invoke**(`key: string`, `arguments: Tuple`) -> `null`
- **IsActivated**() -> `bool`
- **IsActivatedWithExclusiveMouse**() -> `bool`
- **IsLoadedFromProject**() -> `bool`
- **Negate**(`objects: Instances`) -> `Instances`
- **OnInvoke**(`key: string`, `callback: Function`) -> `Instance`
- **OnInvokeSuspendOverride**(`key: string`, `callback: Function`) -> `Instance`
- **OnSetItem**(`key: string`, `callback: Function`) -> `Instance`
- **OpenScript**(`script: LuaSourceContainer`, `lineNumber: int = 1`) -> `null` [Deprecated]
- **OpenWikiPage**(`url: string`) -> `null`
- **PauseSound**(`sound: Instance`) -> `null`
- **PlaySound**(`sound: Instance`, `normalizedTimePosition: double = 0`) -> `null`
- **PromptForExistingAssetId**(`assetType: string`) -> `int64` [Yields]
- **PromptForExistingAssetIdAsync**(`assetType: string`) -> `int64` [Yields]
- **PromptSaveSelection**(`suggestedFileName: string = `) -> `bool` [Yields] [Deprecated]
- **PromptSaveSelectionAsync**(`suggestedFileName: string = `) -> `bool` [Yields]
- **ResumeSound**(`sound: Instance`) -> `null`
- **SaveSelectedToRoblox**() -> `null`
- **SelectRibbonTool**(`tool: RibbonTool`, `position: UDim2`) -> `null`
- **Separate**(`objects: Instances`) -> `Instances`
- **SetItem**(`key: string`, `value: Variant`) -> `null`
- **SetReady**() -> `null`
- **SetSetting**(`key: string`, `value: Variant`) -> `null`
- **StartDecalDrag**(`decal: Instance`) -> `null`
- **StartDrag**(`dragData: Dictionary`) -> `null`
- **StopAllSounds**() -> `null`
- **Union**(`objects: Instances`) -> `Instance`

## Events

- **Deactivation**()
- **Ready**()
- **Unloading**()
- **ViewportDragDropped**(`dragData: Dictionary`)
- **ViewportDragEntered**(`dragData: Dictionary`)
- **ViewportDragLeft**()

## Callbacks

- **ProcessAssetInsertionDrag**(`assetId: string`, `assetTypeId: int`, `instances: Instances`) -> `Instances` [NoYield]
- **ProcessAssetInsertionDrop**() -> `null` [NoYield]
