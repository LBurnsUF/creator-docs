---
title: AudioRecorder
type: class
superclass: Instance
tags: [NotBrowsable]
---

# AudioRecorder

**Inherits**: Instance > Object

**Tags**: NotBrowsable

## Properties

- **IsRecording**: `bool` (Security: Read=None, Write=RobloxSecurity)
- **TimeLength**: `double` [ReadOnly] [NotReplicated]

## Methods

- **CanRecordAsync**() -> `bool` [Yields]
- **Clear**() -> `null`
- **GetConnectedWires**(`pin: string`) -> `Instances`
- **GetInputPins**() -> `Array`
- **GetOutputPins**() -> `Array`
- **GetTemporaryContent**() -> `Content`
- **GetUnrecordableInstancesAsync**() -> `Instances` [Yields]
- **RecordAsync**() -> `null` [Yields]
- **Stop**() -> `null`

## Events

- **WiringChanged**(`connected: bool`, `pin: string`, `wire: Wire`, `instance: Instance`)
