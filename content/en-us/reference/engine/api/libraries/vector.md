---
title: vector
type: library
---

# `vector`

A library of vector functions.

## Description

This library implements functionality for the vector type in addition to the
built-in primitive operator support. It uses vectors with three components
(`x`, `y`, and `z`).

Individual vector components can be accessed using the fields `x` or `X`, `y`
or `Y`, `z` or `Z`. Since vector values are immutable, writing to individual
components is not supported.

## Properties

### `vector.vector.zero`

Constant vector with all components set to `0`.

### `vector.vector.one`

Constant vector with all components set to `1`.

## Functions

### `vector.create`

Creates a new vector with the given component values.

**Parameters:**

- `x`: `number`
- `y`: `number`
- `z`: `number`

### `vector.magnitude`

Calculates the magnitude of a given vector.

**Parameters:**

- `vec`: `vector`

### `vector.normalize`

Computes the normalized version (unit vector) of a given vector.

**Parameters:**

- `vec`: `vector`

### `vector.cross`

Computes the cross product of two vectors.

**Parameters:**

- `vec1`: `vector`
- `vec2`: `vector`

### `vector.dot`

Computes the dot product of two vectors.

**Parameters:**

- `vec1`: `vector`
- `vec2`: `vector`

### `vector.angle`

Computes the angle between two vectors in radians. The axis, if specified,
is used to determine the sign of the angle.

**Parameters:**

- `vec1`: `vector`
- `vec2`: `vector`
- `axis`: `vector?`

### `vector.floor`

Applies `Library.math.floor()` to every component of the input vector.

**Parameters:**

- `vec`: `vector`

### `vector.ceil`

Applies `Library.math.ceil()` to every component of the input vector.

**Parameters:**

- `vec`: `vector`

### `vector.abs`

Applies `Library.math.abs()` to every component of the input vector.

**Parameters:**

- `vec`: `vector`

### `vector.sign`

Applies `Library.math.sign()` to every component of the input vector.

**Parameters:**

- `vec`: `vector`

### `vector.clamp`

Applies `Library.math.clamp()` to every component of the input vector.

**Parameters:**

- `vec`: `vector`
- `min`: `vector`
- `max`: `vector`

### `vector.lerp`

Returns a vector linearly interpolated between two vectors (`vec1`,
`vec2`) by the fraction `alpha`. Note that `alpha` is **not** limited to
the range `[0, 1]`.

**Parameters:**

- `vec1`: `vector`
- `vec2`: `vector`
- `alpha`: `number`

### `vector.max`

Applies `Library.math.max()` to the corresponding components of the input
vectors.

**Parameters:**

- `...`: `vector`

### `vector.min`

Applies `Library.math.min()` to the corresponding components of the input
vectors.

**Parameters:**

- `...`: `vector`
