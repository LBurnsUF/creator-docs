---
title: StyleRule
type: class
superclass: StyleBase
---

# StyleRule

**Inherits from:** `Class.StyleBase` > `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.StyleRule.Priority` | `int` |  |
| `Class.StyleRule.Selector` | `string` |  |
| `Class.StyleRule.SelectorError` | `string` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.StyleRule:GetDefaultPropertyTransition`

``GetDefaultPropertyTransition()`` → `Variant`

### `Class.StyleRule:GetProperties`

``GetProperties()`` → `Dictionary`

### `Class.StyleRule:GetPropertiesResolved`

``GetPropertiesResolved()`` → `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.StyleRule:GetProperty`

``GetProperty(name: `string`)`` → `Variant`

### `Class.StyleRule:GetPropertyResolved`

``GetPropertyResolved(name: `string`)`` → `Variant`
   {security: RobloxScriptSecurity}

### `Class.StyleRule:GetPropertyTransitions`

``GetPropertyTransitions()`` → `Dictionary`

### `Class.StyleRule:SetDefaultPropertyTransition`

``SetDefaultPropertyTransition(transitionParams: `Variant`)`` → `null`

### `Class.StyleRule:SetProperties`

``SetProperties(styleProperties: `Dictionary`)`` → `null`

### `Class.StyleRule:SetProperty`

``SetProperty(name: `string`, value: `Variant`)`` → `null`

### `Class.StyleRule:SetPropertyTransition`

``SetPropertyTransition(property: `string`, transitionParams: `Variant`)`` → `null`

### `Class.StyleRule:SetPropertyTransitions`

``SetPropertyTransitions(properties: `Dictionary`)`` → `null`

## Events

### `Class.StyleRule.StyleRulePropertyChanged`

Fires with: (styleProperty: `string`)
