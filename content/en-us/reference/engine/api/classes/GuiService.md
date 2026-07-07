---
title: GuiService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# GuiService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.GuiService.AutoSelectGuiEnabled` | `bool` |  |
| `Class.GuiService.CoreEffectFolder` | `Class.Folder` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.GuiService.CoreGuiFolder` | `Class.Folder` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.GuiService.CoreGuiNavigationEnabled` | `bool` | [Hidden] [NotReplicated] |
| `Class.GuiService.DisplayScalingMode` | `Enum.DisplayScalingMode` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.GuiService.GuiNavigationEnabled` | `bool` |  |
| `Class.GuiService.IsModalDialog` | `bool` | [ReadOnly] [NotReplicated] [Deprecated] |
| `Class.GuiService.IsWindows` | `bool` | [ReadOnly] [NotReplicated] [Deprecated] |
| `Class.GuiService.MenuIsOpen` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.GuiService.PreferredTextSize` | `Enum.PreferredTextSize` | [ReadOnly] [NotReplicated] |
| `Class.GuiService.PreferredTransparency` | `float` | [Hidden] [ReadOnly] [NotReplicated] |
| `Class.GuiService.ReducedMotionEnabled` | `bool` | [Hidden] [ReadOnly] [NotReplicated] |
| `Class.GuiService.SelectedCoreObject` | `Class.GuiObject` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.GuiService.SelectedObject` | `Class.GuiObject` |  |
| `Class.GuiService.TopbarInset` | `Datatype.Rect` | [ReadOnly] [NotReplicated] |
| `Class.GuiService.TouchControlsEnabled` | `bool` |  |
| `Class.GuiService.ViewportDisplaySize` | `Enum.DisplaySize` | [ReadOnly] [NotReplicated] |
| `Class.GuiService.ViewportSizeInMM` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |

## Methods

### `Class.GuiService:AddCenterDialog`

``AddCenterDialog(dialog: `Class.Instance`, centerDialogType: `Enum.CenterDialogType`, showFunction: `Datatype.Function`, hideFunction: `Datatype.Function`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.GuiService:AddKey`

