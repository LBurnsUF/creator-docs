---
title: Dialog
type: class
superclass: Instance
---

# Dialog

Creates NPC billboard-style dialog bubbles.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

The Dialog object allows users to create non-player characters (NPCs) that
players can talk to using a list of choices. The Dialog object can be inserted
into a part such as a Humanoid's head, and then a player will see a speech
bubble above the part that they can click on to start a conversation. The
creator of a place can choose what choices the player can say by inserting
`Class.DialogChoice` objects into the dialog.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Dialog.BehaviorType` | `Enum.DialogBehaviorType` |  |
| `Class.Dialog.ConversationDistance` | `float` |  |
| `Class.Dialog.GoodbyeChoiceActive` | `bool` |  |
| `Class.Dialog.GoodbyeDialog` | `string` |  |
| `Class.Dialog.InUse` | `bool` |  |
| `Class.Dialog.InitialPrompt` | `string` |  |
| `Class.Dialog.Purpose` | `Enum.DialogPurpose` |  |
| `Class.Dialog.Tone` | `Enum.DialogTone` |  |
| `Class.Dialog.TriggerDistance` | `float` |  |
| `Class.Dialog.TriggerOffset` | `Datatype.Vector3` |  |

## Methods

### `Class.Dialog:GetCurrentPlayers`

``GetCurrentPlayers()`` -> `Datatype.Instances`

### `Class.Dialog:SetGuiObject`

``SetGuiObject(gui: `Class.BillboardGui`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.Dialog:SetPlayerIsUsing`

``SetPlayerIsUsing(player: `Class.Instance`, isUsing: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.Dialog:SignalDialogChoiceSelected`

``SignalDialogChoiceSelected(player: `Class.Instance`, dialogChoice: `Class.Instance`)`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.Dialog.DialogChoiceSelected`

Fires with: (player: `Class.Instance`, dialogChoice: `Class.Instance`)
