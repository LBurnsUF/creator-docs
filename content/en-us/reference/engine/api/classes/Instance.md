---
title: Instance
type: class
superclass: Object
tags: [NotCreatable, NotBrowsable]
---

# Instance

**Inherits from:** `Class.Object`

**Tags:** [NotCreatable] [NotBrowsable]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.Instance.Archivable` | `bool` |  |
| `Class.Instance.Capabilities` | `Datatype.SecurityCapabilities` |  |
| `Class.Instance.DataCost` | `int` | [Hidden] [ReadOnly] [NotReplicated] [Deprecated] {security: LocalUserSecurity} |
| `Class.Instance.IsInSandbox` | `bool` | [ReadOnly] [NotReplicated] [NotScriptable] |
| `Class.Instance.Name` | `string` |  |
| `Class.Instance.Parent` | `Class.Instance` | [NotReplicated] |
| `Class.Instance.PredictionMode` | `Enum.PredictionMode` | [ReadOnly] [NotReplicated] [NotScriptable] |
| `Class.Instance.RobloxLocked` | `bool` | [Hidden] {security: PluginSecurity} |
| `Class.Instance.Sandboxed` | `bool` | [NotReplicated] |
| `Class.Instance.SourceAssetId` | `int64` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.Instance.UniqueId` | `Datatype.UniqueId` | [NotReplicated] {read: RobloxScriptSecurity, write: RobloxSecurity} |
| `Class.Instance.archivable` | `bool` | [Hidden] [NotReplicated] [Deprecated] |

## Methods

### `Class.Instance:AddTag`

``AddTag(tag: `string`)`` → `null`

### `Class.Instance:ClearAllChildren`

``ClearAllChildren()`` → `null`

### `Class.Instance:Clone`

``Clone()`` → `Class.Instance`

### `Class.Instance:Destroy`

``Destroy()`` → `null`

### `Class.Instance:FindFirstAncestor`

``FindFirstAncestor(name: `string`)`` → `Class.Instance`

### `Class.Instance:FindFirstAncestorOfClass`

``FindFirstAncestorOfClass(className: `string`)`` → `Class.Instance`

### `Class.Instance:FindFirstAncestorWhichIsA`

``FindFirstAncestorWhichIsA(className: `string`)`` → `Class.Instance`

### `Class.Instance:FindFirstChild`

``FindFirstChild(name: `string`, recursive: `bool`)`` → `Class.Instance`

### `Class.Instance:FindFirstChildOfClass`

``FindFirstChildOfClass(className: `string`)`` → `Class.Instance`

### `Class.Instance:FindFirstChildWhichIsA`

``FindFirstChildWhichIsA(className: `string`, recursive: `bool`)`` → `Class.Instance`

### `Class.Instance:FindFirstDescendant`

``FindFirstDescendant(name: `string`)`` → `Class.Instance`

### `Class.Instance:GetActor`

``GetActor()`` → `Class.Actor`

### `Class.Instance:GetAttribute`

``GetAttribute(attribute: `string`)`` → `Variant`

### `Class.Instance:GetAttributeChangedSignal`

``GetAttributeChangedSignal(attribute: `string`)`` → `Datatype.RBXScriptSignal`

### `Class.Instance:GetAttributes`

``GetAttributes()`` → `Dictionary`
  [CustomLuaState]

### `Class.Instance:GetChildren`

``GetChildren()`` → `Datatype.Instances`

### `Class.Instance:GetDebugId`

``GetDebugId(scopeLength: `int`)`` → `string`
  [NotBrowsable] {security: PluginSecurity}

### `Class.Instance:GetDescendants`

``GetDescendants()`` → `Datatype.Instances`
  [CustomLuaState]

### `Class.Instance:GetFullName`

``GetFullName()`` → `string`

### `Class.Instance:GetStyled`

``GetStyled(name: `string`, selector: `string?`)`` → `Variant`

### `Class.Instance:GetStyledPropertyChangedSignal`

``GetStyledPropertyChangedSignal(property: `string`)`` → `Datatype.RBXScriptSignal`

### `Class.Instance:GetTags`

``GetTags()`` → `Array`

### `Class.Instance:HasTag`

``HasTag(tag: `string`)`` → `bool`

### `Class.Instance:IsAncestorOf`

``IsAncestorOf(descendant: `Class.Instance`)`` → `bool`

### `Class.Instance:IsDescendantOf`

``IsDescendantOf(ancestor: `Class.Instance`)`` → `bool`

### `Class.Instance:IsPropertyModified`

``IsPropertyModified(property: `string`)`` → `bool`

### `Class.Instance:QueryDescendants`

``QueryDescendants(selector: `string`)`` → `Datatype.Instances`
  [CustomLuaState]

### `Class.Instance:Remove`

``Remove()`` → `null`
  [Deprecated]

### `Class.Instance:RemoveTag`

``RemoveTag(tag: `string`)`` → `null`

### `Class.Instance:ResetPropertyToDefault`

``ResetPropertyToDefault(property: `string`)`` → `null`

### `Class.Instance:SetAttribute`

``SetAttribute(attribute: `string`, value: `Variant`)`` → `null`

### `Class.Instance:WaitForChild`

``WaitForChild(childName: `string`, timeOut: `double`)`` → `Class.Instance`
  [CustomLuaState] [CanYield]

### `Class.Instance:children`

``children()`` → `Datatype.Instances`
  [Deprecated]

### `Class.Instance:clone`

``clone()`` → `Class.Instance`
  [Deprecated]

### `Class.Instance:destroy`

``destroy()`` → `null`
  [Deprecated]

### `Class.Instance:findFirstChild`

``findFirstChild(name: `string`, recursive: `bool`)`` → `Class.Instance`
  [Deprecated]

### `Class.Instance:getChildren`

``getChildren()`` → `Datatype.Instances`
  [Deprecated]

### `Class.Instance:isDescendantOf`

``isDescendantOf(ancestor: `Class.Instance`)`` → `bool`
  [Deprecated]

### `Class.Instance:remove`

``remove()`` → `null`
  [Deprecated]

## Events

### `Class.Instance.AncestryChanged`

Fires with: (child: `Class.Instance`, parent: `Class.Instance`)

### `Class.Instance.AttributeChanged`

Fires with: (attribute: `string`)

### `Class.Instance.ChildAdded`

Fires with: (child: `Class.Instance`)

### `Class.Instance.ChildRemoved`

Fires with: (child: `Class.Instance`)

### `Class.Instance.DescendantAdded`

Fires with: (descendant: `Class.Instance`)

### `Class.Instance.DescendantRemoving`

Fires with: (descendant: `Class.Instance`)

### `Class.Instance.Destroying`

Fires with: ()

### `Class.Instance.StyledPropertiesChanged`

Fires with: ()

### `Class.Instance.childAdded`

Fires with: (child: `Class.Instance`)
  [Deprecated]
