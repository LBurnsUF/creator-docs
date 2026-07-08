---
title: PluginAction
type: class
superclass: Instance
tags: [NotReplicated]
---

# PluginAction

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotReplicated]

## Description

`PluginAction` represents a generic performable action in Studio with no
directly‑associated `Class.PluginToolbarButton`. If
`Class.PluginAction.AllowBinding|AllowBinding` is `true`, the action can be
assigned a keyboard shortcut through Studio's **File**&nbsp;⟩ **Customize
Shortcuts** window.

A `PluginAction` must be created using the `Class.Plugin:CreatePluginAction()`
method in order to work as expected.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.PluginAction.ActionId` | `string` | [ReadOnly] [NotReplicated] |
| `Class.PluginAction.AllowBinding` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.PluginAction.Checked` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.PluginAction.DefaultShortcut` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.PluginAction.Enabled` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.PluginAction.StatusTip` | `string` | [ReadOnly] [NotReplicated] |
| `Class.PluginAction.Text` | `string` | [NotReplicated] {write: RobloxScriptSecurity} |
| `Class.PluginAction.Visible` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |

## Events

### `Class.PluginAction.Triggered`

Fires with: ()
