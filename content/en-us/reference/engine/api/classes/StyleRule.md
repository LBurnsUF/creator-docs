---
title: StyleRule
type: class
superclass: StyleBase
---

# StyleRule

**Inherits**: StyleBase > Instance > Object

## Properties

- **Priority**: `int`
- **Selector**: `string`
- **SelectorError**: `string` [ReadOnly] [NotReplicated]

## Methods

- **GetDefaultPropertyTransition**() -> `Variant`
- **GetProperties**() -> `Dictionary`
- **GetPropertiesResolved**() -> `Dictionary`
- **GetProperty**(`name: string`) -> `Variant`
- **GetPropertyResolved**(`name: string`) -> `Variant`
- **GetPropertyTransitions**() -> `Dictionary`
- **SetDefaultPropertyTransition**(`transitionParams: Variant`) -> `null`
- **SetProperties**(`styleProperties: Dictionary`) -> `null`
- **SetProperty**(`name: string`, `value: Variant`) -> `null`
- **SetPropertyTransition**(`property: string`, `transitionParams: Variant`) -> `null`
- **SetPropertyTransitions**(`properties: Dictionary`) -> `null`

## Events

- **StyleRulePropertyChanged**(`styleProperty: string`)
