---
title: MemStorageService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# MemStorageService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.MemStorageService:Bind`

``Bind(key: `string`, callback: `Datatype.Function`)`` → `Class.MemStorageConnection`
   {security: RobloxScriptSecurity}

### `Class.MemStorageService:BindAndFire`

``BindAndFire(key: `string`, callback: `Datatype.Function`)`` → `Class.MemStorageConnection`
   {security: RobloxScriptSecurity}

### `Class.MemStorageService:Call`

``Call(key: `string`, input: `Variant`)`` → `Variant`
   {security: RobloxScriptSecurity}

### `Class.MemStorageService:Fire`

``Fire(key: `string`, value: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.MemStorageService:GetItem`

``GetItem(key: `string`, defaultValue: `string`)`` → `string`
   {security: RobloxScriptSecurity}

### `Class.MemStorageService:HasItem`

``HasItem(key: `string`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.MemStorageService:RemoveItem`

``RemoveItem(key: `string`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.MemStorageService:SetItem`

``SetItem(key: `string`, value: `string`)`` → `null`
   {security: RobloxScriptSecurity}
