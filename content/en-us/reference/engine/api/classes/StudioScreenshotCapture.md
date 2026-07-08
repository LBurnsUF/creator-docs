---
title: StudioScreenshotCapture
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# StudioScreenshotCapture

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.StudioScreenshotCapture.BufferFormat` | `Enum.StudioCaptureScreenshotFormat` | [ReadOnly] [NotReplicated] {security: PluginSecurity} |
| `Class.StudioScreenshotCapture.BufferStatus` | `Enum.StudioCaptureBufferStatus` | [ReadOnly] [NotReplicated] {security: PluginSecurity} |
| `Class.StudioScreenshotCapture.OriginalSize` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] {security: PluginSecurity} |
| `Class.StudioScreenshotCapture.Position` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] {security: PluginSecurity} |
| `Class.StudioScreenshotCapture.Resolution` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] {security: PluginSecurity} |
| `Class.StudioScreenshotCapture.UICaptureMode` | `Enum.UICaptureMode` | [ReadOnly] [NotReplicated] {security: PluginSecurity} |

## Methods

### `Class.StudioScreenshotCapture:GetBuffer`

``GetBuffer()`` -> `Datatype.buffer`
   {security: PluginSecurity}

### `Class.StudioScreenshotCapture:GetErrors`

``GetErrors()`` -> `Array`
   {security: PluginSecurity}

### `Class.StudioScreenshotCapture:ScaleAsync`

``ScaleAsync(strategy: `Enum.ResamplerMode`, newSize: `Datatype.Vector2`)`` -> `Class.StudioScreenshotCapture`
  [Yields] {security: PluginSecurity}
