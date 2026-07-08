---
title: MemoryStoreHashMapPages
type: class
superclass: Pages
tags: [NotCreatable, NotReplicated]
---

# MemoryStoreHashMapPages

A special type of `Class.Pages` object whose pages contain key-value pairs
from a `Class.MemoryStoreHashMap`.

**Inherits from:** `Class.Pages` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

A special type of `Class.Pages` object whose pages contain key-value pairs
from a `Class.MemoryStoreHashMap`. `Class.Pages:GetCurrentPage()` can be used
to retrieve an array of tables, each containing a key and value; these reflect
the key-value pair data.
