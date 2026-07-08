---
title: StyleDerive
type: class
superclass: Instance
---

# StyleDerive

When parented to a `Class.StyleSheet`, references another `Class.StyleSheet`
from which the parent inherits `Class.StyleRule|StyleRules` and token
definitions.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

When parented to a `Class.StyleSheet`, references another `Class.StyleSheet`
from which the parent inherits `Class.StyleRule|StyleRules` and token
definitions. Multiple `StyleDerive` instances can exist under a
`Class.StyleSheet` and you can order them by
`Class.StyleDerive.Priority|Priority`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.StyleDerive.Priority` | `int` |  |
| `Class.StyleDerive.StyleSheet` | `Class.StyleSheet` |  |
