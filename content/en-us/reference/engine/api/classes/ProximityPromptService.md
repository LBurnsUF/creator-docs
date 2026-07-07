---
title: ProximityPromptService
type: class
superclass: Instance
tags: [Service, NotBrowsable]
---

# ProximityPromptService

**Inherits**: Instance > Object

**Tags**: Service, NotBrowsable

## Properties

- **Enabled**: `bool`
- **MaxIndicatorsVisible**: `int`
- **MaxPromptsVisible**: `int`

## Events

- **IndicatorHidden**(`prompt: ProximityPrompt`)
- **IndicatorShown**(`prompt: ProximityPrompt`)
- **PromptButtonHoldBegan**(`prompt: ProximityPrompt`, `playerWhoTriggered: Player`)
- **PromptButtonHoldEnded**(`prompt: ProximityPrompt`, `playerWhoTriggered: Player`)
- **PromptHidden**(`prompt: ProximityPrompt`)
- **PromptShown**(`prompt: ProximityPrompt`, `inputType: ProximityPromptInputType`)
- **PromptTriggerEnded**(`prompt: ProximityPrompt`, `playerWhoTriggered: Player`)
- **PromptTriggered**(`prompt: ProximityPrompt`, `playerWhoTriggered: Player`)
