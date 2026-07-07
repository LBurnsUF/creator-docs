---
title: ProximityPrompt
type: class
superclass: Instance
---

# ProximityPrompt

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.ProximityPrompt.ActionText` | `string` |  |
| `Class.ProximityPrompt.AutoLocalize` | `bool` |  |
| `Class.ProximityPrompt.ClickablePrompt` | `bool` |  |
| `Class.ProximityPrompt.Enabled` | `bool` |  |
| `Class.ProximityPrompt.Exclusivity` | `Enum.ProximityPromptExclusivity` |  |
| `Class.ProximityPrompt.GamepadKeyCode` | `Enum.KeyCode` |  |
| `Class.ProximityPrompt.HoldDuration` | `float` |  |
| `Class.ProximityPrompt.KeyboardKeyCode` | `Enum.KeyCode` |  |
| `Class.ProximityPrompt.MaxActivationDistance` | `float` |  |
| `Class.ProximityPrompt.MaxIndicatorDistance` | `float` |  |
| `Class.ProximityPrompt.ObjectText` | `string` |  |
| `Class.ProximityPrompt.RequiresLineOfSight` | `bool` |  |
| `Class.ProximityPrompt.RootLocalizationTable` | `Class.LocalizationTable` |  |
| `Class.ProximityPrompt.Style` | `Enum.ProximityPromptStyle` |  |
| `Class.ProximityPrompt.UIOffset` | `Datatype.Vector2` |  |

## Methods

### `Class.ProximityPrompt:InputHoldBegin`

``InputHoldBegin()`` → `null`

### `Class.ProximityPrompt:InputHoldEnd`

``InputHoldEnd()`` → `null`

## Events

### `Class.ProximityPrompt.IndicatorHidden`

Fires with: ()

### `Class.ProximityPrompt.IndicatorShown`

Fires with: ()

### `Class.ProximityPrompt.PromptButtonHoldBegan`

Fires with: (playerWhoTriggered: `Class.Player`)

### `Class.ProximityPrompt.PromptButtonHoldEnded`

Fires with: (playerWhoTriggered: `Class.Player`)

### `Class.ProximityPrompt.PromptHidden`

Fires with: ()

### `Class.ProximityPrompt.PromptShown`

Fires with: (inputType: `Enum.ProximityPromptInputType`)

### `Class.ProximityPrompt.TriggerEnded`

Fires with: (playerWhoTriggered: `Class.Player`)

### `Class.ProximityPrompt.Triggered`

Fires with: (playerWhoTriggered: `Class.Player`)
