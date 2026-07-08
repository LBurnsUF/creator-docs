---
title: File
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# File

An asset loaded from a file on disk.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

An object that represents an asset loaded from a file on a local disk. Files
generate a temporary asset ID in the form `rbxtemp://` which can be used in
Studio without uploading the asset, but will be destroyed when the
`Class.File` is destroyed or when the Studio session ends. Temporary asset IDs
are not shared across [collaborative](../../../projects/collaboration.md)
sessions.

The default `Class.Instance.Name|Name` of a `Class.File` instance will be the
filename on disk, excluding the path but including the extension.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.File.Size` | `int64` | [Hidden] [ReadOnly] [NotReplicated] {security: PluginSecurity} |

## Methods

### `Class.File:GetBinaryContents`

``GetBinaryContents()`` -> `string`
   {security: PluginSecurity}

### `Class.File:GetTemporaryId`

``GetTemporaryId()`` -> `Datatype.ContentId`
   {security: PluginSecurity}
