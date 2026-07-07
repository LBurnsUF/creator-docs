---
title: Dialog
type: class
superclass: Instance
---

# Dialog

**Inherits**: Instance > Object

## Properties

- **BehaviorType**: `DialogBehaviorType`
- **ConversationDistance**: `float`
- **GoodbyeChoiceActive**: `bool`
- **GoodbyeDialog**: `string`
- **InUse**: `bool`
- **InitialPrompt**: `string`
- **Purpose**: `DialogPurpose`
- **Tone**: `DialogTone`
- **TriggerDistance**: `float`
- **TriggerOffset**: `Vector3`

## Methods

- **GetCurrentPlayers**() -> `Instances`
- **SetGuiObject**(`gui: BillboardGui`) -> `null`
- **SetPlayerIsUsing**(`player: Instance`, `isUsing: bool`) -> `null`
- **SignalDialogChoiceSelected**(`player: Instance`, `dialogChoice: Instance`) -> `null`

## Events

- **DialogChoiceSelected**(`player: Instance`, `dialogChoice: Instance`)
