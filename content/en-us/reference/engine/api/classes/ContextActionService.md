---
title: ContextActionService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# ContextActionService

A service used to bind user input to contextual actions.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

Allows an experience to bind user input to contextual actions, or actions that
are only enabled under some condition or period of time. For example, allowing
a player to open a door only while close by. In code, an action is simply a
string (the name of the action) used by the service to differentiate between
unique actions. The action string is provided to
`Class.ContextActionService:BindAction()|BindAction` and
`Class.ContextActionService:UnbindAction()|UnbindAction`, among other member
functions. If two actions are bound to the same input, the most recently bound
will take priority. When the most recent action is unbound, the one bound
before that takes control again. Since this service deals with user input, you
can only use it in client-side `Class.LocalScript|LocalScripts`.

#### Context and Action

A **context** is simply a condition during which a player may perform some
action. Some examples include holding a `Class.Tool`, being
`Class.Seat|seated` in a car or standing near a door. Whatever the case may
be, it is up to your `Class.LocalScript|LocalScripts` to call
`Class.ContextActionService:BindAction()|BindAction` when the context is
entered and `Class.ContextActionService:UnbindAction()|UnbindAction` when the
context is left.

An **action** is simply some input that can be performed by the player while
in that context. Such an action could open/close some menu, trigger a
secondary tool action or send a request to the server using
`Class.RemoteFunction:InvokeServer()`. An action is identified by a unique
string as the first parameter of both
`Class.ContextActionService:BindAction()|BindAction` and
`Class.ContextActionService:UnbindAction()|UnbindAction`. The string can be
anything, but it should reflect the **action being performed, not the input
being used**. For example, don't use "KeyH" as an action name - use "CarHorn"
instead. It is best to define your actions as a constant at the top of your
script since you will use it in at least three different places in your code.

#### Binding Actions Contextually

It's better to use ContextActionService's
`Class.ContextActionService:BindAction()|BindAction` than
`Class.UserInputService.InputBegan` for most cases. For
`Class.UserInputService.InputBegan`, your connected function would have to
check if the player is in the context of the action being performed. In most
cases, this is harder than just calling a function when a context is entered/
left. For example, if you want to have the `H` key trigger a car horn sound
while the player is sitting in it, the player might type "hello" in chat or
otherwise use the `H` key for something else. It is harder to determine if
something else is using the H key (like chat) - the car might honk when the
player didn't mean to. If you instead use
`Class.ContextActionService:BindAction()|BindAction` and
`Class.ContextActionService:UnbindAction()|UnbindAction` when the player
enters/leaves the car, `Class.ContextActionService` will make sure that `H`
key presses trigger the honk action only when it is the most recently bound
action. If something else (like chat) takes control, you won't have to worry
about checking that.

#### Inspecting Bound Actions

To see a list of actions and their bound inputs, you can inspect the "Action
Bindings" tab in the Developer Console (F9 while in game). This shows all
bindings, including those bound by Roblox core scripts and default
camera/control scripts too. This is useful for debugging if your actions are
being bound/unbound at the correct times, or if some other action is stealing
input from your actions. For example, if you are attempting to bind
<kbd>W</kbd><kbd>A</kbd><kbd>S</kbd><kbd>D</kbd>, it may be the case that
default character movement scripts are binding over those same keys.
Similarly, the camera control script can steal right-click input if the script
runs after yours.

#### Keyboardless Input

This service is especially useful for supporting gamepad and touch input. For
gamepad input, you might choose to bind the B button to an action that returns
the user to the previous menu when they enter another menu. For touch,
on-screen touch buttons can be used in place of key presses: these buttons
display only while the action is bound, and the position, text and/or images
of these buttons can be configured through this service. They're somewhat
limited in the amount of customization provided by this service; it's usually
a better idea to make your own on-screen buttons using `Class.ImageButton` or
`Class.TextButton`.

## Methods

### `Class.ContextActionService:BindAction`

``BindAction(actionName: `string`, functionToBind: `Datatype.Function`, createTouchButton: `bool`, inputTypes: `Tuple`)`` -> `null`

