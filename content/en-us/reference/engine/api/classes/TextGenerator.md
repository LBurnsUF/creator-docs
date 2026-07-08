---
title: TextGenerator
type: class
superclass: Instance
---

# TextGenerator

Gives access to a large language model for text generation.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

A `TextGenerator` instance lets you use a large language model (LLM) to
generate text based on a system prompt from you and a user prompt from the
player. The most common use of the API is for creating interactive non-player
characters (NPCs).

For example, in a survival experience, your system prompt for a talking animal
might be
`"You are a very busy beaver. You end all statements by mentioning how you need to get back to work on your dam."`.
Users could ask the beaver about water in the area, the size of a nearby
forest, predators, etc.

The novelty of LLM responses can help create unique, delightful moments for
players, but using the API effectively requires a bit of creativity and
tuning. System prompts can be very extensive, so don't hesitate to include a
long string with lots of detail.

#### Rate limits

Requests are initially limited to 100 per minute, which scales up based on the
number of concurrent users.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.TextGenerator.Seed` | `int` |  |
| `Class.TextGenerator.SystemPrompt` | `string` |  |
| `Class.TextGenerator.Temperature` | `float` |  |
| `Class.TextGenerator.TopP` | `float` |  |

## Methods

### `Class.TextGenerator:GenerateTextAsync`

``GenerateTextAsync(request: `Dictionary`)`` -> `Dictionary`
  [Yields]
