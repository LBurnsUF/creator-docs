---
title: Faces
type: datatype
---

# `Datatype.Faces`

A data type containing six booleans, each representing a face of a
`Class.BasePart`.

## Description

The `Datatype.Faces` data type contains six booleans representing whether a
feature is enabled for each face (`Enum.NormalId`) of a Part. In other words,
this contains a boolean for each axes (X/Y/Z) in both directions
(positive/negative). The `Class.Handles` object uses this data type to enable
whether a direction has a visible handle on a Part's face.

```lua
local handles = Instance.new("Handles")
handles.Faces = Faces.new(Enum.NormalId.Front, Enum.NormalId.Left)
```

Like most data types on Roblox, the Faces data type is immutable: you cannot
assign to its properties once created.

## Constructors

### `Faces.new`

Creates a new Faces given some number of `Enum.NormalId` as arguments. Each NormalId provided indicates the property of the same name in the new Faces will be true.

- The `Library.table.unpack()` function can be used to unpack a table of NormalId to be included.
- Passing values that are not a `Enum.NormalId` will do nothing; they are ignored silently.

**Parameters:**

- `normalIds...`: `Tuple`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Faces.Top` | `bool` | Whether the top face is included. |
| `Faces.Bottom` | `bool` | Whether the bottom face is included. |
| `Faces.Left` | `bool` | Whether the left face is included. |
| `Faces.Right` | `bool` | Whether the right face is included. |
| `Faces.Back` | `bool` | Whether the back face is included. |
| `Faces.Front` | `bool` | Whether the front face is included. |

## API Usage (2 locations)

### Used as Property Type

- `Class.BasePart.ResizeableFaces`
- `Class.Handles.Faces`
