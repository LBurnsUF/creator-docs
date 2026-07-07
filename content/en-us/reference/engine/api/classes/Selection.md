---
title: Selection
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# Selection

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Properties

- **ActiveInstance**: `Instance` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **RenderMode**: `SelectionRenderMode` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **SelectionBoxThickness**: `float` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **SelectionLineThickness**: `int` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **SelectionThickness**: `float` [ReadOnly] [NotReplicated]
- **ShowActiveInstanceHighlight**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **Add**(`instancesToAdd: Instances`) -> `null`
- **AddFocusCallback**(`priority: int`, `function: Function`) -> `RBXScriptConnection`
- **ClearTerrainSelectionHack**() -> `null`
- **Get**() -> `Instances`
- **Remove**(`instancesToRemove: Instances`) -> `null`
- **Set**(`selection: Instances`) -> `null`
- **SetTerrainSelectionHack**(`center: Vector3`, `size: Vector3`) -> `null`

## Events

- **SelectionChanged**()
- **SelectionChangedThisFrame**()
