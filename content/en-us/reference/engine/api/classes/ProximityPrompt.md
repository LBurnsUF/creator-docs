---
title: ProximityPrompt
type: class
superclass: Instance
---

# ProximityPrompt

**Inherits**: Instance > Object

## Properties

- **ActionText**: `string`
- **AutoLocalize**: `bool`
- **ClickablePrompt**: `bool`
- **Enabled**: `bool`
- **Exclusivity**: `ProximityPromptExclusivity`
- **GamepadKeyCode**: `KeyCode`
- **HoldDuration**: `float`
- **KeyboardKeyCode**: `KeyCode`
- **MaxActivationDistance**: `float`
- **MaxIndicatorDistance**: `float`
- **ObjectText**: `string`
- **RequiresLineOfSight**: `bool`
- **RootLocalizationTable**: `LocalizationTable`
- **Style**: `ProximityPromptStyle`
- **UIOffset**: `Vector2`

## Methods

- **InputHoldBegin**() -> `null`
- **InputHoldEnd**() -> `null`

## Events

- **IndicatorHidden**()
- **IndicatorShown**()
- **PromptButtonHoldBegan**(`playerWhoTriggered: Player`)
- **PromptButtonHoldEnded**(`playerWhoTriggered: Player`)
- **PromptHidden**()
- **PromptShown**(`inputType: ProximityPromptInputType`)
- **TriggerEnded**(`playerWhoTriggered: Player`)
- **Triggered**(`playerWhoTriggered: Player`)
