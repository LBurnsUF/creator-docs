---
title: RunService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# RunService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Properties

- **ClientGitHash**: `string` [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **FrameNumber**: `int64` [ReadOnly] [NotReplicated]
- **RunState**: `RunState` [NotReplicated] (Security: Read=PluginSecurity, Write=PluginSecurity)

## Methods

- **BindToRenderStep**(`name: string`, `priority: int`, `function: Function`) -> `null`
- **BindToSimulation**(`function: Function`, `frequency: StepFrequency = Hz30`, `priority: int = 2000`) -> `RBXScriptConnection`
- **GetControlAndVariantRolloutFlags**() -> `Tuple`
- **GetCoreScriptVersion**() -> `string`
- **GetPhysicsStepId**() -> `int64`
- **GetPredictionStatus**(`context: Instance`) -> `PredictionStatus`
- **GetRobloxClientChannel**() -> `string`
- **GetRobloxGuiFocused**() -> `bool`
- **GetRobloxVersion**() -> `string`
- **GetTotalScriptPlusExecutionTime**() -> `double`
- **IsClient**() -> `bool`
- **IsEdit**() -> `bool`
- **IsResimulating**() -> `bool`
- **IsRunMode**() -> `bool`
- **IsRunning**() -> `bool`
- **IsServer**() -> `bool`
- **IsStudio**() -> `bool`
- **Pause**() -> `null`
- **Reset**() -> `null` [Deprecated]
- **Run**() -> `null`
- **Set3dRenderingEnabled**(`enable: bool`) -> `null`
- **SetPredictionMode**(`context: Instance`, `mode: PredictionMode`) -> `null`
- **SetRobloxGuiFocused**(`focus: bool`) -> `null`
- **Stop**() -> `null`
- **UnbindFromRenderStep**(`name: string`) -> `null`
- **getThrottleFramerateEnabled**() -> `bool`
- **setThrottleFramerateEnabled**(`enable: bool`) -> `null`

## Events

- **Heartbeat**(`deltaTime: double`)
- **Misprediction**(`time: double`, `instances: Array`, `stats: Dictionary`)
- **PostSimulation**(`deltaTimeSim: double`)
- **PreAnimation**(`deltaTimeSim: double`)
- **PreRender**(`deltaTimeRender: double`)
- **PreSimulation**(`deltaTimeSim: double`)
- **RenderStepped**(`deltaTime: double`)
- **RobloxGuiFocusedChanged**(`isRobloxGuiFocused: bool`)
- **Rollback**(`time: double`)
- **Stepped**(`time: double`, `deltaTime: double`)
