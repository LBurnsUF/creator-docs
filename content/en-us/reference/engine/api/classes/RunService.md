---
title: RunService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# RunService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.RunService.ClientGitHash` | `string` | [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.RunService.FrameNumber` | `int64` | [ReadOnly] [NotReplicated] |
| `Class.RunService.RunState` | `Enum.RunState` | [NotReplicated] {security: PluginSecurity} |

## Methods

### `Class.RunService:BindToRenderStep`

``BindToRenderStep(name: `string`, priority: `int`, function: `Datatype.Function`)`` → `null`

### `Class.RunService:BindToSimulation`

``BindToSimulation(function: `Datatype.Function`, frequency: `Enum.StepFrequency`, priority: `int`)`` → `Datatype.RBXScriptConnection`

### `Class.RunService:GetControlAndVariantRolloutFlags`

``GetControlAndVariantRolloutFlags()`` → `Tuple`
   {security: RobloxScriptSecurity}

### `Class.RunService:GetCoreScriptVersion`

``GetCoreScriptVersion()`` → `string`
   {security: RobloxScriptSecurity}

### `Class.RunService:GetPhysicsStepId`

``GetPhysicsStepId()`` → `int64`
   {security: RobloxScriptSecurity}

### `Class.RunService:GetPredictionStatus`

``GetPredictionStatus(context: `Class.Instance`)`` → `Enum.PredictionStatus`

### `Class.RunService:GetRobloxClientChannel`

``GetRobloxClientChannel()`` → `string`
   {security: RobloxScriptSecurity}

### `Class.RunService:GetRobloxGuiFocused`

``GetRobloxGuiFocused()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.RunService:GetRobloxVersion`

``GetRobloxVersion()`` → `string`
   {security: RobloxScriptSecurity}

### `Class.RunService:GetTotalScriptPlusExecutionTime`

``GetTotalScriptPlusExecutionTime()`` → `double`
   {security: RobloxScriptSecurity}

### `Class.RunService:IsClient`

``IsClient()`` → `bool`

### `Class.RunService:IsEdit`

``IsEdit()`` → `bool`
   {security: PluginSecurity}

### `Class.RunService:IsResimulating`

``IsResimulating()`` → `bool`

### `Class.RunService:IsRunMode`

``IsRunMode()`` → `bool`

### `Class.RunService:IsRunning`

``IsRunning()`` → `bool`

### `Class.RunService:IsServer`

``IsServer()`` → `bool`

### `Class.RunService:IsStudio`

``IsStudio()`` → `bool`

### `Class.RunService:Pause`

``Pause()`` → `null`
   {security: PluginSecurity}

### `Class.RunService:Reset`

``Reset()`` → `null`
  [Deprecated] {security: PluginSecurity}

### `Class.RunService:Run`

``Run()`` → `null`
   {security: PluginSecurity}

### `Class.RunService:Set3dRenderingEnabled`

``Set3dRenderingEnabled(enable: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.RunService:SetPredictionMode`

``SetPredictionMode(context: `Class.Instance`, mode: `Enum.PredictionMode`)`` → `null`

### `Class.RunService:SetRobloxGuiFocused`

``SetRobloxGuiFocused(focus: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.RunService:Stop`

``Stop()`` → `null`
   {security: PluginSecurity}

### `Class.RunService:UnbindFromRenderStep`

``UnbindFromRenderStep(name: `string`)`` → `null`

### `Class.RunService:getThrottleFramerateEnabled`

``getThrottleFramerateEnabled()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.RunService:setThrottleFramerateEnabled`

``setThrottleFramerateEnabled(enable: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.RunService.Heartbeat`

Fires with: (deltaTime: `double`)

### `Class.RunService.Misprediction`

Fires with: (time: `double`, instances: `Array`, stats: `Dictionary`)

### `Class.RunService.PostSimulation`

Fires with: (deltaTimeSim: `double`)

### `Class.RunService.PreAnimation`

Fires with: (deltaTimeSim: `double`)

### `Class.RunService.PreRender`

Fires with: (deltaTimeRender: `double`)

### `Class.RunService.PreSimulation`

Fires with: (deltaTimeSim: `double`)

### `Class.RunService.RenderStepped`

Fires with: (deltaTime: `double`)

### `Class.RunService.RobloxGuiFocusedChanged`

Fires with: (isRobloxGuiFocused: `bool`)

### `Class.RunService.Rollback`

Fires with: (time: `double`)

### `Class.RunService.Stepped`

Fires with: (time: `double`, deltaTime: `double`)
