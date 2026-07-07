---
title: Instance
type: class
superclass: Object
tags: [NotCreatable, NotBrowsable]
---

# Instance

**Inherits**: Object

**Tags**: NotCreatable, NotBrowsable

## Properties

- **Archivable**: `bool`
- **Capabilities**: `SecurityCapabilities`
- **DataCost**: `int` [Hidden] [ReadOnly] [NotReplicated] [Deprecated] (Security: Read=LocalUserSecurity, Write=LocalUserSecurity)
- **IsInSandbox**: `bool` [ReadOnly] [NotReplicated] [NotScriptable]
- **Name**: `string`
- **Parent**: `Instance` [NotReplicated]
- **PredictionMode**: `PredictionMode` [ReadOnly] [NotReplicated] [NotScriptable]
- **RobloxLocked**: `bool` [Hidden] (Security: Read=PluginSecurity, Write=PluginSecurity)
- **Sandboxed**: `bool` [NotReplicated]
- **SourceAssetId**: `int64` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **UniqueId**: `UniqueId` [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxSecurity)
- **archivable**: `bool` [Hidden] [NotReplicated] [Deprecated]

## Methods

- **AddTag**(`tag: string`) -> `null`
- **ClearAllChildren**() -> `null`
- **Clone**() -> `Instance`
- **Destroy**() -> `null`
- **FindFirstAncestor**(`name: string`) -> `Instance`
- **FindFirstAncestorOfClass**(`className: string`) -> `Instance`
- **FindFirstAncestorWhichIsA**(`className: string`) -> `Instance`
- **FindFirstChild**(`name: string`, `recursive: bool = false`) -> `Instance`
- **FindFirstChildOfClass**(`className: string`) -> `Instance`
- **FindFirstChildWhichIsA**(`className: string`, `recursive: bool = false`) -> `Instance`
- **FindFirstDescendant**(`name: string`) -> `Instance`
- **GetActor**() -> `Actor`
- **GetAttribute**(`attribute: string`) -> `Variant`
- **GetAttributeChangedSignal**(`attribute: string`) -> `RBXScriptSignal`
- **GetAttributes**() -> `Dictionary` [CustomLuaState]
- **GetChildren**() -> `Instances`
- **GetDebugId**(`scopeLength: int = 4`) -> `string` [NotBrowsable]
- **GetDescendants**() -> `Instances` [CustomLuaState]
- **GetFullName**() -> `string`
- **GetStyled**(`name: string`, `selector: string?`) -> `Variant`
- **GetStyledPropertyChangedSignal**(`property: string`) -> `RBXScriptSignal`
- **GetTags**() -> `Array`
- **HasTag**(`tag: string`) -> `bool`
- **IsAncestorOf**(`descendant: Instance`) -> `bool`
- **IsDescendantOf**(`ancestor: Instance`) -> `bool`
- **IsPropertyModified**(`property: string`) -> `bool`
- **QueryDescendants**(`selector: string`) -> `Instances` [CustomLuaState]
- **Remove**() -> `null` [Deprecated]
- **RemoveTag**(`tag: string`) -> `null`
- **ResetPropertyToDefault**(`property: string`) -> `null`
- **SetAttribute**(`attribute: string`, `value: Variant`) -> `null`
- **WaitForChild**(`childName: string`, `timeOut: double`) -> `Instance` [CustomLuaState] [CanYield]
- **children**() -> `Instances` [Deprecated]
- **clone**() -> `Instance` [Deprecated]
- **destroy**() -> `null` [Deprecated]
- **findFirstChild**(`name: string`, `recursive: bool = false`) -> `Instance` [Deprecated]
- **getChildren**() -> `Instances` [Deprecated]
- **isDescendantOf**(`ancestor: Instance`) -> `bool` [Deprecated]
- **remove**() -> `null` [Deprecated]

## Events

- **AncestryChanged**(`child: Instance`, `parent: Instance`)
- **AttributeChanged**(`attribute: string`)
- **ChildAdded**(`child: Instance`)
- **ChildRemoved**(`child: Instance`)
- **DescendantAdded**(`descendant: Instance`)
- **DescendantRemoving**(`descendant: Instance`)
- **Destroying**()
- **StyledPropertiesChanged**()
- **childAdded**(`child: Instance`) [Deprecated]
