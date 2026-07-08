---
title: SensorBase
type: class
superclass: Instance
tags: [NotCreatable]
---

# SensorBase

An abstract class for various sensor instance types.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

A `Class.SensorBase` is an instance that, when parented to a `Class.BasePart`,
outputs additional data about the world around that part. This data is
presented in the sensor's "output" property category. Often, other systems
will consume the sensor's output data.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.SensorBase.UpdateType` | `Enum.SensorUpdateType` |  |

## Methods

### `Class.SensorBase:Sense`

``Sense()`` -> `null`
  [Deprecated]

## Events

### `Class.SensorBase.OnSensorOutputChanged`

Fires with: ()
