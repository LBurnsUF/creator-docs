---
title: Enum
type: datatype
---

# `Datatype.Enum`

A data type that represents an individual enum.

## Description

The `Datatype.Enum` data type represents an individual enum in Roblox. An
individual enum can be indexed through the `Datatype.Enums` type, via the name
of the enum itself.

## Methods

### `Enum:GetEnumItems`

Returns an array of all the `Datatype.EnumItem` options available for this
enum.

### `Enum:FromName`

Returns either the converted `Datatype.Enum` or `nil`.

**Parameters:**

- `name`: `string`

### `Enum:FromValue`

Returns either the converted `Datatype.Enum` or `nil`.

**Parameters:**

- `value`: `number`
