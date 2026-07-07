---
title: Tool
type: class
superclass: BackpackItem
---

# Tool

**Inherits**: BackpackItem > Model > PVInstance > Instance > Object

## Properties

- **CanBeDropped**: `bool`
- **Enabled**: `bool`
- **Grip**: `CFrame`
- **GripForward**: `Vector3` [Hidden] [NotReplicated]
- **GripPos**: `Vector3` [Hidden] [NotReplicated]
- **GripRight**: `Vector3` [Hidden] [NotReplicated]
- **GripUp**: `Vector3` [Hidden] [NotReplicated]
- **ManualActivationOnly**: `bool`
- **RequiresHandle**: `bool`
- **ToolTip**: `string`

## Methods

- **Activate**() -> `null`
- **Deactivate**() -> `null`

## Events

- **Activated**()
- **Deactivated**()
- **Equipped**(`mouse: Mouse`)
- **Unequipped**()
