---
title: PluginToolbar
type: class
superclass: Instance
tags: [NotCreatable]
---

# PluginToolbar

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

A `PluginToolbar` object is created by calling the
`Class.Plugin:CreateToolbar()` method and is used to contain
`Class.PluginToolbarButton|PluginToolbarButtons`.

## Methods

### `Class.PluginToolbar:CreateButton`

``CreateButton(buttonId: `string`, tooltip: `string`, iconname: `string`, text: `string`)`` -> `Class.PluginToolbarButton`
   {security: PluginSecurity}

### `Class.PluginToolbar:CreatePopupButton`

``CreatePopupButton(buttonId: `string`, tooltip: `string`, iconname: `string`, text: `string`)`` -> `Class.PluginToolbarButton`
   {security: RobloxScriptSecurity}
