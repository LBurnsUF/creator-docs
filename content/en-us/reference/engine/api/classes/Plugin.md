---
title: Plugin
type: class
superclass: Instance
tags: [NotCreatable]
---

# Plugin

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.Plugin.CollisionEnabled` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.Plugin.DisableUIDragDetectorDrags` | `bool` |  {security: RobloxScriptSecurity} |
| `Class.Plugin.GridSize` | `float` | [ReadOnly] [NotReplicated] |
| `Class.Plugin.HostDataModelType` | `Enum.StudioDataModelType` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Plugin.HostDataModelTypeIsCurrent` | `bool` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Plugin.IsDebuggable` | `bool` |  {security: RobloxScriptSecurity} |
| `Class.Plugin.MultipleDocumentInterfaceInstance` | `Class.MultipleDocumentInterfaceInstance` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Plugin.UsesAssetInsertionDrag` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |

## Methods

### `Class.Plugin:Activate`

``Activate(exclusiveMouse: `bool`)`` → `null`
   {security: PluginSecurity}

### `Class.Plugin:CreateDockWidgetPluginGui`

``CreateDockWidgetPluginGui(pluginGuiId: `string`, dockWidgetPluginGuiInfo: `Datatype.DockWidgetPluginGuiInfo`)`` → `Class.DockWidgetPluginGui`
  [Yields] [Deprecated] {security: PluginSecurity}

### `Class.Plugin:CreateDockWidgetPluginGuiAsync`

``CreateDockWidgetPluginGuiAsync(pluginGuiId: `string`, dockWidgetPluginGuiInfo: `Datatype.DockWidgetPluginGuiInfo`)`` → `Class.DockWidgetPluginGui`
  [Yields] {security: PluginSecurity}

### `Class.Plugin:CreatePluginAction`

``CreatePluginAction(actionId: `string`, text: `string`, statusTip: `string`, iconName: `string`, allowBinding: `bool`)`` → `Class.PluginAction`
   {security: PluginSecurity}

### `Class.Plugin:CreatePluginMenu`

``CreatePluginMenu(id: `string`, title: `string`, icon: `string`)`` → `Class.PluginMenu`
   {security: PluginSecurity}

### `Class.Plugin:CreateQWidgetPluginGui`

``CreateQWidgetPluginGui(pluginGuiId: `string`, pluginGuiOptions: `Dictionary`)`` → `Class.QWidgetPluginGui`
  [Yields] {security: RobloxScriptSecurity}

### `Class.Plugin:CreateToolbar`

``CreateToolbar(name: `string`)`` → `Class.PluginToolbar`
   {security: PluginSecurity}

### `Class.Plugin:Deactivate`

``Deactivate()`` → `null`
   {security: PluginSecurity}

### `Class.Plugin:FinishFullLoading`

``FinishFullLoading()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Plugin:GetItem`

``GetItem(key: `string`, defaultValue: `Variant`)`` → `Variant`
   {security: RobloxScriptSecurity}

### `Class.Plugin:GetJoinMode`

``GetJoinMode()`` → `Enum.JointCreationMode`
   {security: PluginSecurity}

### `Class.Plugin:GetMouse`

``GetMouse()`` → `Class.PluginMouse`
   {security: PluginSecurity}

### `Class.Plugin:GetPluginComponent`

``GetPluginComponent(name: `string`)`` → `Variant`
  [CustomLuaState] {security: RobloxScriptSecurity}

### `Class.Plugin:GetSelectedRibbonTool`

``GetSelectedRibbonTool()`` → `Enum.RibbonTool`
   {security: PluginSecurity}

### `Class.Plugin:GetSetting`

``GetSetting(key: `string`)`` → `Variant`
   {security: PluginSecurity}

### `Class.Plugin:GetStudioUserId`

``GetStudioUserId()`` → `int64`
  [Deprecated] {security: PluginSecurity}

### `Class.Plugin:GetUri`

``GetUri()`` → `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.Plugin:ImportFbxAnimation`

``ImportFbxAnimation(rigModel: `Class.Instance`, isR15: `bool`)`` → `Class.Instance`
  [Yields] [Deprecated] {security: PluginSecurity}

### `Class.Plugin:ImportFbxAnimationAsync`

``ImportFbxAnimationAsync(rigModel: `Class.Instance`, isR15: `bool`)`` → `Class.Instance`
  [Yields] {security: PluginSecurity}

### `Class.Plugin:ImportFbxRig`

``ImportFbxRig(isR15: `bool`)`` → `Class.Instance`
  [Yields] [Deprecated] {security: PluginSecurity}

### `Class.Plugin:ImportFbxRigAsync`

``ImportFbxRigAsync(isR15: `bool`)`` → `Class.Instance`
  [Yields] {security: PluginSecurity}

