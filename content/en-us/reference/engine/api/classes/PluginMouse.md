---
title: PluginMouse
type: class
superclass: Mouse
tags: [NotCreatable]
---

# PluginMouse

The PluginMouse object gives `Class.Plugin|Plugins` access to the mouse. It
works like the `Class.Mouse` object and can be obtained using the plugin
`Class.Plugin:GetMouse()` method.

**Inherits from:** `Class.Mouse` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

The PluginMouse object gives `Class.Plugin|Plugins` access to the mouse. It
works like the `Class.Mouse` object and can be obtained using the plugin
`Class.Plugin:GetMouse()` method.

Note the PluginMouse can only be used when the plugin has been activated using
`Class.Plugin:Activate()`.

In addition to the functions from the `Class.Mouse` object, the PluginMouse
includes the `Class.PluginMouse.DragEnter` function which keeps track of items
being selected while the mouse is dragging.

For more information on how to use mouse objects, see the `Class.Mouse` page.

## Events

### `Class.PluginMouse.DragEnter`

Fires with: (instances: `Datatype.Instances`)
