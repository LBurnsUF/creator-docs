---
title: GuiService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# GuiService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Properties

- **AutoSelectGuiEnabled**: `bool`
- **CoreEffectFolder**: `Folder` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **CoreGuiFolder**: `Folder` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **CoreGuiNavigationEnabled**: `bool` [Hidden] [NotReplicated]
- **DisplayScalingMode**: `DisplayScalingMode` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **GuiNavigationEnabled**: `bool`
- **IsModalDialog**: `bool` [ReadOnly] [NotReplicated] [Deprecated]
- **IsWindows**: `bool` [ReadOnly] [NotReplicated] [Deprecated]
- **MenuIsOpen**: `bool` [ReadOnly] [NotReplicated]
- **PreferredTextSize**: `PreferredTextSize` [ReadOnly] [NotReplicated]
- **PreferredTransparency**: `float` [Hidden] [ReadOnly] [NotReplicated]
- **ReducedMotionEnabled**: `bool` [Hidden] [ReadOnly] [NotReplicated]
- **SelectedCoreObject**: `GuiObject` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **SelectedObject**: `GuiObject`
- **TopbarInset**: `Rect` [ReadOnly] [NotReplicated]
- **TouchControlsEnabled**: `bool`
- **ViewportDisplaySize**: `DisplaySize` [ReadOnly] [NotReplicated]
- **ViewportSizeInMM**: `Vector2` [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **AddCenterDialog**(`dialog: Instance`, `centerDialogType: CenterDialogType`, `showFunction: Function`, `hideFunction: Function`) -> `null`
- **AddKey**(`key: string`) -> `null`
- **AddSelectionParent**(`selectionName: string`, `selectionParent: Instance`) -> `null` [Deprecated]
- **AddSelectionTuple**(`selectionName: string`, `selections: Tuple`) -> `null` [Deprecated]
- **AddSpecialKey**(`key: SpecialKey`) -> `null`
- **BroadcastNotification**(`data: string`, `notificationType: int`) -> `null`
- **ClearError**() -> `null`
- **CloseInspectMenu**() -> `null`
- **CloseStatsBasedOnInputString**(`input: string`) -> `bool`
- **DismissNotification**(`notificationId: string`) -> `bool`
- **ForceTenFootInterface**(`isForced: bool`) -> `null`
- **GetBrickCount**() -> `int`
- **GetClosestDialogToPosition**(`position: Vector3`) -> `Instance`
- **GetClosestVisibleDialogToPosition**(`position: Vector3`) -> `Dialog`
- **GetEmotesMenuOpen**() -> `bool`
- **GetErrorCode**() -> `ConnectionError`
- **GetErrorDetails**() -> `Dictionary`
- **GetErrorMessage**() -> `string` [Deprecated]
- **GetErrorType**() -> `ConnectionError`
- **GetGameplayPausedNotificationEnabled**() -> `bool`
- **GetGuiInset**() -> `Tuple`
- **GetGuiIsVisible**(`guiType: GuiType`) -> `bool`
- **GetHardwareSafeViewport**() -> `Vector2`
- **GetInsetArea**(`screenInsets: ScreenInsets`) -> `Rect`
- **GetInspectMenuEnabled**() -> `bool`
- **GetNotificationTypeList**() -> `Dictionary`
- **GetRawScreenScale**() -> `float`
- **GetResolutionScale**() -> `int`
- **GetSafeZoneOffsets**() -> `Dictionary`
- **GetScreenResolution**() -> `Vector2` [Yields]
- **GetUiMessage**() -> `string`
- **InspectPlayerFromHumanoidDescription**(`humanoidDescription: Instance`, `name: string`) -> `null`
- **InspectPlayerFromUserId**(`userId: User`) -> `null`
- **InspectPlayerFromUserIdWithCtx**(`userId: User`, `ctx: string`) -> `null`
- **IsMemoryTrackerEnabled**() -> `bool`
- **IsTenFootInterface**() -> `bool`
- **OnNotificationDisplayed**(`notificationId: string`) -> `null`
- **OnNotificationInteraction**(`notificationId: string`, `buttonIndex: int`) -> `null`
- **OpenBrowserWindow**(`url: string`) -> `null` [Deprecated]
- **OpenNativeOverlay**(`title: string`, `url: string`) -> `null` [Deprecated]
- **RemoveCenterDialog**(`dialog: Instance`) -> `null`
- **RemoveKey**(`key: string`) -> `null`
- **RemoveSelectionGroup**(`selectionName: string`) -> `null` [Deprecated]
- **RemoveSpecialKey**(`key: SpecialKey`) -> `null`
- **Select**(`selectionParent: Instance`) -> `null`
- **SendNotification**(`notificationInfo: Dictionary`) -> `string`
- **SendUIOcclusionMetricsForQueryRegion**(`position: UDim2`, `size: UDim2`, `regionName: string`) -> `null`
- **SetEmotesMenuOpen**(`isOpen: bool`) -> `null`
- **SetGameplayPausedNotificationEnabled**(`enabled: bool`) -> `null`
- **SetGlobalGuiInset**(`x1: int`, `y1: int`, `x2: int`, `y2: int`) -> `null`
- **SetHardwareSafeAreaInsets**(`left: float`, `top: float`, `right: float`, `bottom: float`) -> `null`
- **SetInspectMenuEnabled**(`enabled: bool`) -> `null`
- **SetMenuIsOpen**(`open: bool`, `menuName: string = default`) -> `null`
- **SetPurchasePromptIsShown**(`isShown: bool`) -> `null`
- **SetSafeZoneOffsets**(`top: float`, `bottom: float`, `left: float`, `right: float`) -> `null`
- **SetTopbarInset**(`topbarInset: Rect`) -> `null`
- **SetUiMessage**(`msgType: UiMessageType`, `uiMessage: string = errorCode`) -> `null`
- **ShowStatsBasedOnInputString**(`input: string`) -> `bool`
- **ToggleFullscreen**() -> `null`
- **ToggleGuiIsVisibleForCaptures**(`guiType: GuiType`) -> `null`
- **ToggleGuiIsVisibleIfAllowed**(`guiType: GuiType`) -> `null`

## Events

- **BrowserWindowClosed**() [Deprecated]
- **CloseInspectMenuRequest**()
- **CoreGuiRenderOverflowed**()
- **EmotesMenuOpenChanged**(`isOpen: bool`)
- **ErrorMessageChanged**(`newErrorMessage: string`) [Deprecated]
- **GuiVisibilityChangedSignal**(`guiType: GuiType`, `visible: bool`)
- **InspectMenuEnabledChangedSignal**(`enabled: bool`)
- **InspectPlayerFromHumanoidDescriptionRequest**(`humanoidDescription: Instance`, `name: string`)
- **InspectPlayerFromUserIdWithCtxRequest**(`userId: int64`, `ctx: string`)
- **KeyPressed**(`key: string`, `modifiers: string`)
- **MenuClosed**()
- **MenuOpened**()
- **NativeClose**()
- **NetworkPausedEnabledChanged**(`enabled: bool`)
- **Open9SliceEditor**(`selectedImageObject: Instance`)
- **OpenStyleEditor**(`styleBase: Instance`)
- **PurchasePromptShown**()
- **SafeZoneOffsetsChanged**()
- **ShowLeaveConfirmation**()
- **SpecialKeyPressed**(`key: SpecialKey`, `modifiers: string`)
- **UiMessageChanged**(`msgType: UiMessageType`, `newUiMessage: string`)

## Callbacks

- **SendCoreUiNotification**(`title: string`, `text: string`) -> `null`
