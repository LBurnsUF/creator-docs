---
title: ConfigSnapshot
type: class
superclass: Object
tags: [NotCreatable, NotReplicated]
---

# ConfigSnapshot

**Inherits**: Object

**Tags**: NotCreatable, NotReplicated

## Properties

- **Error**: `ConfigSnapshotErrorState` [ReadOnly] [NotReplicated]
- **Outdated**: `bool` [ReadOnly] [NotReplicated]

## Methods

- **GetValue**(`key: string`) -> `Variant`
- **GetValueChangedSignal**(`key: string`) -> `RBXScriptSignal`
- **Refresh**() -> `null`

## Events

- **UpdateAvailable**()
