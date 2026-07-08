---
title: RunService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# RunService

Service responsible for all runtime activity and progression of time.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

`RunService` contains methods and events for time management as well as for
managing the context in which an experience or script is running. Methods like
`Class.RunService:IsClient()|IsClient()`,
`Class.RunService:IsServer()|IsServer()`, and
`Class.RunService:IsStudio()|IsStudio()` can help you determine under what
context code is running. These methods are useful for
`Class.ModuleScript|ModuleScripts` that may be required by both client and
server scripts. Furthermore, `Class.RunService:IsStudio()|IsStudio()` can be
used to add special behaviors for in‑Studio testing.

`RunService` also houses events that allow your code to adhere to the engine's
frame‑by‑frame loop, such as `Class.RunService.PreRender|PreRender`,
`Class.RunService.PreAnimation|PreAnimation`,
`Class.RunService.PreSimulation|PreSimulation`,
`Class.RunService.PostSimulation|PostSimulation`, and
`Class.RunService.Heartbeat|Heartbeat`. Selecting the proper event to use for
any case is important, so you should read
[Task Scheduler](../../../performance-optimization/microprofiler/task-scheduler.md)
to make an informed decision.

##### Context Test Results

<table size="small">
  <thead>
    <tr>
      <th>Environment</th>
      <th><code>Class.RunService:IsStudio()|IsStudio</code></th>
      <th><code>Class.RunService:IsClient()|IsClient</code></th>
      <th><code>Class.RunService:IsServer()|IsServer</code></th>
      <th><code>Class.RunService:IsEdit()|IsEdit</code></th>
      <th><code>Class.RunService:IsRunning()|IsRunning</code></th>
      <th><code>Class.RunService:IsRunMode()|IsRunMode</code></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Live (Client)</td>
      <td><code>false</code></td>
      <td><code>true</code></td>
      <td><code>false</code></td>
      <td></td>
      <td><code>true</code></td>
      <td><code>false</code></td>
    </tr>
    <tr>
      <td>Live (Server)</td>
      <td><code>false</code></td>
      <td><code>false</code></td>
      <td><code>true</code></td>
      <td></td>
      <td><code>true</code></td>
      <td><code>false</code></td>
    </tr>
    <tr>
      <td>Edit</td>
      <td><code>true</code></td>
      <td><code>true</code></td>
      <td><code>true</code></td>
      <td><code>true</code></td>
      <td><code>false</code></td>
      <td><code>false</code></td>
    </tr>
    <tr>
      <td>Collaborative Edit</td>
      <td><code>true</code></td>
      <td><code>true</code></td>
      <td><code>false</code></td>
      <td><code>true</code></td>
      <td><code>false</code></td>
      <td><code>false</code></td>
    </tr>
    <tr>
      <td>Run Mode</td>
      <td><code>true</code></td>
      <td><code>false</code></td>
      <td><code>true</code></td>
      <td></td>
      <td><code>true</code></td>
      <td><code>true</code></td>
    </tr>
    <tr>
      <td>Play Mode (Client)</td>
      <td><code>true</code></td>
      <td><code>true</code></td>
      <td><code>false</code></td>
      <td></td>
      <td><code>true</code></td>
      <td><code>false</code></td>
    </tr>
    <tr>
      <td>Play Mode (Server)</td>
      <td><code>true</code></td>
      <td><code>false</code></td>
      <td><code>true</code></td>
      <td></td>
      <td><code>true</code></td>
      <td><code>false</code></td>
    </tr>
    <tr>
      <td>Team Test (Client)</td>
      <td><code>true</code></td>
      <td><code>true</code></td>
      <td><code>false</code></td>
      <td></td>
      <td><code>true</code></td>
      <td><code>false</code></td>
    </tr>
    <tr>
      <td>Team Test (Server)</td>
      <td><code>true</code></td>
      <td><code>false</code></td>
      <td><code>true</code></td>
      <td></td>
      <td><code>true</code></td>
      <td><code>false</code></td>
    </tr>
    <tr>
      <td>Luau Execution</td>
      <td><code>false</code></td>
      <td><code>false</code></td>
      <td><code>true</code></td>
      <td></td>
      <td><code>false</code></td>
      <td><code>false</code></td>
    </tr>
  </tbody>
</table>

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.RunService.ClientGitHash` | `string` | [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.RunService.FrameNumber` | `int64` | [ReadOnly] [NotReplicated] |
| `Class.RunService.RunState` | `Enum.RunState` | [NotReplicated] {security: PluginSecurity} |

## Methods

### `Class.RunService:BindToRenderStep`

``BindToRenderStep(name: `string`, priority: `int`, function: `Datatype.Function`)`` -> `null`

### `Class.RunService:BindToSimulation`

``BindToSimulation(function: `Datatype.Function`, frequency: `Enum.StepFrequency`, priority: `int`)`` -> `Datatype.RBXScriptConnection`

### `Class.RunService:GetControlAndVariantRolloutFlags`

``GetControlAndVariantRolloutFlags()`` -> `Tuple`
   {security: RobloxScriptSecurity}

### `Class.RunService:GetCoreScriptVersion`

``GetCoreScriptVersion()`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.RunService:GetPhysicsStepId`

``GetPhysicsStepId()`` -> `int64`
   {security: RobloxScriptSecurity}

### `Class.RunService:GetPredictionStatus`

``GetPredictionStatus(context: `Class.Instance`)`` -> `Enum.PredictionStatus`

### `Class.RunService:GetRobloxClientChannel`

``GetRobloxClientChannel()`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.RunService:GetRobloxGuiFocused`

``GetRobloxGuiFocused()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.RunService:GetRobloxVersion`

``GetRobloxVersion()`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.RunService:GetTotalScriptPlusExecutionTime`

``GetTotalScriptPlusExecutionTime()`` -> `double`
   {security: RobloxScriptSecurity}

### `Class.RunService:IsClient`

``IsClient()`` -> `bool`

### `Class.RunService:IsEdit`

``IsEdit()`` -> `bool`
   {security: PluginSecurity}

### `Class.RunService:IsResimulating`

``IsResimulating()`` -> `bool`

### `Class.RunService:IsRunMode`

``IsRunMode()`` -> `bool`

### `Class.RunService:IsRunning`

``IsRunning()`` -> `bool`

### `Class.RunService:IsServer`

``IsServer()`` -> `bool`

### `Class.RunService:IsStudio`

``IsStudio()`` -> `bool`

### `Class.RunService:Pause`

``Pause()`` -> `null`
   {security: PluginSecurity}

### `Class.RunService:Reset`

``Reset()`` -> `null`
  [Deprecated] {security: PluginSecurity}

### `Class.RunService:Run`

``Run()`` -> `null`
   {security: PluginSecurity}

### `Class.RunService:Set3dRenderingEnabled`

``Set3dRenderingEnabled(enable: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.RunService:SetPredictionMode`

``SetPredictionMode(context: `Class.Instance`, mode: `Enum.PredictionMode`)`` -> `null`

### `Class.RunService:SetRobloxGuiFocused`

``SetRobloxGuiFocused(focus: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.RunService:Stop`

``Stop()`` -> `null`
   {security: PluginSecurity}

### `Class.RunService:UnbindFromRenderStep`

``UnbindFromRenderStep(name: `string`)`` -> `null`

### `Class.RunService:getThrottleFramerateEnabled`

``getThrottleFramerateEnabled()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.RunService:setThrottleFramerateEnabled`

``setThrottleFramerateEnabled(enable: `bool`)`` -> `null`
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
