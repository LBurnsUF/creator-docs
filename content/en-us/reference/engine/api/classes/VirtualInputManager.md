---
title: VirtualInputManager
type: class
superclass: Instance
tags: [Service]
---

# VirtualInputManager

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [Service]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.VirtualInputManager.AdditionalLuaState` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |

## Methods

### `Class.VirtualInputManager:Dump`

``Dump()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.VirtualInputManager:HandleGamepadAxisInput`

``HandleGamepadAxisInput(objectId: `int`, keyCode: `Enum.KeyCode`, x: `float`, y: `float`, z: `float`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.VirtualInputManager:HandleGamepadButtonInput`

``HandleGamepadButtonInput(deviceId: `int`, keyCode: `Enum.KeyCode`, buttonState: `int`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.VirtualInputManager:HandleGamepadConnect`

``HandleGamepadConnect(deviceId: `int`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.VirtualInputManager:HandleGamepadDisconnect`

``HandleGamepadDisconnect(deviceId: `int`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.VirtualInputManager:SendAccelerometerEvent`

``SendAccelerometerEvent(x: `float`, y: `float`, z: `float`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.VirtualInputManager:SendGravityEvent`

``SendGravityEvent(x: `float`, y: `float`, z: `float`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.VirtualInputManager:SendGyroscopeEvent`

``SendGyroscopeEvent(quatX: `float`, quatY: `float`, quatZ: `float`, quatW: `float`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.VirtualInputManager:SendKeyEvent`

``SendKeyEvent(isPressed: `bool`, keyCode: `Enum.KeyCode`, isRepeatedKey: `bool`, layerCollector: `Class.Instance`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.VirtualInputManager:SendMouseButtonEvent`

``SendMouseButtonEvent(x: `int`, y: `int`, mouseButton: `int`, isDown: `bool`, layerCollector: `Class.Instance`, repeatCount: `int`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.VirtualInputManager:SendMouseMoveDeltaEvent`

``SendMouseMoveDeltaEvent(deltaX: `float`, deltaY: `float`, layerCollector: `Class.Instance`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.VirtualInputManager:SendMouseMoveEvent`

``SendMouseMoveEvent(x: `float`, y: `float`, layerCollector: `Class.Instance`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.VirtualInputManager:SendMouseWheelEvent`

``SendMouseWheelEvent(x: `float`, y: `float`, isForwardScroll: `bool`, layerCollector: `Class.Instance`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.VirtualInputManager:SendScroll`

``SendScroll(x: `float`, y: `float`, deltaX: `float`, deltaY: `float`, options: `Dictionary`, layerCollector: `Class.Instance`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.VirtualInputManager:SendTextInputCharacterEvent`

``SendTextInputCharacterEvent(str: `string`, layerCollector: `Class.Instance`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.VirtualInputManager:SendTouchEvent`

``SendTouchEvent(touchId: `int64`, state: `int`, x: `float`, y: `float`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.VirtualInputManager:SetInputTypesToIgnore`

``SetInputTypesToIgnore(inputTypesToIgnore: `Variant`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.VirtualInputManager:StartPlaying`

``StartPlaying(fileName: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.VirtualInputManager:StartPlayingJSON`

``StartPlayingJSON(string: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.VirtualInputManager:StartRecording`

``StartRecording()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.VirtualInputManager:StopPlaying`

``StopPlaying()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.VirtualInputManager:StopRecording`

``StopRecording()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.VirtualInputManager:WaitForInputEventsProcessed`

``WaitForInputEventsProcessed()`` → `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.VirtualInputManager:sendRobloxEvent`

``sendRobloxEvent(namespace: `string`, detail: `string`, detailType: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.VirtualInputManager:sendThemeChangeEvent`

``sendThemeChangeEvent(themeName: `string`)`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.VirtualInputManager.PlaybackCompleted`

Fires with: (additionalLuaState: `string`)

### `Class.VirtualInputManager.RecordingCompleted`

Fires with: (result: `string`)