``AddKey(key: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.GuiService:AddSelectionParent`

``AddSelectionParent(selectionName: `string`, selectionParent: `Class.Instance`)`` → `null`
  [Deprecated]

### `Class.GuiService:AddSelectionTuple`

``AddSelectionTuple(selectionName: `string`, selections: `Tuple`)`` → `null`
  [Deprecated]

### `Class.GuiService:AddSpecialKey`

``AddSpecialKey(key: `Enum.SpecialKey`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.GuiService:BroadcastNotification`

``BroadcastNotification(data: `string`, notificationType: `int`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.GuiService:ClearError`

``ClearError()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.GuiService:CloseInspectMenu`

``CloseInspectMenu()`` → `null`

### `Class.GuiService:CloseStatsBasedOnInputString`

``CloseStatsBasedOnInputString(input: `string`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.GuiService:DismissNotification`

``DismissNotification(notificationId: `string`)`` → `bool`

### `Class.GuiService:ForceTenFootInterface`

``ForceTenFootInterface(isForced: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.GuiService:GetBrickCount`

``GetBrickCount()`` → `int`
   {security: RobloxScriptSecurity}

### `Class.GuiService:GetClosestDialogToPosition`

``GetClosestDialogToPosition(position: `Datatype.Vector3`)`` → `Class.Instance`
   {security: RobloxScriptSecurity}

### `Class.GuiService:GetClosestVisibleDialogToPosition`

``GetClosestVisibleDialogToPosition(position: `Datatype.Vector3`)`` → `Class.Dialog`
   {security: RobloxScriptSecurity}

### `Class.GuiService:GetEmotesMenuOpen`

``GetEmotesMenuOpen()`` → `bool`

### `Class.GuiService:GetErrorCode`

``GetErrorCode()`` → `Enum.ConnectionError`
   {security: RobloxScriptSecurity}

### `Class.GuiService:GetErrorDetails`

``GetErrorDetails()`` → `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.GuiService:GetErrorMessage`

``GetErrorMessage()`` → `string`
  [Deprecated] {security: RobloxScriptSecurity}

### `Class.GuiService:GetErrorType`

``GetErrorType()`` → `Enum.ConnectionError`
   {security: RobloxScriptSecurity}

### `Class.GuiService:GetGameplayPausedNotificationEnabled`

``GetGameplayPausedNotificationEnabled()`` → `bool`

### `Class.GuiService:GetGuiInset`

``GetGuiInset()`` → `Tuple`

### `Class.GuiService:GetGuiIsVisible`

``GetGuiIsVisible(guiType: `Enum.GuiType`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.GuiService:GetHardwareSafeViewport`

``GetHardwareSafeViewport()`` → `Datatype.Vector2`
   {security: RobloxScriptSecurity}

### `Class.GuiService:GetInsetArea`

``GetInsetArea(screenInsets: `Enum.ScreenInsets`)`` → `Datatype.Rect`

### `Class.GuiService:GetInspectMenuEnabled`

``GetInspectMenuEnabled()`` → `bool`

### `Class.GuiService:GetNotificationTypeList`

``GetNotificationTypeList()`` → `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.GuiService:GetRawScreenScale`

``GetRawScreenScale()`` → `float`
   {security: RobloxScriptSecurity}

### `Class.GuiService:GetResolutionScale`

``GetResolutionScale()`` → `int`
   {security: RobloxScriptSecurity}

### `Class.GuiService:GetSafeZoneOffsets`

``GetSafeZoneOffsets()`` → `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.GuiService:GetScreenResolution`

``GetScreenResolution()`` → `Datatype.Vector2`
  [Yields] {security: RobloxScriptSecurity}

### `Class.GuiService:GetUiMessage`

``GetUiMessage()`` → `string`
   {security: RobloxScriptSecurity}

### `Class.GuiService:InspectPlayerFromHumanoidDescription`

``InspectPlayerFromHumanoidDescription(humanoidDescription: `Class.Instance`, name: `string`)`` → `null`

### `Class.GuiService:InspectPlayerFromUserId`

``InspectPlayerFromUserId(userId: `Datatype.User`)`` → `null`

### `Class.GuiService:InspectPlayerFromUserIdWithCtx`

``InspectPlayerFromUserIdWithCtx(userId: `Datatype.User`, ctx: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.GuiService:IsMemoryTrackerEnabled`

``IsMemoryTrackerEnabled()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.GuiService:IsTenFootInterface`

``IsTenFootInterface()`` → `bool`

### `Class.GuiService:OnNotificationDisplayed`

``OnNotificationDisplayed(notificationId: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.GuiService:OnNotificationInteraction`

``OnNotificationInteraction(notificationId: `string`, buttonIndex: `int`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.GuiService:OpenBrowserWindow`

``OpenBrowserWindow(url: `string`)`` → `null`
  [Deprecated] {security: RobloxScriptSecurity}

### `Class.GuiService:OpenNativeOverlay`

``OpenNativeOverlay(title: `string`, url: `string`)`` → `null`
  [Deprecated] {security: RobloxScriptSecurity}

### `Class.GuiService:RemoveCenterDialog`

``RemoveCenterDialog(dialog: `Class.Instance`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.GuiService:RemoveKey`

``RemoveKey(key: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.GuiService:RemoveSelectionGroup`

``RemoveSelectionGroup(selectionName: `string`)`` → `null`
  [Deprecated]

### `Class.GuiService:RemoveSpecialKey`

``RemoveSpecialKey(key: `Enum.SpecialKey`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.GuiService:Select`

``Select(selectionParent: `Class.Instance`)`` → `null`

### `Class.GuiService:SendNotification`

``SendNotification(notificationInfo: `Dictionary`)`` → `string`

### `Class.GuiService:SendUIOcclusionMetricsForQueryRegion`

``SendUIOcclusionMetricsForQueryRegion(position: `Datatype.UDim2`, size: `Datatype.UDim2`, regionName: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.GuiService:SetEmotesMenuOpen`

``SetEmotesMenuOpen(isOpen: `bool`)`` → `null`

### `Class.GuiService:SetGameplayPausedNotificationEnabled`

``SetGameplayPausedNotificationEnabled(enabled: `bool`)`` → `null`

### `Class.GuiService:SetGlobalGuiInset`

``SetGlobalGuiInset(x1: `int`, y1: `int`, x2: `int`, y2: `int`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.GuiService:SetHardwareSafeAreaInsets`

``SetHardwareSafeAreaInsets(left: `float`, top: `float`, right: `float`, bottom: `float`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.GuiService:SetInspectMenuEnabled`

``SetInspectMenuEnabled(enabled: `bool`)`` → `null`

### `Class.GuiService:SetMenuIsOpen`

``SetMenuIsOpen(open: `bool`, menuName: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.GuiService:SetPurchasePromptIsShown`

``SetPurchasePromptIsShown(isShown: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.GuiService:SetSafeZoneOffsets`

``SetSafeZoneOffsets(top: `float`, bottom: `float`, left: `float`, right: `float`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.GuiService:SetTopbarInset`

``SetTopbarInset(topbarInset: `Datatype.Rect`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.GuiService:SetUiMessage`

``SetUiMessage(msgType: `Enum.UiMessageType`, uiMessage: `string`)`` → `null`
   {security: LocalUserSecurity}

### `Class.GuiService:ShowStatsBasedOnInputString`

``ShowStatsBasedOnInputString(input: `string`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.GuiService:ToggleFullscreen`

``ToggleFullscreen()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.GuiService:ToggleGuiIsVisibleForCaptures`

``ToggleGuiIsVisibleForCaptures(guiType: `Enum.GuiType`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.GuiService:ToggleGuiIsVisibleIfAllowed`

``ToggleGuiIsVisibleIfAllowed(guiType: `Enum.GuiType`)`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.GuiService.BrowserWindowClosed`

Fires with: ()
  [Deprecated]

### `Class.GuiService.CloseInspectMenuRequest`

Fires with: ()

### `Class.GuiService.CoreGuiRenderOverflowed`

Fires with: ()

### `Class.GuiService.EmotesMenuOpenChanged`

Fires with: (isOpen: `bool`)

### `Class.GuiService.ErrorMessageChanged`

Fires with: (newErrorMessage: `string`)
  [Deprecated]

### `Class.GuiService.GuiVisibilityChangedSignal`

Fires with: (guiType: `Enum.GuiType`, visible: `bool`)

### `Class.GuiService.InspectMenuEnabledChangedSignal`

Fires with: (enabled: `bool`)

### `Class.GuiService.InspectPlayerFromHumanoidDescriptionRequest`

Fires with: (humanoidDescription: `Class.Instance`, name: `string`)

### `Class.GuiService.InspectPlayerFromUserIdWithCtxRequest`

Fires with: (userId: `int64`, ctx: `string`)

### `Class.GuiService.KeyPressed`

Fires with: (key: `string`, modifiers: `string`)

### `Class.GuiService.MenuClosed`

Fires with: ()

### `Class.GuiService.MenuOpened`

Fires with: ()

### `Class.GuiService.NativeClose`

Fires with: ()

### `Class.GuiService.NetworkPausedEnabledChanged`

Fires with: (enabled: `bool`)

### `Class.GuiService.Open9SliceEditor`

Fires with: (selectedImageObject: `Class.Instance`)

### `Class.GuiService.OpenStyleEditor`

Fires with: (styleBase: `Class.Instance`)

### `Class.GuiService.PurchasePromptShown`

Fires with: ()

### `Class.GuiService.SafeZoneOffsetsChanged`

Fires with: ()

### `Class.GuiService.ShowLeaveConfirmation`

Fires with: ()

### `Class.GuiService.SpecialKeyPressed`

Fires with: (key: `Enum.SpecialKey`, modifiers: `string`)

### `Class.GuiService.UiMessageChanged`

Fires with: (msgType: `Enum.UiMessageType`, newUiMessage: `string`)

## Callbacks

### `Class.GuiService.SendCoreUiNotification`

``SendCoreUiNotification(title: `string`, text: `string`)`` → `null`
