---
title: ScreenshotCaptureResult
type: enum
---

# `Enum.ScreenshotCaptureResult`

Describes the result of a screenshot capture initiated by
`Class.CaptureService:TakeScreenshotCaptureAsync()`.

The ScreenshotCaptureResult enum describes the result of a screenshot capture
initiated through `Class.CaptureService:TakeScreenshotCaptureAsync()`. It is
passed as the first argument to the `onCaptureReady` callback.

The `Enum.ScreenshotCaptureResult` enum has 4 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.ScreenshotCaptureResult.Success` | 0 | The screenshot capture completed successfully. |
| `Enum.ScreenshotCaptureResult.OtherError` | 1 | The screenshot capture failed due to an unspecified error. |
| `Enum.ScreenshotCaptureResult.NoDeviceSupport` | 2 | The device does not support screenshot captures. |
| `Enum.ScreenshotCaptureResult.NoSpaceOnDevice` | 3 | The device does not have enough storage space to save the screenshot capture. |
