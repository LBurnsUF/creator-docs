---
title: TestService
type: class
superclass: Instance
tags: [Service]
---

# TestService

A service used by Roblox to run controlled tests of the engine. It is
available for developers to use, to a limited degree.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [Service]

## Description

`TestService` is a service used by Roblox internally to run analytical tests
on the engine.

Scripts that are executed inside of `TestService` (via
`Class.TestService:RunAsync()`) have access to special macros that directly
invoke functions under the service. Macros are essentially substitutions for
large blocks of code that shouldn't need to be rewritten each time you want to
call them.

#### RBX_CHECK

This macro does tests with calls to the `Class.TestService:Check()` function.

<table size="small">
  <thead>
	<tr>
		<th>Macro</th>
		<th>Test Condition</th>
	</tr>
  </thead>
  <tbody>
	<tr>
		<td><code>RBX_CHECK(cond)</code></td>
		<td><code>cond == true</code></td>
	</tr>
	<tr>
		<td><code>RBX_CHECK_MESSAGE(cond, failMsg)</code></td>
		<td><code>cond == true</code></td>
	</tr>
	<tr>
		<td><code>RBX_CHECK_THROW(CODE)</code></td>
		<td><code>pcall(function() CODE end) == false</code></td>
	</tr>
	<tr>
		<td><code>RBX_CHECK_NO_THROW(CODE)</code></td>
		<td><code>pcall(function() CODE end) == true</code></td>
	</tr>
	<tr>
		<td><code>RBX_CHECK_EQUAL(a, b)</code></td>
		<td><code>a == b</code></td>
	</tr>
	<tr>
		<td><code>RBX_CHECK_NE(a, b)</code></td>
		<td><code>a ~= b</code></td>
	</tr>
	<tr>
		<td><code>RBX_CHECK_GE(a, b)</code></td>
		<td><code>a &gt;= b</code></td>
	</tr>
	<tr>
		<td><code>RBX_CHECK_LE(a, b)</code></td>
		<td><code>a &lt;= b</code></td>
	</tr>
	<tr>
		<td><code>RBX_CHECK_GT(a, b)</code></td>
		<td><code>a &gt; b</code></td>
	</tr>
	<tr>
		<td><code>RBX_CHECK_LT(a, b)</code></td>
		<td><code>a &lt; b</code></td>
	</tr>
  </tbody>
</table>

#### RBX_REQUIRE

This macro does tests with calls to the `Class.TestService:Require()`
function.

<table size="small">
  <thead>
	<tr>
		<th>Macro</th>
		<th>Test Condition</th>
	</tr>
  </thead>
  <tbody>
	<tr>
		<td><code>RBX_REQUIRE(cond)</code></td>
		<td><code>cond == true</code></td>
	</tr>
	<tr>
		<td><code>RBX_REQUIRE_MESSAGE(cond, failMsg)</code></td>
		<td><code>cond == true</code></td>
	</tr>
	<tr>
		<td><code>RBX_REQUIRE_THROW(CODE)</code></td>
		<td><code>pcall(function() CODE end) == false</code></td>
	</tr>
	<tr>
		<td><code>RBX_REQUIRE_NO_THROW(CODE)</code></td>
		<td><code>pcall(function() CODE end) == true</code></td>
	</tr>
	<tr>
		<td><code>RBX_REQUIRE_EQUAL(a, b)</code></td>
		<td><code>a == b</code></td>
	</tr>
	<tr>
		<td><code>RBX_REQUIRE_NE(a, b)</code></td>
		<td><code>a ~= b</code></td>
	</tr>
	<tr>
		<td><code>RBX_REQUIRE_GE(a, b)</code></td>
		<td><code>a &gt;= b</code></td>
	</tr>
	<tr>
		<td><code>RBX_REQUIRE_LE(a, b)</code></td>
		<td><code>a &lt;= b</code></td>
	</tr>
	<tr>
		<td><code>RBX_REQUIRE_GT(a, b)</code></td>
		<td><code>a &gt; b</code></td>
	</tr>
	<tr>
		<td><code>RBX_REQUIRE_LT(a, b)</code></td>
		<td><code>a &lt; b</code></td>
	</tr>
  </tbody>
</table>

#### RBX_WARN

This macro does tests with calls to the `Class.TestService:Warn()` function.

<table size="small">
  <thead>
	<tr>
		<th>Macro</th>
		<th>Test Condition</th>
	</tr>
  </thead>
  <tbody>
	<tr>
		<td><code>RBX_WARN(cond)</code></td>
		<td><code>cond == true</code></td>
	</tr>
	<tr>
		<td><code>RBX_WARN_MESSAGE(cond, failMsg)</code></td>
		<td><code>cond == true</code></td>
	</tr>
	<tr>
		<td><code>RBX_WARN_THROW(CODE)</code></td>
		<td><code>pcall(function() CODE end) == false</code></td>
	</tr>
	<tr>
		<td><code>RBX_WARN_NO_THROW(CODE)</code></td>
		<td><code>pcall(function() CODE end) == true</code></td>
	</tr>
	<tr>
		<td><code>RBX_WARN_EQUAL(a, b)</code></td>
		<td><code>a == b</code></td>
	</tr>
	<tr>
		<td><code>RBX_WARN_NE(a, b)</code></td>
		<td><code>a ~= b</code></td>
	</tr>
	<tr>
		<td><code>RBX_WARN_GE(a, b)</code></td>
		<td><code>a &gt;= b</code></td>
	</tr>
	<tr>
		<td><code>RBX_WARN_LE(a, b)</code></td>
		<td><code>a &lt;= b</code></td>
	</tr>
	<tr>
		<td><code>RBX_WARN_GT(a, b)</code></td>
		<td><code>a &gt; b</code></td>
	</tr>
	<tr>
		<td><code>RBX_WARN_LT(a, b)</code></td>
		<td><code>a &lt; b</code></td>
	</tr>
  </tbody>
