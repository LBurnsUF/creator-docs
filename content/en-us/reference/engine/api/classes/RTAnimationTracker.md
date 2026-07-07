---
title: RTAnimationTracker
type: class
superclass: Instance
tags: [NotReplicated]
---

# RTAnimationTracker

**Inherits**: Instance > Object

**Tags**: NotReplicated

## Properties

- **Active**: `bool` [Hidden] [NotReplicated]
- **EnableFallbackAudioInput**: `bool` [Hidden] [NotReplicated]
- **SessionName**: `string` [Hidden] [NotReplicated]
- **TrackerMode**: `TrackerMode` [Hidden] [ReadOnly] [NotReplicated]
- **TrackerType**: `TrackerType` [Hidden] [NotReplicated]

## Methods

- **Step**() -> `null`

## Events

- **TrackerError**(`errorCode: TrackerError`, `msg: string`)
- **TrackerPrompt**(`prompt: TrackerPromptEvent`)
