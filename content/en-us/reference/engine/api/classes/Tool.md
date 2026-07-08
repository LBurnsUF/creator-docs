---
title: Tool
type: class
superclass: BackpackItem
---

# Tool

An object, such as a weapon, that can be equipped by a `Class.Humanoid`.

**Inherits from:** `Class.BackpackItem` > `Class.Model` > `Class.PVInstance` > `Class.Instance` > `Class.Object`

## Description

A `Tool` is an object that a `Class.Humanoid` object can equip. For players,
they are stored in a `Class.Backpack` object parented to a `Class.Player`
object. In-experience, players may have multiple tools which appear as icons
at the bottom of the screen. Equipping a tool moves it from the
`Class.Backpack` and into a `Class.Player.Character` model in the
`Class.Workspace`. By default, tools are held in the right hand and have a
handle in them, which is a `Class.BasePart` named `Handle` inside (although
one isn't required if `Class.Tool.RequiresHandle` is `false`). Tools that are
to be provided to (re)spawning players should be stored in the
`Class.StarterPack`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Tool.CanBeDropped` | `bool` |  |
| `Class.Tool.Enabled` | `bool` |  |
| `Class.Tool.Grip` | `Datatype.CFrame` |  |
| `Class.Tool.GripForward` | `Datatype.Vector3` | [Hidden] [NotReplicated] |
| `Class.Tool.GripPos` | `Datatype.Vector3` | [Hidden] [NotReplicated] |
| `Class.Tool.GripRight` | `Datatype.Vector3` | [Hidden] [NotReplicated] |
| `Class.Tool.GripUp` | `Datatype.Vector3` | [Hidden] [NotReplicated] |
| `Class.Tool.ManualActivationOnly` | `bool` |  |
| `Class.Tool.RequiresHandle` | `bool` |  |
| `Class.Tool.ToolTip` | `string` |  |

## Methods

### `Class.Tool:Activate`

``Activate()`` -> `null`

### `Class.Tool:Deactivate`

``Deactivate()`` -> `null`

## Events

### `Class.Tool.Activated`

Fires with: ()

### `Class.Tool.Deactivated`

Fires with: ()

### `Class.Tool.Equipped`

Fires with: (mouse: `Class.Mouse`)

### `Class.Tool.Unequipped`

Fires with: ()
