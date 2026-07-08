---
title: ReflectionService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ReflectionService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

`ReflectionService` allows scripts to query the engine for details about its
API, including required security permissions, functionality, and inheritance
structure. You can use this service to dynamically inspect classes and their
properties, methods, and events, which can be useful for debugging, tooling,
or creating dynamic behaviors based on the engine's capabilities.

The following is an example script that inspects classes and their properties:

```lua
local ReflectionService = game:GetService("ReflectionService")

-- Create a SecurityCapabilities object with all capabilities
local allCapabilities = SecurityCapabilities.new(table.unpack(Enum.SecurityCapability:GetEnumItems()))

-- Get all classes accessible with all capabilities
local allClasses = ReflectionService:GetClasses({ Security = allCapabilities })
print("Total classes:", #allClasses)

-- Get a specific class
local partClass = ReflectionService:GetClass("Part")
if partClass then
	print("\nPart class:")
	print("  Name:", partClass.Name)
	print("  Superclass:", partClass.Superclass and tostring(partClass.Superclass) or "none")
end

-- Get the first 5 properties of a class
local properties = ReflectionService:GetPropertiesOfClass("Part", { Security = allCapabilities })
print("\nPart properties:", #properties)
for i = 1, math.min(5, #properties) do
	print("  -", properties[i].Name)
end
```

## Methods

### `Class.ReflectionService:GetClass`

``GetClass(className: `string`, filter: `Dictionary`)`` -> `Dictionary?`
  [CustomLuaState]

### `Class.ReflectionService:GetClasses`

``GetClasses(filter: `Dictionary`)`` -> `Array`
  [CustomLuaState]

### `Class.ReflectionService:GetEventsOfClass`

``GetEventsOfClass(className: `string`, filter: `Dictionary`)`` -> `Array`
  [CustomLuaState]

### `Class.ReflectionService:GetMethodsOfClass`

``GetMethodsOfClass(className: `string`, filter: `Dictionary`)`` -> `Array`
  [CustomLuaState]

### `Class.ReflectionService:GetPropertiesOfClass`

``GetPropertiesOfClass(className: `string`, filter: `Dictionary`)`` -> `Array`
  [CustomLuaState]

### `Class.ReflectionService:GetPropertyNames`

``GetPropertyNames(name: `string`)`` -> `Array`
  [CustomLuaState] {security: RobloxScriptSecurity}

### `Class.ReflectionService:GetStyledPropertyNames`

``GetStyledPropertyNames(name: `string`)`` -> `Array`
  [CustomLuaState] {security: RobloxScriptSecurity}