</table>

#### Additional Macros

<table size="small">
<thead>
<tr>
<th>Macro</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>RBX_ERROR(msg)</code></td>
<td>Directly calls the <code>Class.TestService:Error()</code> function.</td>
</tr>
<tr>
<td><code>RBX_FAIL(msg)</code></td>
<td>Directly calls the <code>Class.TestService:Fail()</code> function.</td>
</tr>
<tr>
<td><code>RBX_MESSAGE(msg)</code></td>
<td>Directly calls the <code>Class.TestService:Message()</code> function.</td>
</tr>
</tbody>
</table>

## Properties

| Property | Type | Description |
|----------|------|-------------|
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

``CaptureScreenshotAsync(artifactName: `string`, options: `Dictionary`)`` -> `Tuple`
  [Yields]

### `Class.TestService:Check`

``Check(condition: `bool`, description: `string`, source: `Class.Instance`, line: `int`)`` -> `null`

### `Class.TestService:Checkpoint`

``Checkpoint(text: `string`, source: `Class.Instance`, line: `int`)`` -> `null`

### `Class.TestService:ConvertSlimAcrToObj`

``ConvertSlimAcrToObj(acrFullFilePath: `string`, objFileName: `string`)`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.TestService:CreateAndSavePropertySet`

``CreateAndSavePropertySet(source: `Class.Instance`)`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.TestService:CreateExtraAssetsFileFromPropertySet`

``CreateExtraAssetsFileFromPropertySet(psetFileName: `string`)`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.TestService:Done`

``Done()`` -> `null`

### `Class.TestService:Error`

``Error(description: `string`, source: `Class.Instance`, line: `int`)`` -> `null`

### `Class.TestService:Fail`

``Fail(description: `string`, source: `Class.Instance`, line: `int`)`` -> `null`

### `Class.TestService:FetchExtraAssets`

``FetchExtraAssets(extraAssetsFileName: `string`)`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.TestService:GetTestControlSchema`

``GetTestControlSchema(providerName: `string`)`` -> `Dictionary`

### `Class.TestService:GetTestControls`

``GetTestControls(providerName: `string`)`` -> `Dictionary`

### `Class.TestService:Message`

``Message(text: `string`, source: `Class.Instance`, line: `int`)`` -> `null`

### `Class.TestService:RegisterTest`

``RegisterTest(testOptions: `Dictionary`)`` -> `Class.TestCase`

### `Class.TestService:RequestValidationAsync`

``RequestValidationAsync(artifactType: `string`, artifactName: `string`)`` -> `Tuple`
  [Yields]

### `Class.TestService:Require`

``Require(condition: `bool`, description: `string`, source: `Class.Instance`, line: `int`)`` -> `null`

### `Class.TestService:ResetTestControl`

``ResetTestControl(providerName: `string`, controlName: `string`)`` -> `null`

### `Class.TestService:Run`

``Run()`` -> `null`
  [Yields] [Deprecated] {security: PluginSecurity}

### `Class.TestService:RunAsync`

``RunAsync()`` -> `null`
  [Yields] {security: PluginSecurity}

### `Class.TestService:ScopeTime`

``ScopeTime()`` -> `Dictionary`

### `Class.TestService:SetTestControl`

``SetTestControl(providerName: `string`, controlName: `string`, value: `Variant`)`` -> `null`

### `Class.TestService:StartTestSession`

``StartTestSession()`` -> `null`

### `Class.TestService:StartVideoCaptureAsync`

``StartVideoCaptureAsync(artifactName: `string`, options: `Dictionary`)`` -> `Tuple`
  [Yields]

### `Class.TestService:StopTestSession`

``StopTestSession()`` -> `null`

### `Class.TestService:StopVideoCaptureAsync`

``StopVideoCaptureAsync()`` -> `Tuple`
  [Yields]

### `Class.TestService:TakeSnapshot`

``TakeSnapshot(snapshotname: `string`, source: `Class.Instance`)`` -> `null`

### `Class.TestService:TranscodePropertySet`

``TranscodePropertySet(extraAssetsFileName: `string`, psetFileName: `string`)`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.TestService:Warn`

``Warn(condition: `bool`, description: `string`, source: `Class.Instance`, line: `int`)`` -> `null`

### `Class.TestService:getTestSessionProviderStats`

``getTestSessionProviderStats(providerName: `string`)`` -> `Dictionary`

### `Class.TestService:isFeatureEnabled`

``isFeatureEnabled(name: `string`)`` -> `bool`

## Events

### `Class.TestService.ServerCollectConditionalResult`

Fires with: (condition: `bool`, text: `string`, script: `Class.Instance`, line: `int`)

### `Class.TestService.ServerCollectResult`

Fires with: (text: `string`, script: `Class.Instance`, line: `int`)
