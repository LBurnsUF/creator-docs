---
title: VideoSampler
type: class
superclass: Object
tags: [NotCreatable, NotReplicated]
---

# VideoSampler

An object for sampling frames from video content.

**Inherits from:** `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

This object lets you get image frames from selected timestamps of a video. To
create a `Class.VideoSampler`, call
`Class.VideoService:CreateVideoSamplerAsync()`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.VideoSampler.TimeLength` | `double` | [ReadOnly] [NotReplicated] |
| `Class.VideoSampler.VideoContent` | `Datatype.Content` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.VideoSampler:GetSamplesAtTimesAsync`

``GetSamplesAtTimesAsync(times: `Array`)`` -> `Array`
  [Yields]
