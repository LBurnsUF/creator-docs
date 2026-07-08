---
title: DataStorePages
type: class
superclass: Pages
tags: [NotCreatable, NotReplicated]
---

# DataStorePages

A `Class.Pages` object that allows iteration through `Class.OrderedDataStore`
key/value pairs.

**Inherits from:** `Class.Pages` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

A special type of `Class.Pages` object whose pages contain key/value pairs
from an `Class.OrderedDataStore`. For this object,
`Class.Pages:GetCurrentPage()|GetCurrentPage()` returns an array of tables,
each containing keys named **key** and **value**; these reflect the key/value
pair data.
