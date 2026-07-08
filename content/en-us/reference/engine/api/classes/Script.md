---
title: Script
type: class
superclass: BaseScript
---

# Script

An object that contains and runs Luau code on the server.

**Inherits from:** `Class.BaseScript` > `Class.LuaSourceContainer` > `Class.Instance` > `Class.Object`

## Description

A `Class.Script` is a Luau source container that can access server-side
objects, properties, and events, such as to award badges to players using
`Class.BadgeService`, while `Class.LocalScript|LocalScripts` on the client
cannot.

The instant that the following conditions are met, a script's code is run in a
new thread:

- Its `Class.Script.Enabled|Enabled` property is `true`.
- The `Class.Script` object is a descendant of the `Class.Workspace` or
  `Class.ServerScriptService`.

The script will continue to run until the above conditions are **not** met, it
terminates, or it raises an error (unless that error is raised by a function
connected to some event that is firing). Additionally, the thread will be
stopped if the script or one of its ancestors is destroyed. A script will
continue to run even if the `Class.Instance.Parent|Parent` property is set to
`nil` and the `Class.Script` is not destroyed.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Script.Source` | `Datatype.ProtectedString` |  |

## Methods

### `Class.Script:GetHash`

``GetHash()`` -> `string`
   {security: LocalUserSecurity}
