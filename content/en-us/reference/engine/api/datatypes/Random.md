---
title: Random
type: datatype
---

# `Datatype.Random`

Generates pseudorandom numbers and directions.

## Description

The `Datatype.Random` data type generates pseudorandom numbers and directions.

## Constructors

### `Random.new`

Returns a new `Datatype.Random` object. If you don't provide the seed
parameter, `Datatype.Random` uses a seed from an internal entropy source.

If you provide a seed, it should be within the range [-9007199254740991,
9007199254740991], and `Datatype.Random` will round it down to the 
nearest integer. So seeds of 0, 0.99, and `Library.math.random()` all 
produce identical generators. If you need to generate a seed and store it 
for later retrieval, use `Library.math.random()|math.random(max)`.

**Parameters:**

- `seed`: `number`

## Methods

### `Random:NextInteger`

Returns a pseudorandom integer uniformly distributed over `[min, max]`.

**Parameters:**

- `min`: `number`
- `max`: `number`

### `Random:NextNumber`

Returns a uniform pseudorandom real number in the range of 0 to 1,
inclusive.

### `Random:NextNumber`

Returns a uniform pseudorandom real number in the range of `min` to `max`,
inclusive.

**Parameters:**

- `min`: `number`
- `max`: `number`

### `Random:Shuffle`

Uniformly shuffles the array part of `tb` in-place using `NextInteger` to
pick indices. If there are any `nil` "holes" in the array part of the
table, `Shuffle` throws an error, since shuffling could change the length.

The hash part of `tb` is ignored. No metamethods of `tb` are invoked.

The shuffle is defined to be a Fisher-Yates shuffle so the number of
`NextInteger` calls is guaranteed to be consistent between engine versions
for a given size of table.

**Parameters:**

- `tb`: `table`

### `Random:NextUnitVector`

Returns a unit vector with a pseudorandom direction. Vectors returned from
this function are uniformly distributed over the unit sphere.

### `Random:Clone`

Returns a new Random object with the same state as the original.
