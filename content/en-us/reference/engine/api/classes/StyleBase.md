---
title: StyleBase
type: class
superclass: Instance
tags: [NotCreatable]
---

# StyleBase

The base class for `Class.StyleSheet` and `Class.StyleRule`.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

The base class for `Class.StyleSheet` and `Class.StyleRule`. Holds a list of
child `Class.StyleRule|StyleRules`, as well as token definitions which are
stored as [attributes](../../../studio/properties.md#instance-attributes).

## Methods

### `Class.StyleBase:GetStyleRules`

``GetStyleRules()`` -> `Datatype.Instances`

### `Class.StyleBase:InsertStyleRule`

``InsertStyleRule(rule: `Class.StyleRule`, priority: `int?`)`` -> `null`

### `Class.StyleBase:SetStyleRules`

``SetStyleRules(rules: `Datatype.Instances`)`` -> `null`

## Events

### `Class.StyleBase.StyleRulesChanged`

Fires with: ()
