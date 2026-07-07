---
title: Object
type: class
superclass: <<<ROOT>>>
tags: [NotCreatable, NotReplicated]
---

# Object

**Tags**: NotCreatable, NotReplicated

## Properties

- **ClassName**: `string` [ReadOnly] [NotReplicated]
- **className**: `string` [ReadOnly] [NotReplicated] [Deprecated]

## Methods

- **GetPropertyChangedSignal**(`property: string`) -> `RBXScriptSignal`
- **IsA**(`className: string`) -> `bool` [CustomLuaState]
- **isA**(`className: string`) -> `bool` [Deprecated] [CustomLuaState]

## Events

- **Changed**(`property: string`)
