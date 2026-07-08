---
title: PluginConnectionService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# PluginConnectionService

This service is used by plugins to communicate with other instances of
themselves running in other data models.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

This service is used by plugins to communicate with other instances of
themselves running in other data models (e.g. a plugin in the Studio edit data
model can communicate with the instance of that same plugin in the Studio
playtest Server data model). Plugins can retrieve `Class.PluginConnection`
objects from this service, which provide an API for sending messages across
the data model boundary. All access to this class is restricted to Plugin
security. The command bar is not currently supported.

## Methods

### `Class.PluginConnectionService:CanHaveConnectionType`

``CanHaveConnectionType(type: `Enum.PluginConnectionTargetType`)`` -> `bool`
   {security: PluginSecurity}

### `Class.PluginConnectionService:GetPluginConnectionsOfType`

``GetPluginConnectionsOfType(type: `Enum.PluginConnectionTargetType`)`` -> `Array`
   {security: PluginSecurity}

## Events

### `Class.PluginConnectionService.Connected`

Fires with: (conn: `Class.PluginConnection`)
