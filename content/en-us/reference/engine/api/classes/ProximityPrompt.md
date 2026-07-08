---
title: ProximityPrompt
type: class
superclass: Instance
---

# ProximityPrompt

An object that lets you prompt players to interact with an object in the 3D
world.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

The **ProximityPrompt** instance lets you prompt players to interact with an
object in the 3D world, such as opening a door or picking up an item. A
`Class.ProximityPrompt` object works when parented to a `Class.BasePart`,
`Class.Attachment`, or `Class.Model` (with
`Class.Model.PrimaryPart|PrimaryPart` set) in the workspace. When the player's
character approaches, a UI appears to prompt them for input.

Prompts consist of three primary elements, each of which can be controlled by
the noted properties. The default UI can be swapped out for your own custom
appearance as outlined in `Class.ProximityPrompt.Style|Style`.

<img src="../../../assets/ui/proximity-prompt/Prompt-Diagram.png" width="600" />

<table>
<thead>
  <tr>
    <td>Property</td>
    <td>Description</td>
    <td>Default</td>
  </tr>
</thead>
<tbody>
  <tr>
    <td><code>Class.ProximityPrompt.ObjectText|ObjectText</code></td>
    <td>An optional name for the object being interacted with.</td>
    <td></td>
  </tr>
  <tr>
    <td><code>Class.ProximityPrompt.ActionText|ActionText</code></td>
    <td>An optional action name shown to the player.</td>
    <td>Interact</td>
  </tr>
  <tr>
    <td><code>Class.ProximityPrompt.KeyboardKeyCode|KeyboardKeyCode</code></td>
    <td>The keyboard key which will trigger the prompt.</td>
    <td>E</td>
  </tr>
  <tr>
    <td><code>Class.ProximityPrompt.GamepadKeyCode|GamepadKeyCode</code></td>
    <td>The gamepad button which will trigger the prompt.</td>
    <td>ButtonX</td>
  </tr>
</tbody>
</table>

You can connect to proximity prompt events either on the
`Class.ProximityPrompt` object itself or globally through
`Class.ProximityPromptService`. The `Class.ProximityPromptService` allows you
to manage all proximity prompt behavior from one location, preventing any need
for duplicate code in your experience.

For more information regarding proximity prompts, see the
[Proximity Prompts](../../../ui/proximity-prompts.md) guide.

## Properties

| Property | Type | Description |
|----------|------|-------------|
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

``InputHoldBegin()`` -> `null`

### `Class.ProximityPrompt:InputHoldEnd`

``InputHoldEnd()`` -> `null`

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
