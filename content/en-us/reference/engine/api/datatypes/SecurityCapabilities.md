---
title: SecurityCapabilities
type: datatype
---

# `Datatype.SecurityCapabilities`

A set of `Enum.SecurityCapability` items. See
[script capabilities](../../../scripting/capabilities.md).

## Constructors

### `SecurityCapabilities.new`

Returns a new set of capabilities from zero or more `Enum.SecurityCapability`
items.

```lua
local capabilities = SecurityCapabilities.new(Enum.SecurityCapability.Players,
	Enum.SecurityCapability.Animation,
	Enum.SecurityCapability.Basic)

local newScript = Instance.new("Script")
newScript.Capabilities = capabilities
```

**Parameters:**

- `...`: `SecurityCapability`

### `SecurityCapabilities.fromCurrent`

Returns a new set of capabilities from the capabilities of the calling function.

## Methods

### `SecurityCapabilities:Add`

Returns a new set of capabilities with zero or more additions. If you add
`Enum.SecurityCapability` items that are already present, they are not
duplicated.

**Parameters:**

- `...`: `SecurityCapability`

### `SecurityCapabilities:Add`

Returns a new set of capabilities with the provided set added. If you add
`Enum.SecurityCapability` items that are already present, they are not
duplicated.

**Parameters:**

- `capabilities`: `SecurityCapabilities`

### `SecurityCapabilities:Remove`

Returns a new set of capabilities with zero or more deletions.
`Enum.SecurityCapability` items not present in the original set are
ignored.

**Parameters:**

- `...`: `SecurityCapability`

### `SecurityCapabilities:Remove`

Returns a new set of capabilities with the provided set deleted.
`Enum.SecurityCapability` items not present in the original set are
ignored.

**Parameters:**

- `capabilities`: `SecurityCapabilities`

### `SecurityCapabilities:Contains`

Returns whether a set of capabilities contains the specified
`Enum.SecurityCapability` items. The set must contain **all** provided
items to return true.

**Parameters:**

- `...`: `SecurityCapability`

### `SecurityCapabilities:Contains`

Returns whether a set of capabilities contains another set of
capabilities. The set must contain **all** items in the provided set to
return true.

**Parameters:**

- `capabilities`: `SecurityCapabilities`

## API Usage (1 locations)

### Used as Property Type

- `Class.Instance.Capabilities`
