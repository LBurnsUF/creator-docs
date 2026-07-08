---
title: AudioRecorder
type: class
superclass: Instance
tags: [NotBrowsable]
---

# AudioRecorder

Records audio streams in-experience.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotBrowsable]

## Description

**This API is in development and is not available yet.**

`AudioRecorder` records audio streams in-experience with a fixed time limit of
60 seconds. The results can be loaded into an `Class.AudioPlayer` for
playback.

At this time, `Class.AudioDeviceInput` cannot be recorded. The
`Class.AudioRecorder:GetUnrecordableInstancesAsync()|GetUnrecordableInstancesAsync()`
method can be used to check specifically which instances aren't recordable.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AudioRecorder.IsRecording` | `bool` |  {write: RobloxSecurity} |
| `Class.AudioRecorder.TimeLength` | `double` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.AudioRecorder:CanRecordAsync`

``CanRecordAsync()`` -> `bool`
  [Yields]

### `Class.AudioRecorder:Clear`

``Clear()`` -> `null`

### `Class.AudioRecorder:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` -> `Datatype.Instances`

### `Class.AudioRecorder:GetInputPins`

``GetInputPins()`` -> `Array`

### `Class.AudioRecorder:GetOutputPins`

``GetOutputPins()`` -> `Array`

### `Class.AudioRecorder:GetTemporaryContent`

``GetTemporaryContent()`` -> `Datatype.Content`

### `Class.AudioRecorder:GetUnrecordableInstancesAsync`

``GetUnrecordableInstancesAsync()`` -> `Datatype.Instances`
  [Yields]

### `Class.AudioRecorder:RecordAsync`

``RecordAsync()`` -> `null`
  [Yields]

### `Class.AudioRecorder:Stop`

``Stop()`` -> `null`

## Events

### `Class.AudioRecorder.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)
