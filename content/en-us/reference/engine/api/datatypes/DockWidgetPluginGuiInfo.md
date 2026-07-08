---
title: DockWidgetPluginGuiInfo
type: datatype
---

# `Datatype.DockWidgetPluginGuiInfo`

Describes details for a `Class.DockWidgetPluginGui`.

## Description

The `Datatype.DockWidgetPluginGuiInfo` data type describes details for a
`Class.DockWidgetPluginGui`. This data type is used when constructing a
`Class.PluginGui` via the plugin's
`Class.Plugin:CreateDockWidgetPluginGuiAsync()` method.

## Constructors

### `DockWidgetPluginGuiInfo.new`

The main constructor function for the `Datatype.DockWidgetPluginGuiInfo`.

**Parameters:**

- `InitialDockState`: `InitialDockState`
- `InitialEnabled`: `bool`
- `InitialEnabledShouldOverrideRestore`: `bool`
- `FloatingXSize`: `number`
- `FloatingYSize`: `number`
- `MinWidth`: `number`
- `MinHeight`: `number`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `DockWidgetPluginGuiInfo.InitialEnabled` | `bool` | The enabled state of the `Class.PluginGui` if it does not have a saved state from a previous session |
| `DockWidgetPluginGuiInfo.InitialEnabledShouldOverrideRestore` | `bool` | If true, will override any saved enabled state with the `InitialEnabled` value. |
| `DockWidgetPluginGuiInfo.FloatingXSize` | `number` | The initial pixel width of the PluginGui when floating. |
| `DockWidgetPluginGuiInfo.FloatingYSize` | `number` | The initial pixel height of the PluginGui when floating. |
| `DockWidgetPluginGuiInfo.MinWidth` | `number` | The minimum pixel width of the PluginGui. |
| `DockWidgetPluginGuiInfo.MinHeight` | `number` | The minimum pixel height of the PluginGui. |

## API Usage (2 locations)

### Used as Parameter Type

- `Class.Plugin:CreateDockWidgetPluginGui` (parameter `dockWidgetPluginGuiInfo`)
- `Class.Plugin:CreateDockWidgetPluginGuiAsync` (parameter `dockWidgetPluginGuiInfo`)
