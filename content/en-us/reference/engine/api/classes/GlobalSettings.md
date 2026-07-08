---
title: GlobalSettings
type: class
superclass: GenericSettings
tags: [NotCreatable, NotBrowsable]
---

# GlobalSettings

Collection of menu settings for Roblox Studio.

**Inherits from:** `Class.GenericSettings` > `Class.ServiceProvider` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotBrowsable]

## Description

The base object used for Roblox Studio's settings menu. Can be accessed by
using the `settings()` function.

## Settings classes under the GlobalSettings

- `Class.DebugSettings`
- `Class.GameSettings`
- `Class.LuaSettings`
- `Class.NetworkSettings`
- `Class.PhysicsSettings`
- `Class.RenderSettings`
- `Class.Studio`

## Methods

### `Class.GlobalSettings:GetFFlag`

``GetFFlag(name: `string`)`` -> `bool`

### `Class.GlobalSettings:GetFFlagOverrides`

``GetFFlagOverrides()`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.GlobalSettings:GetFFlags`

``GetFFlags()`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.GlobalSettings:GetFVariable`

``GetFVariable(name: `string`)`` -> `string`

### `Class.GlobalSettings:SetFFlagOverrides`

``SetFFlagOverrides(overrides: `string`)`` -> `bool`
   {security: RobloxScriptSecurity}
