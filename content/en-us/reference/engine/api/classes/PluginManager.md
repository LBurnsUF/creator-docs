---
title: PluginManager
type: class
superclass: Instance
tags: [NotCreatable]
---

# PluginManager

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

`PluginManager` is a deprecated singleton that was previously required to
create plugins. It still has some applicable uses, such as if you need to
create a `Class.Plugin` object from Studio's
[Command Bar](../../../studio/ui-overview.md#command-bar).

## Methods

### `Class.PluginManager:CreatePlugin`

``CreatePlugin()`` -> `Class.Instance`
  [Deprecated] [CustomLuaState] {security: PluginSecurity}

### `Class.PluginManager:ExportPlace`

``ExportPlace(filePath: `string`)`` -> `null`
   {security: PluginSecurity}

### `Class.PluginManager:ExportSelection`

``ExportSelection(filePath: `string`)`` -> `null`
   {security: PluginSecurity}
