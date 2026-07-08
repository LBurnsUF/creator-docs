---
title: ProximityPromptService
type: class
superclass: Instance
tags: [Service, NotBrowsable]
---

# ProximityPromptService

Allows developers to interact with `Class.ProximityPrompt` objects in a global
way.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [Service] [NotBrowsable]

## Description

**ProximityPromptService** allows developers to interact with
`Class.ProximityPrompt` objects in a global way. It may be more convenient to
listen to events through this service rather than on individual
`Class.ProximityPrompt` objects.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ProximityPromptService.Enabled` | `bool` |  |
| `Class.ProximityPromptService.MaxIndicatorsVisible` | `int` |  |
| `Class.ProximityPromptService.MaxPromptsVisible` | `int` |  |

## Events

### `Class.ProximityPromptService.IndicatorHidden`

Fires with: (prompt: `Class.ProximityPrompt`)

### `Class.ProximityPromptService.IndicatorShown`

Fires with: (prompt: `Class.ProximityPrompt`)

### `Class.ProximityPromptService.PromptButtonHoldBegan`

Fires with: (prompt: `Class.ProximityPrompt`, playerWhoTriggered: `Class.Player`)

### `Class.ProximityPromptService.PromptButtonHoldEnded`

Fires with: (prompt: `Class.ProximityPrompt`, playerWhoTriggered: `Class.Player`)

### `Class.ProximityPromptService.PromptHidden`

Fires with: (prompt: `Class.ProximityPrompt`)

### `Class.ProximityPromptService.PromptShown`

Fires with: (prompt: `Class.ProximityPrompt`, inputType: `Enum.ProximityPromptInputType`)

### `Class.ProximityPromptService.PromptTriggerEnded`

Fires with: (prompt: `Class.ProximityPrompt`, playerWhoTriggered: `Class.Player`)

### `Class.ProximityPromptService.PromptTriggered`

Fires with: (prompt: `Class.ProximityPrompt`, playerWhoTriggered: `Class.Player`)
