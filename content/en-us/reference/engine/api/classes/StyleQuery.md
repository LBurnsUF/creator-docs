---
title: StyleQuery
type: class
superclass: Instance
---

# StyleQuery

Instance used to set conditions such as `"MaxSize"` and `"PreferredInput"` for
a `Class.StyleRule`.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`StyleQuery` is an instance used to set conditions like `"MaxSize"` and
`"PreferredInput"` for a `Class.StyleRule`. If the conditions are `true`, the
rule's `@` selector is enabled. This is helpful to author styling with dynamic
container sizes and cross-platform UI.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.StyleQuery.AspectRatioRange` | `Datatype.NumberRange` | [NotReplicated] [NotScriptable] {read: RobloxSecurity} |
| `Class.StyleQuery.IsActive` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.StyleQuery.MaxSize` | `Datatype.Vector2` | [NotReplicated] [NotScriptable] {read: RobloxSecurity} |
| `Class.StyleQuery.MinSize` | `Datatype.Vector2` | [NotReplicated] [NotScriptable] {read: RobloxSecurity} |
| `Class.StyleQuery.PreferredInput` | `Enum.PreferredInput` | [NotReplicated] [NotScriptable] {read: RobloxSecurity} |
| `Class.StyleQuery.PreferredTextSize` | `Enum.PreferredTextSize` | [NotReplicated] [NotScriptable] {read: RobloxSecurity} |
| `Class.StyleQuery.ReducedMotionEnabled` | `bool` | [NotReplicated] [NotScriptable] {read: RobloxSecurity} |
| `Class.StyleQuery.ViewportDisplaySize` | `Enum.DisplaySize` | [NotReplicated] [NotScriptable] {read: RobloxSecurity} |

## Methods

### `Class.StyleQuery:GetCondition`

``GetCondition(name: `string`)`` -> `Variant`

### `Class.StyleQuery:GetConditions`

``GetConditions()`` -> `Dictionary`

### `Class.StyleQuery:SetCondition`

``SetCondition(name: `string`, value: `Variant`)`` -> `null`

### `Class.StyleQuery:SetConditions`

``SetConditions(conditions: `Dictionary`)`` -> `null`
