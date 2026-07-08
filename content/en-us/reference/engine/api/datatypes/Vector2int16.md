---
title: Vector2int16
type: datatype
---

# `Datatype.Vector2int16`

Represents a Vector2 with signed 16-bit integers for components.

## Description

The `Datatype.Vector2int16` data type represents a vector in 2D space with a
**signed 16-bit integer** for its components. It is similar to
`Datatype.Vector2` in that it allows for the same arithmetic operations, but
it lacks commonly used vector functions.

`Datatype.Vector2int16` should **not** be confused with:

- `Datatype.Vector2`, a **more precise** and complete implementation for 2D
  vectors.
- `Datatype.Vector3int16`, a similar implementation for 3D vectors.

For each component:

- The **lower** bound is -2<sup>15</sup>, or **-32,768**.
- The **upper** bound is 2<sup>15</sup> &minus; 1, or **32,767**.

#### Converting to Vector2

To convert a `Datatype.Vector2int16` to a `Datatype.Vector2`, construct a
`Datatype.Vector2` by passing each **component** of the
`Datatype.Vector2int16` to `Datatype.Vector2.new()`:

```lua
local vector2int16 = Vector2int16.new(1, 2)
local vector2 = Vector2.new(vector2int16.X, vector2int16.Y)
print(vector2)  --> 1, 2
```

Do **not** pass an entire `Datatype.Vector2int16` to `Datatype.Vector2.new()`,
as the constructor interprets a `Datatype.Vector2int16` as a `0` within its
parameters **without producing an error**. This can lead to silent logic
errors if you do something like:

```lua
local vector2int16 = Vector2int16.new(1, 2)
local vector2 = Vector2.new(vector2int16)
print(vector2)  --> 0, 0
```

#### Math Operations

The following math operations are valid for the `Datatype.Vector2int16` data
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
      <td><code>Datatype.Vector2int16</code>&nbsp;<code>+</code>&nbsp;<code>Datatype.Vector2int16</code></td>
      <td>Produces a <code>Datatype.Vector2int16</code> whose components are the sum of the operands' respective components.</td>
    </tr>
    <tr>
      <td><code>Datatype.Vector2int16</code>&nbsp;<code>-</code>&nbsp;<code>Datatype.Vector2int16</code></td>
      <td>Produces a <code>Datatype.Vector2int16</code> whose components are the difference of the operands' respective components.</td>
    </tr>
    <tr>
      <td><code>Datatype.Vector2int16</code>&nbsp;<code>*</code>&nbsp;<code>Datatype.Vector2int16</code></td>
      <td>Produces a <code>Datatype.Vector2int16</code> whose components are the product of the operands' respective components.</td>
    </tr>
    <tr>
      <td><code>Datatype.Vector2int16</code>&nbsp;<code>/</code>&nbsp;<code>Datatype.Vector2int16</code></td>
      <td>Produces a <code>Datatype.Vector2int16</code> whose components are the quotient of the operands' respective components. The results of the
    division are rounded down.</td>
    </tr>
    <tr>
      <td><code>Datatype.Vector2int16</code>&nbsp;<code>*</code>&nbsp;<code>number</code></td>
      <td>Produces a <code>Datatype.Vector2int16</code> whose components are the product of the respective <code>Datatype.Vector2int16</code> components and the number (factor). This operation is commutative.</td>
    </tr>
    <tr>
      <td><code>Datatype.Vector2int16</code>&nbsp;<code>/</code>&nbsp;<code>number</code></td>
      <td>Produces a <code>Datatype.Vector2int16</code> whose components are the quotient of the respective <code>Datatype.Vector2int16</code> components and the number (divisor). The results of the
    division are rounded toward zero.</td>
    </tr>
  </tbody>
</table>

## Constructors

### `Vector2int16.new`

Returns a new `Datatype.Vector2int16` given the x and y components. Non-integer
components are rounded down.

The components must fall within the range [-2<sup>15</sup>,
2<sup>15</sup>).  If outside this range, integer
overflow may occur. For
example, providing 32,768 (equal to 2<sup>15</sup>) as a component
overflows the 16-bit integer, and so the component is -32,768 (equal
to -2<sup>15</sup>) instead.

**Parameters:**

- `x`: `number`
- `y`: `number`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Vector2int16.X` | `number` | The x-coordinate of the `Datatype.Vector2int16`. |
| `Vector2int16.Y` | `number` | The y-coordinate of the `Datatype.Vector2int16`. |

## Math Operations

| Operation | Description |
|-----------|-------------|
| `Vector2int16` + | Produces a `Datatype.Vector2int16` whose components are the sum of the operands' respective componen |
| `Vector2int16` - | Produces a `Datatype.Vector2int16` whose components are the difference of the operands' respective c |
| `Vector2int16` * | Produces a `Datatype.Vector2int16` whose components are the product of the operands' respective comp |
| `Vector2int16` / | Produces a `Datatype.Vector2int16` whose components are the quotient of the operands' respective com |
| `Vector2int16` * | Produces a `Datatype.Vector2int16` whose components are the product of the respective `Datatype.Vect |
| `Vector2int16` / | Produces a `Datatype.Vector2int16` whose components are the quotient of the respective `Datatype.Vec |
