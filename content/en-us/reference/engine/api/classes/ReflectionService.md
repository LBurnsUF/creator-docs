---
title: ReflectionService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ReflectionService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.ReflectionService:GetClass`

``GetClass(className: `string`, filter: `Dictionary`)`` → `Dictionary?`
  [CustomLuaState]

### `Class.ReflectionService:GetClasses`

``GetClasses(filter: `Dictionary`)`` → `Array`
  [CustomLuaState]

### `Class.ReflectionService:GetEventsOfClass`

``GetEventsOfClass(className: `string`, filter: `Dictionary`)`` → `Array`
  [CustomLuaState]

### `Class.ReflectionService:GetMethodsOfClass`

``GetMethodsOfClass(className: `string`, filter: `Dictionary`)`` → `Array`
  [CustomLuaState]

### `Class.ReflectionService:GetPropertiesOfClass`

``GetPropertiesOfClass(className: `string`, filter: `Dictionary`)`` → `Array`
  [CustomLuaState]

### `Class.ReflectionService:GetPropertyNames`

``GetPropertyNames(name: `string`)`` → `Array`
  [CustomLuaState] {security: RobloxScriptSecurity}

### `Class.ReflectionService:GetStyledPropertyNames`

``GetStyledPropertyNames(name: `string`)`` → `Array`
  [CustomLuaState] {security: RobloxScriptSecurity}
