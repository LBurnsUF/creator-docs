---
title: SafetyService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# SafetyService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Properties

- **IsCaptureModeForReport**: `bool` (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **DecodeAvatarMovementProto**(`avatarMovementProtoString: string`) -> `Dictionary`
- **ReportCapturesUIClose**() -> `null`
- **ReportCapturesUIOpen**() -> `null`
- **ReportChatLineReportingClose**() -> `null`
- **ReportChatLineReportingOpen**() -> `null`
- **ReportChatSuspensionDialogClose**() -> `null`
- **ReportChatSuspensionDialogOpen**() -> `null`
- **ReportMenuTabClose**() -> `null`
- **ReportMenuTabOpen**() -> `null`
- **ReportPartyChatWindowClose**() -> `null`
- **ReportPartyChatWindowOpen**() -> `null`
- **TakeScreenshot**(`screenshotOptions: Dictionary`) -> `int64`

## Events

- **ScreenshotContentReady**(`screenshotJobId: int64`, `contentId: ContentId`)
- **ScreenshotUploaded**(`screenshotJobId: int64`, `screenshotId: string`)
