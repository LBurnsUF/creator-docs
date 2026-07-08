---
title: InputObject
type: class
superclass: Instance
tags: [NotCreatable]
---

# InputObject

An object created when an input begins that describes a particular user input.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

An `InputObject` represents a single user input, such as mouse movement,
touches, key presses and more. It is created when an input begins.

The properties of this object vary according the
`Class.InputObject.UserInputType|UserInputType`. Each kind of input will
undergo various changes to its
`Class.InputObject.UserInputState|UserInputState`. During the lifetime of an
input, other properties which further describe the input may change, such as
`Class.InputObject.Position|Position` and `Class.InputObject.Delta|Delta`.
Keyboard and gamepad button presses will have the
`Class.InputObject.KeyCode|KeyCode` property set.

Once created at the beginning of an input, the same object persists and is
updated until the input ends. As a result, you can track the object's changes
using the `Class.Object.Changed|Changed` event as the user changes the input
in question. You can also place these objects into a list of active inputs
track and interact with the object after it's creation by an event such as
`Class.UserInputService.InputBegan`. This is mostly useful for touch events,
as each touch point will have a separate `InputObject`.

See also `Class.UserInputService` whose events and functions often use
`InputObject`, and `Class.GuiObject` whose events related to user input use
`InputObject`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.InputObject.Delta` | `Datatype.Vector3` |  |
| `Class.InputObject.KeyCode` | `Enum.KeyCode` |  |
| `Class.InputObject.Position` | `Datatype.Vector3` |  |
| `Class.InputObject.UserInputState` | `Enum.UserInputState` |  |
| `Class.InputObject.UserInputType` | `Enum.UserInputType` |  |

## Methods

### `Class.InputObject:IsModifierKeyDown`

``IsModifierKeyDown(modifierKey: `Enum.ModifierKey`)`` -> `bool`
