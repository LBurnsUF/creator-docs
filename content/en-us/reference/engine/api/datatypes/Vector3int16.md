---
title: Vector3int16
type: datatype
---

# `Datatype.Vector3int16`

A Vector3 with signed 16-bit integers for components.

## Description

The `Datatype.Vector3int16` data type represents a vector in 3D space with a
**signed 16-bit integer** for its components. It is similar to
`Datatype.Vector3` in that it allows for the same arithmetic operations, but
it lacks commonly used vector functions.

`Datatype.Vector3int16` should **not** be confused with:

- `Datatype.Vector3`, a **more precise** and complete implementation for 3D
  vectors.
- `Datatype.Vector2int16`, a similar implementation for 2D vectors.

For each component:

- The **lower** bound is -2<sup>15</sup>, or **-32,768**.
- The **upper** bound is 2<sup>15</sup> &minus; 1, or **32,767**.

#### Converting to Vector3

To convert a `Datatype.Vector3int16` to a `Datatype.Vector3`, construct a
`Datatype.Vector3` by passing each **component** of the
`Datatype.Vector3int16` to `Datatype.Vector3.new()`:

```lua
local vector3int16 = Vector3int16.new(1, 2, 3)
local vector3 = Vector3.new(vector3int16.X, vector3int16.Y, vector3int16.Z)
print(vector3)  --> 1, 2, 3
```

Do **not** pass an entire `Datatype.Vector3int16` to `Datatype.Vector3.new()`,
as the constructor interprets a `Datatype.Vector3int16` as a `0` within its
parameters **without producing an error**. This can lead to silent logic
errors if you do something like:

```lua
local vector3int16 = Vector3int16.new(1, 2, 3)
local vector3 = Vector3.new(vector3int16)
print(vector3)  --> 0, 0, 0
```

#### Math Operations

The following math operations are valid for the `Datatype.Vector3int16` data
type. For all operations, be mindful of the bounds associated with signed
16-bit integers, described earlier.

<table>
  <thead>
    <tr>
      <td>Operation</td>
      <td>Description</td>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>Datatype.Vector3int16</code>&nbsp;<code>+</code>&nbsp;<code>Datatype.Vector3int16</code></td>
      <td>Produces a <code>Datatype.Vector3int16</code> whose components are the sum of the operands' respective components.</td>
    </tr>
    <tr>
      <td><code>Datatype.Vector3int16</code>&nbsp;<code>-</code>&nbsp;<code>Datatype.Vector3int16</code></td>
      <td>Produces a <code>Datatype.Vector3int16</code> whose components are the difference of the operands' respective components.</td>
    </tr>
    <tr>
      <td><code>Datatype.Vector3int16</code>&nbsp;<code>*</code>&nbsp;<code>Datatype.Vector3int16</code></td>
      <td>Produces a <code>Datatype.Vector3int16</code> whose components are the product of the operands' respective components.</td>
    </tr>
    <tr>
      <td><code>Datatype.Vector3int16</code>&nbsp;<code>/</code>&nbsp;<code>Datatype.Vector3int16</code></td>
      <td>Produces a <code>Datatype.Vector3int16</code> whose components are the quotient of the operands' respective components. The results of the
    division are rounded down.</td>
    </tr>
    <tr>
      <td><code>Datatype.Vector3int16</code>&nbsp;<code>*</code>&nbsp;<code>number</code></td>
      <td>Produces a <code>Datatype.Vector3int16</code> whose components are the product of the respective <code>Datatype.Vector3int16</code> components and the number (factor). This operation is commutative.</td>
    </tr>
    <tr>
      <td><code>Datatype.Vector3int16</code>&nbsp;<code>/</code>&nbsp;<code>number</code></td>
      <td>Produces a <code>Datatype.Vector3int16</code> whose components are the quotient of the respective <code>Datatype.Vector3int16</code> components and the number (divisor). The results of the
    division are rounded toward zero.</td>
    </tr>
  </tbody>
</table>

## Constructors

### `Vector3int16.new`

Returns a new `Datatype.Vector3int16` from the given x, y and z components.
Non-integer components are rounded down.

The components must fall within the range [-2<sup>15</sup>,
2<sup>15</sup>).  If outside this range, integer
overflow may occur. For
example, providing 32,768 (equal to 2<sup>15</sup>) as a component
overflows the 16-bit integer, and so the component will be -32,768 (equal
to -2<sup>15</sup>) instead.

**Parameters:**

- `x`: `number`
- `y`: `number`
- `z`: `number`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Vector3int16.X` | `number` | The x-coordinate of the `Datatype.Vector3int16`. |
| `Vector3int16.Y` | `number` | The y-coordinate of the `Datatype.Vector3int16`. |
| `Vector3int16.Z` | `number` | The z-coordinate of the `Datatype.Vector3int16`. |

## Math Operations

| Operation | Description |
|-----------|-------------|
| `Vector3int16` + | Produces a `Datatype.Vector3int16` whose components are the sum of the operands' respective componen |
| `Vector3int16` - | Produces a `Datatype.Vector3int16` whose components are the difference of the operands' respective c |
| `Vector3int16` * | Produces a `Datatype.Vector3int16` whose components are the product of the operands' respective comp |
| `Vector3int16` / | Produces a `Datatype.Vector3int16` whose components are the quotient of the operands' respective com |
| `Vector3int16` * | Produces a `Datatype.Vector3int16` whose components are the product of the respective `Datatype.Vect |
| `Vector3int16` / | Produces a `Datatype.Vector3int16` whose components are the quotient of the respective `Datatype.Vec |

## API Usage (1 locations)

### Used as Parameter Type

- `Class.Terrain:PasteRegion` (parameter `corner`)
