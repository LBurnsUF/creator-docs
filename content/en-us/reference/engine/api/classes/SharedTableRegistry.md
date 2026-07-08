---
title: SharedTableRegistry
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# SharedTableRegistry

Provides a global registry of named `Datatype.SharedTable` objects.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

Provides a global registry of named `Datatype.SharedTable` objects. It can be
used to store `Datatype.SharedTable` objects that are used by multiple
scripts.

## Methods

### `Class.SharedTableRegistry:GetSharedTable`

``GetSharedTable(name: `string`)`` -> `Datatype.SharedTable`

### `Class.SharedTableRegistry:SetSharedTable`

``SetSharedTable(name: `string`, st: `Datatype.SharedTable`?)`` -> `null`
