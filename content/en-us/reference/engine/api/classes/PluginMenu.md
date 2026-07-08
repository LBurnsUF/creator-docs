---
title: PluginMenu
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# PluginMenu

A context menu that can be shown in Studio. Displays a list of
`Class.PluginAction|PluginActions` and supports submenus.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

`PluginMenu` represents a context menu which can be shown in Studio to display
a list of `Class.PluginAction|PluginActions` and which also supports submenus.
A `PluginMenu` must be created using the `Class.Plugin:CreatePluginMenu()`
method in order to work as expected.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.PluginMenu.Icon` | `string` | [NotReplicated] |
| `Class.PluginMenu.Title` | `string` | [NotReplicated] |
| `Class.PluginMenu.Visible` | `bool` |  {security: RobloxScriptSecurity} |

## Methods

### `Class.PluginMenu:AddAction`

``AddAction(action: `Class.Instance`)`` -> `null`
   {security: PluginSecurity}

### `Class.PluginMenu:AddMenu`

``AddMenu(menu: `Class.Instance`)`` -> `null`
   {security: PluginSecurity}

### `Class.PluginMenu:AddNewAction`

``AddNewAction(actionId: `string`, text: `string`, icon: `string`)`` -> `Class.Instance`
   {security: PluginSecurity}

### `Class.PluginMenu:AddSeparator`

``AddSeparator()`` -> `null`
   {security: PluginSecurity}

### `Class.PluginMenu:Clear`

``Clear()`` -> `null`
   {security: PluginSecurity}

### `Class.PluginMenu:ShowAsync`

``ShowAsync()`` -> `Class.Instance`
  [Yields] {security: PluginSecurity}
