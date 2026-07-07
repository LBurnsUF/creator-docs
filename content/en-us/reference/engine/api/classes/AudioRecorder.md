---
title: AudioRecorder
type: class
superclass: Instance
tags: [NotBrowsable]
---

# AudioRecorder

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotBrowsable]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.AudioRecorder.IsRecording` | `bool` |  {write: RobloxSecurity} |
| `Class.AudioRecorder.TimeLength` | `double` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.AudioRecorder:CanRecordAsync`

``CanRecordAsync()`` → `bool`
  [Yields]

### `Class.AudioRecorder:Clear`

``Clear()`` → `null`

### `Class.AudioRecorder:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` → `Datatype.Instances`

### `Class.AudioRecorder:GetInputPins`

``GetInputPins()`` → `Array`

### `Class.AudioRecorder:GetOutputPins`

``GetOutputPins()`` → `Array`

### `Class.AudioRecorder:GetTemporaryContent`

``GetTemporaryContent()`` → `Datatype.Content`

### `Class.AudioRecorder:GetUnrecordableInstancesAsync`

``GetUnrecordableInstancesAsync()`` → `Datatype.Instances`
  [Yields]

### `Class.AudioRecorder:RecordAsync`

``RecordAsync()`` → `null`
  [Yields]

### `Class.AudioRecorder:Stop`

``Stop()`` → `null`

## Events

### `Class.AudioRecorder.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)
