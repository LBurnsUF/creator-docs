---
title: UserSettings
type: class
superclass: GenericSettings
tags: [NotCreatable]
---

# UserSettings

A singleton object that houses basic user settings, which persist across all
games on Roblox.

**Inherits from:** `Class.GenericSettings` > `Class.ServiceProvider` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

UserSettings is a singleton object that is used to house basic user settings,
which persist across all games. Currently, it only stores the
`Class.UserGameSettings` object.

You can retrieve a reference to this object via the
`Class.UserSettings|UserSettings()` function, which returns it.

## Methods

### `Class.UserSettings:IsUserFeatureEnabled`

``IsUserFeatureEnabled(name: `string`)`` -> `bool`

### `Class.UserSettings:Reset`

``Reset()`` -> `null`

### `Class.UserSettings:SaveState`

``SaveState()`` -> `null`
   {security: RobloxScriptSecurity}
