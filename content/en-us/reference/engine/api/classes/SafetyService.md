---
title: SafetyService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# SafetyService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.SafetyService.IsCaptureModeForReport` | `bool` |  {security: RobloxScriptSecurity} |

## Methods

### `Class.SafetyService:DecodeAvatarMovementProto`

``DecodeAvatarMovementProto(avatarMovementProtoString: `string`)`` → `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.SafetyService:ReportCapturesUIClose`

``ReportCapturesUIClose()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SafetyService:ReportCapturesUIOpen`

``ReportCapturesUIOpen()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SafetyService:ReportChatLineReportingClose`

``ReportChatLineReportingClose()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SafetyService:ReportChatLineReportingOpen`

``ReportChatLineReportingOpen()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SafetyService:ReportChatSuspensionDialogClose`

``ReportChatSuspensionDialogClose()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SafetyService:ReportChatSuspensionDialogOpen`

``ReportChatSuspensionDialogOpen()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SafetyService:ReportMenuTabClose`

``ReportMenuTabClose()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SafetyService:ReportMenuTabOpen`

``ReportMenuTabOpen()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SafetyService:ReportPartyChatWindowClose`

``ReportPartyChatWindowClose()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SafetyService:ReportPartyChatWindowOpen`

``ReportPartyChatWindowOpen()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SafetyService:TakeScreenshot`

``TakeScreenshot(screenshotOptions: `Dictionary`)`` → `int64`
   {security: RobloxScriptSecurity}

## Events

### `Class.SafetyService.ScreenshotContentReady`

Fires with: (screenshotJobId: `int64`, contentId: `Datatype.ContentId`)

### `Class.SafetyService.ScreenshotUploaded`

Fires with: (screenshotJobId: `int64`, screenshotId: `string`)
