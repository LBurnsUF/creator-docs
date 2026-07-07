---
title: VirtualInputManager
type: class
superclass: Instance
tags: [Service]
---

# VirtualInputManager

**Inherits**: Instance > Object

**Tags**: Service

## Properties

- **AdditionalLuaState**: `string` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **Dump**() -> `null`
- **HandleGamepadAxisInput**(`objectId: int`, `keyCode: KeyCode`, `x: float`, `y: float`, `z: float`) -> `null`
- **HandleGamepadButtonInput**(`deviceId: int`, `keyCode: KeyCode`, `buttonState: int`) -> `null`
- **HandleGamepadConnect**(`deviceId: int`) -> `null`
- **HandleGamepadDisconnect**(`deviceId: int`) -> `null`
- **SendAccelerometerEvent**(`x: float`, `y: float`, `z: float`) -> `null`
- **SendGravityEvent**(`x: float`, `y: float`, `z: float`) -> `null`
- **SendGyroscopeEvent**(`quatX: float`, `quatY: float`, `quatZ: float`, `quatW: float`) -> `null`
- **SendKeyEvent**(`isPressed: bool`, `keyCode: KeyCode`, `isRepeatedKey: bool`, `layerCollector: Instance`) -> `null`
- **SendMouseButtonEvent**(`x: int`, `y: int`, `mouseButton: int`, `isDown: bool`, `layerCollector: Instance`, `repeatCount: int`) -> `null`
- **SendMouseMoveDeltaEvent**(`deltaX: float`, `deltaY: float`, `layerCollector: Instance`) -> `null`
- **SendMouseMoveEvent**(`x: float`, `y: float`, `layerCollector: Instance`) -> `null`
- **SendMouseWheelEvent**(`x: float`, `y: float`, `isForwardScroll: bool`, `layerCollector: Instance`) -> `null`
- **SendScroll**(`x: float`, `y: float`, `deltaX: float`, `deltaY: float`, `options: Dictionary`, `layerCollector: Instance`) -> `null`
- **SendTextInputCharacterEvent**(`str: string`, `layerCollector: Instance`) -> `null`
- **SendTouchEvent**(`touchId: int64`, `state: int`, `x: float`, `y: float`) -> `null`
- **SetInputTypesToIgnore**(`inputTypesToIgnore: Variant`) -> `null`
- **StartPlaying**(`fileName: string`) -> `null`
- **StartPlayingJSON**(`string: string`) -> `null`
- **StartRecording**() -> `null`
- **StopPlaying**() -> `null`
- **StopRecording**() -> `null`
- **WaitForInputEventsProcessed**() -> `null` [Yields]
- **sendRobloxEvent**(`namespace: string`, `detail: string`, `detailType: string`) -> `null`
- **sendThemeChangeEvent**(`themeName: string`) -> `null`

## Events

- **PlaybackCompleted**(`additionalLuaState: string`)
- **RecordingCompleted**(`result: string`)
