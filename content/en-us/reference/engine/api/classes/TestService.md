---
title: TestService
type: class
superclass: Instance
tags: [Service]
---

# TestService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [Service]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.TestService.AutoRuns` | `bool` |  |
| `Class.TestService.Description` | `string` |  |
| `Class.TestService.ErrorCount` | `int` | [ReadOnly] [NotReplicated] |
| `Class.TestService.ExecuteWithStudioRun` | `bool` |  |
| `Class.TestService.Is30FpsThrottleEnabled` | `bool` | [NotReplicated] [Deprecated] |
| `Class.TestService.IsPhysicsEnvironmentalThrottled` | `bool` |  |
| `Class.TestService.IsSleepAllowed` | `bool` |  |
| `Class.TestService.NumberOfPlayers` | `int` |  |
| `Class.TestService.SimulateSecondsLag` | `double` |  |
| `Class.TestService.TestCount` | `int` | [ReadOnly] [NotReplicated] |
| `Class.TestService.ThrottlePhysicsToRealtime` | `bool` |  |
| `Class.TestService.Timeout` | `double` |  |
| `Class.TestService.WarnCount` | `int` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.TestService:CaptureScreenshotAsync`

``CaptureScreenshotAsync(artifactName: `string`, options: `Dictionary`)`` → `Tuple`
  [Yields]

### `Class.TestService:Check`

``Check(condition: `bool`, description: `string`, source: `Class.Instance`, line: `int`)`` → `null`

### `Class.TestService:Checkpoint`

``Checkpoint(text: `string`, source: `Class.Instance`, line: `int`)`` → `null`

### `Class.TestService:ConvertSlimAcrToObj`

``ConvertSlimAcrToObj(acrFullFilePath: `string`, objFileName: `string`)`` → `string`
   {security: RobloxScriptSecurity}

### `Class.TestService:CreateAndSavePropertySet`

``CreateAndSavePropertySet(source: `Class.Instance`)`` → `string`
   {security: RobloxScriptSecurity}

### `Class.TestService:CreateExtraAssetsFileFromPropertySet`

``CreateExtraAssetsFileFromPropertySet(psetFileName: `string`)`` → `string`
   {security: RobloxScriptSecurity}

### `Class.TestService:Done`

``Done()`` → `null`

### `Class.TestService:Error`

``Error(description: `string`, source: `Class.Instance`, line: `int`)`` → `null`

### `Class.TestService:Fail`

``Fail(description: `string`, source: `Class.Instance`, line: `int`)`` → `null`

### `Class.TestService:FetchExtraAssets`

``FetchExtraAssets(extraAssetsFileName: `string`)`` → `string`
   {security: RobloxScriptSecurity}

### `Class.TestService:GetTestControlSchema`

``GetTestControlSchema(providerName: `string`)`` → `Dictionary`

### `Class.TestService:GetTestControls`

``GetTestControls(providerName: `string`)`` → `Dictionary`

### `Class.TestService:Message`

``Message(text: `string`, source: `Class.Instance`, line: `int`)`` → `null`

### `Class.TestService:RegisterTest`

``RegisterTest(testOptions: `Dictionary`)`` → `Class.TestCase`

### `Class.TestService:RequestValidationAsync`

``RequestValidationAsync(artifactType: `string`, artifactName: `string`)`` → `Tuple`
  [Yields]

### `Class.TestService:Require`

``Require(condition: `bool`, description: `string`, source: `Class.Instance`, line: `int`)`` → `null`

### `Class.TestService:ResetTestControl`

``ResetTestControl(providerName: `string`, controlName: `string`)`` → `null`

### `Class.TestService:Run`

``Run()`` → `null`
  [Yields] [Deprecated] {security: PluginSecurity}

### `Class.TestService:RunAsync`

``RunAsync()`` → `null`
  [Yields] {security: PluginSecurity}

### `Class.TestService:ScopeTime`

``ScopeTime()`` → `Dictionary`

### `Class.TestService:SetTestControl`

``SetTestControl(providerName: `string`, controlName: `string`, value: `Variant`)`` → `null`

### `Class.TestService:StartTestSession`

``StartTestSession()`` → `null`

### `Class.TestService:StartVideoCaptureAsync`

``StartVideoCaptureAsync(artifactName: `string`, options: `Dictionary`)`` → `Tuple`
  [Yields]

### `Class.TestService:StopTestSession`

``StopTestSession()`` → `null`

### `Class.TestService:StopVideoCaptureAsync`

``StopVideoCaptureAsync()`` → `Tuple`
  [Yields]

### `Class.TestService:TakeSnapshot`

``TakeSnapshot(snapshotname: `string`, source: `Class.Instance`)`` → `null`

### `Class.TestService:TranscodePropertySet`

``TranscodePropertySet(extraAssetsFileName: `string`, psetFileName: `string`)`` → `string`
   {security: RobloxScriptSecurity}

### `Class.TestService:Warn`

``Warn(condition: `bool`, description: `string`, source: `Class.Instance`, line: `int`)`` → `null`

### `Class.TestService:getTestSessionProviderStats`

``getTestSessionProviderStats(providerName: `string`)`` → `Dictionary`

### `Class.TestService:isFeatureEnabled`

``isFeatureEnabled(name: `string`)`` → `bool`

## Events

### `Class.TestService.ServerCollectConditionalResult`

Fires with: (condition: `bool`, text: `string`, script: `Class.Instance`, line: `int`)

### `Class.TestService.ServerCollectResult`

Fires with: (text: `string`, script: `Class.Instance`, line: `int`)
