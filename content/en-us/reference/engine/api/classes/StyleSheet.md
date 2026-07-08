---
title: StyleSheet
type: class
superclass: StyleBase
---

# StyleSheet

Aggregates `Class.StyleRule|StyleRules` and can be linked to `Class.DataModel`
trees to apply style properties to instances.

**Inherits from:** `Class.StyleBase` > `Class.Instance` > `Class.Object`

## Description

Aggregates `Class.StyleRule|StyleRules` and can be linked to `Class.DataModel`
trees to apply style properties to instances. Note that a `StyleSheet` may
exist outside the `Class.DataModel`, but it cannot be derived or linked to a
`Class.DataModel` tree in such a case.

## Methods

### `Class.StyleSheet:GetDerives`

``GetDerives()`` -> `Datatype.Instances`

### `Class.StyleSheet:SetDerives`

``SetDerives(derives: `Datatype.Instances`)`` -> `null`
