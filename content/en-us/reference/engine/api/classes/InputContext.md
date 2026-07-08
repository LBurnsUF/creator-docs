---
title: InputContext
type: class
superclass: Instance
---

# InputContext

Collection of actions which holds related actions and defines how they
interact with other contexts/actions.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

An `InputContext` is a collection of actions which holds related
`Class.InputAction|InputActions` and defines how they interact with other
contexts and actions. Nested `InputContext` instances will have no effect and
ordering/priority is managed through `Class.InputContext.Enabled|Enabled`,
`Class.InputContext.Priority|Priority`, and `Class.InputContext.Sink|Sink`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.InputContext.Enabled` | `bool` |  |
| `Class.InputContext.Priority` | `int` |  |
| `Class.InputContext.Sink` | `bool` |  |

## Methods

### `Class.InputContext:GetInputActions`

``GetInputActions()`` -> `Datatype.Instances`
   {security: RobloxScriptSecurity}

## Events

### `Class.InputContext.InputActionsChanged`

Fires with: ()
