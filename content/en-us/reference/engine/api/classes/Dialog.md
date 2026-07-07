---
title: Dialog
type: class
superclass: Instance
---

# Dialog

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
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

``GetCurrentPlayers()`` → `Datatype.Instances`

### `Class.Dialog:SetGuiObject`

``SetGuiObject(gui: `Class.BillboardGui`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Dialog:SetPlayerIsUsing`

``SetPlayerIsUsing(player: `Class.Instance`, isUsing: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Dialog:SignalDialogChoiceSelected`

``SignalDialogChoiceSelected(player: `Class.Instance`, dialogChoice: `Class.Instance`)`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.Dialog.DialogChoiceSelected`

Fires with: (player: `Class.Instance`, dialogChoice: `Class.Instance`)
