---
title: Pages
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# Pages

An abstract class for pages objects.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

An object which is essentially a table of pages, each of which is a sorted
list of the key/value pairs.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Pages.IsFinished` | `bool` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.Pages:AdvanceToNextPageAsync`

``AdvanceToNextPageAsync()`` -> `null`
  [Yields]

### `Class.Pages:GetCurrentPage`

``GetCurrentPage()`` -> `Array`
