---
title: ContextActionService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# ContextActionService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **BindAction**(`actionName: string`, `functionToBind: Function`, `createTouchButton: bool`, `inputTypes: Tuple`) -> `null`
- **BindActionAtPriority**(`actionName: string`, `functionToBind: Function`, `createTouchButton: bool`, `priorityLevel: int`, `inputTypes: Tuple`) -> `null`
- **BindActionToInputTypes**(`actionName: string`, `functionToBind: Function`, `createTouchButton: bool`, `inputTypes: Tuple`) -> `null` [Deprecated]
- **BindActivate**(`userInputTypeForActivation: UserInputType`, `keyCodesForActivation: Tuple`) -> `null`
- **BindCoreAction**(`actionName: string`, `functionToBind: Function`, `createTouchButton: bool`, `inputTypes: Tuple`) -> `null`
- **BindCoreActionAtPriority**(`actionName: string`, `functionToBind: Function`, `createTouchButton: bool`, `priorityLevel: int`, `inputTypes: Tuple`) -> `null`
- **BindCoreActivate**(`userInputTypeForActivation: UserInputType`, `keyCodesForActivation: Tuple`) -> `null`
- **CallFunction**(`actionName: string`, `state: UserInputState`, `inputObject: Instance`) -> `Tuple`
- **FireActionButtonFoundSignal**(`actionName: string`, `actionButton: Instance`) -> `null`
- **GetAllBoundActionInfo**() -> `Dictionary`
- **GetAllBoundCoreActionInfo**() -> `Dictionary`
- **GetBoundActionInfo**(`actionName: string`) -> `Dictionary`
- **GetBoundCoreActionInfo**(`actionName: string`) -> `Dictionary`
- **GetButton**(`actionName: string`) -> `Instance` [Yields]
- **GetCurrentLocalToolIcon**() -> `string`
- **GetInputContexts**() -> `Instances`
- **GetInputSchemaKeyCodeTree**() -> `Dictionary`
- **SetDescription**(`actionName: string`, `description: string`) -> `null`
- **SetImage**(`actionName: string`, `image: string`) -> `null`
- **SetPosition**(`actionName: string`, `position: UDim2`) -> `null`
- **SetTitle**(`actionName: string`, `title: string`) -> `null`
- **UnbindAction**(`actionName: string`) -> `null`
- **UnbindActivate**(`userInputTypeForActivation: UserInputType`, `keyCodeForActivation: KeyCode = Unknown`) -> `null`
- **UnbindAllActions**() -> `null`
- **UnbindCoreAction**(`actionName: string`) -> `null`
- **UnbindCoreActivate**(`userInputTypeForActivation: UserInputType`, `keyCodeForActivation: KeyCode = Unknown`) -> `null`

## Events

- **BoundActionAdded**(`actionAdded: string`, `createTouchButton: bool`, `functionInfoTable: Dictionary`, `isCore: bool`)
- **BoundActionChanged**(`actionChanged: string`, `changeName: string`, `changeTable: Dictionary`)
- **BoundActionRemoved**(`actionRemoved: string`, `functionInfoTable: Dictionary`, `isCore: bool`)
- **GetActionButtonEvent**(`actionName: string`)
- **InputContextsChanged**()
- **LocalToolEquipped**(`toolEquipped: Instance`)
- **LocalToolUnequipped**(`toolUnequipped: Instance`)