### `Class.ContextActionService:BindActionAtPriority`

``BindActionAtPriority(actionName: `string`, functionToBind: `Datatype.Function`, createTouchButton: `bool`, priorityLevel: `int`, inputTypes: `Tuple`)`` -> `null`

### `Class.ContextActionService:BindActionToInputTypes`

``BindActionToInputTypes(actionName: `string`, functionToBind: `Datatype.Function`, createTouchButton: `bool`, inputTypes: `Tuple`)`` -> `null`
  [Deprecated]

### `Class.ContextActionService:BindActivate`

``BindActivate(userInputTypeForActivation: `Enum.UserInputType`, keyCodesForActivation: `Tuple`)`` -> `null`

### `Class.ContextActionService:BindCoreAction`

``BindCoreAction(actionName: `string`, functionToBind: `Datatype.Function`, createTouchButton: `bool`, inputTypes: `Tuple`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.ContextActionService:BindCoreActionAtPriority`

``BindCoreActionAtPriority(actionName: `string`, functionToBind: `Datatype.Function`, createTouchButton: `bool`, priorityLevel: `int`, inputTypes: `Tuple`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.ContextActionService:BindCoreActivate`

``BindCoreActivate(userInputTypeForActivation: `Enum.UserInputType`, keyCodesForActivation: `Tuple`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.ContextActionService:CallFunction`

``CallFunction(actionName: `string`, state: `Enum.UserInputState`, inputObject: `Class.Instance`)`` -> `Tuple`
   {security: RobloxScriptSecurity}

### `Class.ContextActionService:FireActionButtonFoundSignal`

``FireActionButtonFoundSignal(actionName: `string`, actionButton: `Class.Instance`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.ContextActionService:GetAllBoundActionInfo`

``GetAllBoundActionInfo()`` -> `Dictionary`

### `Class.ContextActionService:GetAllBoundCoreActionInfo`

``GetAllBoundCoreActionInfo()`` -> `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.ContextActionService:GetBoundActionInfo`

``GetBoundActionInfo(actionName: `string`)`` -> `Dictionary`

### `Class.ContextActionService:GetBoundCoreActionInfo`

``GetBoundCoreActionInfo(actionName: `string`)`` -> `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.ContextActionService:GetButton`

``GetButton(actionName: `string`)`` -> `Class.Instance`
  [Yields]

### `Class.ContextActionService:GetCurrentLocalToolIcon`

``GetCurrentLocalToolIcon()`` -> `string`

### `Class.ContextActionService:GetInputContexts`

``GetInputContexts()`` -> `Datatype.Instances`
   {security: RobloxScriptSecurity}

### `Class.ContextActionService:GetInputSchemaKeyCodeTree`

``GetInputSchemaKeyCodeTree()`` -> `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.ContextActionService:SetDescription`

``SetDescription(actionName: `string`, description: `string`)`` -> `null`

### `Class.ContextActionService:SetImage`

``SetImage(actionName: `string`, image: `string`)`` -> `null`

### `Class.ContextActionService:SetPosition`

``SetPosition(actionName: `string`, position: `Datatype.UDim2`)`` -> `null`

### `Class.ContextActionService:SetTitle`

``SetTitle(actionName: `string`, title: `string`)`` -> `null`

### `Class.ContextActionService:UnbindAction`

``UnbindAction(actionName: `string`)`` -> `null`

### `Class.ContextActionService:UnbindActivate`

``UnbindActivate(userInputTypeForActivation: `Enum.UserInputType`, keyCodeForActivation: `Enum.KeyCode`)`` -> `null`

### `Class.ContextActionService:UnbindAllActions`

``UnbindAllActions()`` -> `null`

### `Class.ContextActionService:UnbindCoreAction`

``UnbindCoreAction(actionName: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.ContextActionService:UnbindCoreActivate`

``UnbindCoreActivate(userInputTypeForActivation: `Enum.UserInputType`, keyCodeForActivation: `Enum.KeyCode`)`` -> `null`
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
