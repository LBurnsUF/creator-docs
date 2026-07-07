---
title: TestService
type: class
superclass: Instance
tags: [Service]
---

# TestService

**Inherits**: Instance > Object

**Tags**: Service

## Properties

- **AutoRuns**: `bool`
- **Description**: `string`
- **ErrorCount**: `int` [ReadOnly] [NotReplicated]
- **ExecuteWithStudioRun**: `bool`
- **Is30FpsThrottleEnabled**: `bool` [NotReplicated] [Deprecated]
- **IsPhysicsEnvironmentalThrottled**: `bool`
- **IsSleepAllowed**: `bool`
- **NumberOfPlayers**: `int`
- **SimulateSecondsLag**: `double`
- **TestCount**: `int` [ReadOnly] [NotReplicated]
- **ThrottlePhysicsToRealtime**: `bool`
- **Timeout**: `double`
- **WarnCount**: `int` [ReadOnly] [NotReplicated]

## Methods

- **CaptureScreenshotAsync**(`artifactName: string = `, `options: Dictionary = nil`) -> `Tuple` [Yields]
- **Check**(`condition: bool`, `description: string`, `source: Instance = nil`, `line: int = 0`) -> `null`
- **Checkpoint**(`text: string`, `source: Instance = nil`, `line: int = 0`) -> `null`
- **ConvertSlimAcrToObj**(`acrFullFilePath: string`, `objFileName: string`) -> `string`
- **CreateAndSavePropertySet**(`source: Instance`) -> `string`
- **CreateExtraAssetsFileFromPropertySet**(`psetFileName: string`) -> `string`
- **Done**() -> `null`
- **Error**(`description: string`, `source: Instance = nil`, `line: int = 0`) -> `null`
- **Fail**(`description: string`, `source: Instance = nil`, `line: int = 0`) -> `null`
- **FetchExtraAssets**(`extraAssetsFileName: string`) -> `string`
- **GetTestControlSchema**(`providerName: string`) -> `Dictionary`
- **GetTestControls**(`providerName: string`) -> `Dictionary`
- **Message**(`text: string`, `source: Instance = nil`, `line: int = 0`) -> `null`
- **RegisterTest**(`testOptions: Dictionary`) -> `TestCase`
- **RequestValidationAsync**(`artifactType: string`, `artifactName: string`) -> `Tuple` [Yields]
- **Require**(`condition: bool`, `description: string`, `source: Instance = nil`, `line: int = 0`) -> `null`
- **ResetTestControl**(`providerName: string`, `controlName: string`) -> `null`
- **Run**() -> `null` [Yields] [Deprecated]
- **RunAsync**() -> `null` [Yields]
- **ScopeTime**() -> `Dictionary`
- **SetTestControl**(`providerName: string`, `controlName: string`, `value: Variant`) -> `null`
- **StartTestSession**() -> `null`
- **StartVideoCaptureAsync**(`artifactName: string = `, `options: Dictionary = nil`) -> `Tuple` [Yields]
- **StopTestSession**() -> `null`
- **StopVideoCaptureAsync**() -> `Tuple` [Yields]
- **TakeSnapshot**(`snapshotname: string`, `source: Instance = nil`) -> `null`
- **TranscodePropertySet**(`extraAssetsFileName: string`, `psetFileName: string`) -> `string`
- **Warn**(`condition: bool`, `description: string`, `source: Instance = nil`, `line: int = 0`) -> `null`
- **getTestSessionProviderStats**(`providerName: string`) -> `Dictionary`
- **isFeatureEnabled**(`name: string`) -> `bool`

## Events

- **ServerCollectConditionalResult**(`condition: bool`, `text: string`, `script: Instance`, `line: int`)
- **ServerCollectResult**(`text: string`, `script: Instance`, `line: int`)
