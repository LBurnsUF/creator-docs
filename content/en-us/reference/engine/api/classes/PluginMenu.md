---
title: PluginMenu
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# PluginMenu

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.PluginMenu.Icon` | `string` | [NotReplicated] |
| `Class.PluginMenu.Title` | `string` | [NotReplicated] |
| `Class.PluginMenu.Visible` | `bool` |  {security: RobloxScriptSecurity} |

## Methods

### `Class.PluginMenu:AddAction`

``AddAction(action: `Class.Instance`)`` → `null`
   {security: PluginSecurity}

### `Class.PluginMenu:AddMenu`

``AddMenu(menu: `Class.Instance`)`` → `null`
   {security: PluginSecurity}

### `Class.PluginMenu:AddNewAction`

``AddNewAction(actionId: `string`, text: `string`, icon: `string`)`` → `Class.Instance`
   {security: PluginSecurity}

### `Class.PluginMenu:AddSeparator`

``AddSeparator()`` → `null`
   {security: PluginSecurity}

### `Class.PluginMenu:Clear`

``Clear()`` → `null`
   {security: PluginSecurity}

### `Class.PluginMenu:ShowAsync`

``ShowAsync()`` → `Class.Instance`
  [Yields] {security: PluginSecurity}
