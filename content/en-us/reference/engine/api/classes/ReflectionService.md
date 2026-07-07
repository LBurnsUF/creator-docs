---
title: ReflectionService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ReflectionService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **GetClass**(`className: string`, `filter: Dictionary = nil`) -> `Dictionary?` [CustomLuaState]
- **GetClasses**(`filter: Dictionary = nil`) -> `Array` [CustomLuaState]
- **GetEventsOfClass**(`className: string`, `filter: Dictionary = nil`) -> `Array` [CustomLuaState]
- **GetMethodsOfClass**(`className: string`, `filter: Dictionary = nil`) -> `Array` [CustomLuaState]
- **GetPropertiesOfClass**(`className: string`, `filter: Dictionary = nil`) -> `Array` [CustomLuaState]
- **GetPropertyNames**(`name: string`) -> `Array` [CustomLuaState]
- **GetStyledPropertyNames**(`name: string`) -> `Array` [CustomLuaState]
