---
title: PluginToolbarButton
type: class
superclass: Instance
tags: [NotCreatable]
---

# PluginToolbarButton

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

A `PluginToolbarButton` object is created through the
`Class.PluginToolbar:CreateButton()` function. It allows the user to initiate
a single, one-off action in Roblox Studio through the
`Class.PluginToolbarButton.Click|Click` event. Toolbar buttons can also be
assigned a keyboard shortcut through Studio's **File**&nbsp;⟩ **Customize
Shortcuts** window.

When pressed, the `Class.PluginToolbarButton.Click|Click` event fires. A
button will also remain in the pressed state, which may be set manually using
`Class.PluginToolbarButton:SetActive()|SetActive()`. Upon plugin activation
(`Class.Plugin:Activate()`), buttons in all other
`Class.PluginToolbar|PluginToolbars` will be toggled off. If all buttons in a
toolbar are off, the toolbar's plugin is deactivated
(`Class.Plugin:Deactivate()`).

When the game viewport is not visible, buttons will be disabled as if their
`Class.PluginToolbarButton.Enabled|Enabled` property were false. Disabled
buttons are desaturated and do not respond to user clicks. By setting
`Class.PluginToolbarButton.ClickableWhenViewportHidden|ClickableWhenViewportHidden`
to true, you can allow plugin buttons to remain clickable, such as during
script editing.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.PluginToolbarButton.ClickableWhenViewportHidden` | `bool` | [NotReplicated] |
| `Class.PluginToolbarButton.Enabled` | `bool` | [NotReplicated] |
| `Class.PluginToolbarButton.Icon` | `Datatype.ContentId` | [NotReplicated] |
| `Class.PluginToolbarButton.IconContent` | `Datatype.Content` | [NotReplicated] {security: PluginSecurity} |

## Methods

### `Class.PluginToolbarButton:SetActive`

``SetActive(active: `bool`)`` -> `null`
   {security: PluginSecurity}

### `Class.PluginToolbarButton:SetDropdownActive`

``SetDropdownActive(active: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.PluginToolbarButton.Click`

Fires with: ()

### `Class.PluginToolbarButton.DropdownClick`

Fires with: ()
