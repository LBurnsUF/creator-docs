---
title: UserGameSettings
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# UserGameSettings

The UserGameSettings is a singleton class found inside of the
`Class.UserSettings` singleton. It holds various persistent settings relating
to how the user wants to control their camera, and their character.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

The UserGameSettings is a singleton class found inside of the
`Class.UserSettings` singleton. It holds various persistent settings relating
to how the user wants to control their camera, and their character.

The properties on this class reflect both the user-facing options exposed in
the in-experience settings menu (such as graphics quality, master volume,
camera and control modes) as well as other contextual user-configurable state
that is not surfaced in the menu itself (such as internal onboarding progress,
VR comfort options, window layout, and debug or profiling configuration). As a
result, some properties listed here may not correspond to anything visible in
the settings UI, and many are restricted to internal Roblox scripts.

You can access this object from a `Class.LocalScript` via:

```lua
UserSettings():GetService("UserGameSettings")
```

This object is intended to be used on the client only, as it serves no purpose
on the server. It will also reflect your own settings when testing in Roblox
Studio.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.UserGameSettings.AllTutorialsDisabled` | `bool` |  {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.BadgeVisible` | `bool` |  {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.CameraMode` | `Enum.CustomCameraMode` |  {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.CameraYInverted` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.ChatTranslationEnabled` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.ChatTranslationFTUXShown` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.ChatTranslationLocale` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.ChatTranslationToggleEnabled` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.ChatVisible` | `bool` |  {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.ComputerCameraMovementMode` | `Enum.ComputerCameraMovementMode` |  |
| `Class.UserGameSettings.ComputerMovementMode` | `Enum.ComputerMovementMode` |  |
| `Class.UserGameSettings.ControlMode` | `Enum.ControlMode` |  |
| `Class.UserGameSettings.DefaultCameraID` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.FramerateCap` | `int` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.Fullscreen` | `bool` |  {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.GamepadCameraSensitivity` | `float` |  |
| `Class.UserGameSettings.GraphicsOptimizationMode` | `Enum.GraphicsOptimizationMode` |  {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.GraphicsQualityLevel` | `int` |  {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.HapticStrength` | `float` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.HasEverUsedVR` | `bool` |  {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.IsUsingCameraYInverted` | `bool` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.IsUsingGamepadCameraSensitivity` | `bool` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.MasterVolume` | `float` |  {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.MasterVolumeStudio` | `float` |  {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.MaxQualityEnabled` | `bool` |  {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.MicroProfilerWebServerEnabled` | `bool` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.MicroProfilerWebServerIP` | `string` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.MicroProfilerWebServerPort` | `int` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.MouseSensitivity` | `float` |  |
| `Class.UserGameSettings.MouseSensitivityFirstPerson` | `Datatype.Vector2` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.MouseSensitivityThirdPerson` | `Datatype.Vector2` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.OnScreenProfilerEnabled` | `bool` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.OnboardingsCompleted` | `string` |  {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.PartyVoiceVolume` | `float` |  {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.PeoplePageLayout` | `Enum.PeoplePageLayout` |  {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.PerformanceStatsVisible` | `bool` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.PlayerHeight` | `float` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.PlayerListVisible` | `bool` |  {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.PlayerNamesEnabled` | `bool` |  {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.PreferredTextSize` | `Enum.PreferredTextSize` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.PreferredTransparency` | `float` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.QualityResetLevel` | `int` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.RCCProfilerRecordFrameRate` | `int` |  |
| `Class.UserGameSettings.RCCProfilerRecordTimeFrame` | `int` |  |
| `Class.UserGameSettings.ReadAloud` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.ReducedMotion` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.RotationType` | `Enum.RotationType` |  |
| `Class.UserGameSettings.SavedQualityLevel` | `Enum.SavedQualitySetting` |  |
| `Class.UserGameSettings.StartMaximized` | `bool` | [NotReplicated] [NotScriptable] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.StartScreenPosition` | `Datatype.Vector2` | [NotReplicated] [NotScriptable] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.StartScreenSize` | `Datatype.Vector2` | [NotReplicated] [NotScriptable] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.StudioPreferredTextSize` | `Enum.PreferredTextSize` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.TouchCameraMovementMode` | `Enum.TouchCameraMovementMode` |  |
| `Class.UserGameSettings.TouchMovementMode` | `Enum.TouchMovementMode` |  |
| `Class.UserGameSettings.UiNavigationKeyBindEnabled` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.UsedCoreGuiIsVisibleToggle` | `bool` |  {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.UsedCustomGuiIsVisibleToggle` | `bool` |  {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.UsedHideHudShortcut` | `bool` |  {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.VRComfortSetting` | `Enum.VRComfortSetting` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.VREnabled` | `bool` |  {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.VRRotationIntensity` | `int` |  {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.VRSafetyBubbleMode` | `Enum.VRSafetyBubbleMode` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.VRSmoothRotationEnabled` | `bool` |  {write: RobloxScriptSecurity} |
| `Class.UserGameSettings.VRSmoothRotationEnabledCustomOption` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.VRThirdPersonFollowCamEnabled` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.VRThirdPersonFollowCamEnabledCustomOption` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.VignetteEnabled` | `bool` |  {write: RobloxScriptSecurity} |
| `Class.UserGameSettings.VignetteEnabledCustomOption` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserGameSettings.VoiceChatVolume` | `float` |  {security: RobloxScriptSecurity} |

## Methods

### `Class.UserGameSettings:GetCameraYInvertValue`

``GetCameraYInvertValue()`` -> `int`

### `Class.UserGameSettings:GetDefaultFramerateCap`

``GetDefaultFramerateCap()`` -> `int`
   {security: RobloxScriptSecurity}

### `Class.UserGameSettings:GetOnboardingCompleted`

``GetOnboardingCompleted(onboardingId: `string`)`` -> `bool`

### `Class.UserGameSettings:GetTutorialState`

``GetTutorialState(tutorialId: `string`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.UserGameSettings:InFullScreen`

``InFullScreen()`` -> `bool`

### `Class.UserGameSettings:InStudioMode`

``InStudioMode()`` -> `bool`

### `Class.UserGameSettings:ResetOnboardingCompleted`

``ResetOnboardingCompleted(onboardingId: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.UserGameSettings:SetCameraYInvertVisible`

``SetCameraYInvertVisible()`` -> `null`

### `Class.UserGameSettings:SetGamepadCameraSensitivityVisible`

``SetGamepadCameraSensitivityVisible()`` -> `null`

### `Class.UserGameSettings:SetOnboardingCompleted`

``SetOnboardingCompleted(onboardingId: `string`)`` -> `null`

### `Class.UserGameSettings:SetTutorialState`

``SetTutorialState(tutorialId: `string`, value: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.UserGameSettings.FullscreenChanged`

Fires with: (isFullscreen: `bool`)

### `Class.UserGameSettings.PerformanceStatsVisibleChanged`

Fires with: (isPerformanceStatsVisible: `bool`)

### `Class.UserGameSettings.StudioModeChanged`

Fires with: (isStudioMode: `bool`)
