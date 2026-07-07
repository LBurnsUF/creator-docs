---
title: StudioScreenshotCapture
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# StudioScreenshotCapture

**Inherits**: Instance > Object

**Tags**: NotCreatable, NotReplicated

## Properties

- **BufferFormat**: `StudioCaptureScreenshotFormat` [ReadOnly] [NotReplicated] (Security: Read=PluginSecurity, Write=PluginSecurity)
- **BufferStatus**: `StudioCaptureBufferStatus` [ReadOnly] [NotReplicated] (Security: Read=PluginSecurity, Write=PluginSecurity)
- **OriginalSize**: `Vector2` [ReadOnly] [NotReplicated] (Security: Read=PluginSecurity, Write=PluginSecurity)
- **Position**: `Vector2` [ReadOnly] [NotReplicated] (Security: Read=PluginSecurity, Write=PluginSecurity)
- **Resolution**: `Vector2` [ReadOnly] [NotReplicated] (Security: Read=PluginSecurity, Write=PluginSecurity)
- **UICaptureMode**: `UICaptureMode` [ReadOnly] [NotReplicated] (Security: Read=PluginSecurity, Write=PluginSecurity)

## Methods

- **GetBuffer**() -> `buffer`
- **GetErrors**() -> `Array`
- **ScaleAsync**(`strategy: ResamplerMode`, `newSize: Vector2`) -> `StudioScreenshotCapture` [Yields]
