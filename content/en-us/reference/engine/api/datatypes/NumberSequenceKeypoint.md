---
title: NumberSequenceKeypoint
type: datatype
---

# `Datatype.NumberSequenceKeypoint`

Represents keypoint within a `Datatype.NumberSequence` with a particular time,
value, and envelope size.

## Description

The `Datatype.NumberSequenceKeypoint` data type represents keypoints within a
NumberSequence with a particular time, value, and envelope size.

## Constructors

### `NumberSequenceKeypoint.new`

Returns a keypoint with a specified time and value.

**Parameters:**

- `time`: `number`
- `value`: `number`

### `NumberSequenceKeypoint.new`

Returns a keypoint with a specified time, value, and envelope.

**Parameters:**

- `time`: `number`
- `value`: `number`
- `envelope`: `number`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `NumberSequenceKeypoint.Envelope` | `number` | The amount of variance allowed from the value. |
| `NumberSequenceKeypoint.Time` | `number` | The relative time at which the keypoint is positioned. |
| `NumberSequenceKeypoint.Value` | `number` | The base value of the keypoint. |
