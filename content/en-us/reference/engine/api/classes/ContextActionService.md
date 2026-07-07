---
title: ContextActionService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# ContextActionService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Methods

### `Class.ContextActionService:BindAction`

``BindAction(actionName: `string`, functionToBind: `Datatype.Function`, createTouchButton: `bool`, inputTypes: `Tuple`)`` → `null`

### `Class.ContextActionService:BindActionAtPriority`

``BindActionAtPriority(actionName: `string`, functionToBind: `Datatype.Function`, createTouchButton: `bool`, priorityLevel: `int`, inputTypes: `Tuple`)`` → `null`

### `Class.ContextActionService:BindActionToInputTypes`

``BindActionToInputTypes(actionName: `string`, functionToBind: `Datatype.Function`, createTouchButton: `bool`, inputTypes: `Tuple`)`` → `null`
  [Deprecated]

### `Class.ContextActionService:BindActivate`

``BindActivate(userInputTypeForActivation: `Enum.UserInputType`, keyCodesForActivation: `Tuple`)`` → `null`

### `Class.ContextActionService:BindCoreAction`

``BindCoreAction(actionName: `string`, functionToBind: `Datatype.Function`, createTouchButton: `bool`, inputTypes: `Tuple`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.ContextActionService:BindCoreActionAtPriority`

``BindCoreActionAtPriority(actionName: `string`, functionToBind: `Datatype.Function`, createTouchButton: `bool`, priorityLevel: `int`, inputTypes: `Tuple`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.ContextActionService:BindCoreActivate`

``BindCoreActivate(userInputTypeForActivation: `Enum.UserInputType`, keyCodesForActivation: `Tuple`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.ContextActionService:CallFunction`

``CallFunction(actionName: `string`, state: `Enum.UserInputState`, inputObject: `Class.Instance`)`` → `Tuple`
   {security: RobloxScriptSecurity}

### `Class.ContextActionService:FireActionButtonFoundSignal`

``FireActionButtonFoundSignal(actionName: `string`, actionButton: `Class.Instance`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.ContextActionService:GetAllBoundActionInfo`

``GetAllBoundActionInfo()`` → `Dictionary`

### `Class.ContextActionService:GetAllBoundCoreActionInfo`

``GetAllBoundCoreActionInfo()`` → `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.ContextActionService:GetBoundActionInfo`

``GetBoundActionInfo(actionName: `string`)`` → `Dictionary`

### `Class.ContextActionService:GetBoundCoreActionInfo`

``GetBoundCoreActionInfo(actionName: `string`)`` → `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.ContextActionService:GetButton`

``GetButton(actionName: `string`)`` → `Class.Instance`
  [Yields]

### `Class.ContextActionService:GetCurrentLocalToolIcon`

``GetCurrentLocalToolIcon()`` → `string`

### `Class.ContextActionService:GetInputContexts`

``GetInputContexts()`` → `Datatype.Instances`
   {security: RobloxScriptSecurity}

### `Class.ContextActionService:GetInputSchemaKeyCodeTree`

``GetInputSchemaKeyCodeTree()`` → `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.ContextActionService:SetDescription`

``SetDescription(actionName: `string`, description: `string`)`` → `null`

### `Class.ContextActionService:SetImage`

``SetImage(actionName: `string`, image: `string`)`` → `null`

### `Class.ContextActionService:SetPosition`

``SetPosition(actionName: `string`, position: `Datatype.UDim2`)`` → `null`

### `Class.ContextActionService:SetTitle`

``SetTitle(actionName: `string`, title: `string`)`` → `null`

### `Class.ContextActionService:UnbindAction`

``UnbindAction(actionName: `string`)`` → `null`

### `Class.ContextActionService:UnbindActivate`

``UnbindActivate(userInputTypeForActivation: `Enum.UserInputType`, keyCodeForActivation: `Enum.KeyCode`)`` → `null`

### `Class.ContextActionService:UnbindAllActions`

``UnbindAllActions()`` → `null`

### `Class.ContextActionService:UnbindCoreAction`

``UnbindCoreAction(actionName: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.ContextActionService:UnbindCoreActivate`

``UnbindCoreActivate(userInputTypeForActivation: `Enum.UserInputType`, keyCodeForActivation: `Enum.KeyCode`)`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.ContextActionService.BoundActionAdded`

Fires with: (actionAdded: `string`, createTouchButton: `bool`, functionInfoTable: `Dictionary`, isCore: `bool`)

### `Class.ContextActionService.BoundActionChanged`

Fires with: (actionChanged: `string`, changeName: `string`, changeTable: `Dictionary`)

### `Class.ContextActionService.BoundActionRemoved`

Fires with: (actionRemoved: `string`, functionInfoTable: `Dictionary`, isCore: `bool`)

### `Class.ContextActionService.GetActionButtonEvent`

Fires with: (actionName: `string`)

### `Class.ContextActionService.InputContextsChanged`

Fires with: ()

### `Class.ContextActionService.LocalToolEquipped`

Fires with: (toolEquipped: `Class.Instance`)

### `Class.ContextActionService.LocalToolUnequipped`

Fires with: (toolUnequipped: `Class.Instance`)