### `Class.Plugin:Intersect`

``Intersect(objects: `Datatype.Instances`)`` → `Class.Instance`
   {security: PluginSecurity}

### `Class.Plugin:Invoke`

``Invoke(key: `string`, arguments: `Tuple`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Plugin:IsActivated`

``IsActivated()`` → `bool`
   {security: PluginSecurity}

### `Class.Plugin:IsActivatedWithExclusiveMouse`

``IsActivatedWithExclusiveMouse()`` → `bool`
   {security: PluginSecurity}

### `Class.Plugin:IsLoadedFromProject`

``IsLoadedFromProject()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.Plugin:Negate`

``Negate(objects: `Datatype.Instances`)`` → `Datatype.Instances`
   {security: PluginSecurity}

### `Class.Plugin:OnInvoke`

``OnInvoke(key: `string`, callback: `Datatype.Function`)`` → `Class.Instance`
   {security: RobloxScriptSecurity}

### `Class.Plugin:OnInvokeSuspendOverride`

``OnInvokeSuspendOverride(key: `string`, callback: `Datatype.Function`)`` → `Class.Instance`
   {security: RobloxScriptSecurity}

### `Class.Plugin:OnSetItem`

``OnSetItem(key: `string`, callback: `Datatype.Function`)`` → `Class.Instance`
   {security: RobloxScriptSecurity}

### `Class.Plugin:OpenScript`

``OpenScript(script: `Class.LuaSourceContainer`, lineNumber: `int`)`` → `null`
  [Deprecated] {security: PluginSecurity}

### `Class.Plugin:OpenWikiPage`

``OpenWikiPage(url: `string`)`` → `null`
   {security: PluginSecurity}

### `Class.Plugin:PauseSound`

``PauseSound(sound: `Class.Instance`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Plugin:PlaySound`

``PlaySound(sound: `Class.Instance`, normalizedTimePosition: `double`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Plugin:PromptForExistingAssetId`

``PromptForExistingAssetId(assetType: `string`)`` → `int64`
  [Yields] {security: PluginSecurity}

### `Class.Plugin:PromptForExistingAssetIdAsync`

``PromptForExistingAssetIdAsync(assetType: `string`)`` → `int64`
  [Yields] {security: PluginSecurity}

### `Class.Plugin:PromptSaveSelection`

``PromptSaveSelection(suggestedFileName: `string`)`` → `bool`
  [Yields] [Deprecated] {security: PluginSecurity}

### `Class.Plugin:PromptSaveSelectionAsync`

``PromptSaveSelectionAsync(suggestedFileName: `string`)`` → `bool`
  [Yields] {security: PluginSecurity}

### `Class.Plugin:ResumeSound`

``ResumeSound(sound: `Class.Instance`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Plugin:SaveSelectedToRoblox`

``SaveSelectedToRoblox()`` → `null`
   {security: PluginSecurity}

### `Class.Plugin:SelectRibbonTool`

``SelectRibbonTool(tool: `Enum.RibbonTool`, position: `Datatype.UDim2`)`` → `null`
   {security: PluginSecurity}

### `Class.Plugin:Separate`

``Separate(objects: `Datatype.Instances`)`` → `Datatype.Instances`
   {security: PluginSecurity}

### `Class.Plugin:SetItem`

``SetItem(key: `string`, value: `Variant`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Plugin:SetReady`

``SetReady()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Plugin:SetSetting`

``SetSetting(key: `string`, value: `Variant`)`` → `null`
   {security: PluginSecurity}

### `Class.Plugin:StartDecalDrag`

``StartDecalDrag(decal: `Class.Instance`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Plugin:StartDrag`

``StartDrag(dragData: `Dictionary`)`` → `null`
   {security: PluginSecurity}

### `Class.Plugin:StopAllSounds`

``StopAllSounds()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Plugin:Union`

``Union(objects: `Datatype.Instances`)`` → `Class.Instance`
   {security: PluginSecurity}

## Events

### `Class.Plugin.Deactivation`

Fires with: ()

### `Class.Plugin.Ready`

Fires with: ()

### `Class.Plugin.Unloading`

Fires with: ()

### `Class.Plugin.ViewportDragDropped`

Fires with: (dragData: `Dictionary`)

### `Class.Plugin.ViewportDragEntered`

Fires with: (dragData: `Dictionary`)

### `Class.Plugin.ViewportDragLeft`

Fires with: ()

## Callbacks

### `Class.Plugin.ProcessAssetInsertionDrag`

``ProcessAssetInsertionDrag(assetId: `string`, assetTypeId: `int`, instances: `Datatype.Instances`)`` → `Datatype.Instances`
  [NoYield]

### `Class.Plugin.ProcessAssetInsertionDrop`

``ProcessAssetInsertionDrop()`` → `null`
  [NoYield]
