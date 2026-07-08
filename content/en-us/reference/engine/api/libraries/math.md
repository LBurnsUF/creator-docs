---
title: math
type: library
---

# `math`

A library of math functions.

## Description

This library is an interface to the standard C math library, providing all of
its functions inside the `Library.math` table.

## Properties

### `math.math.e`

The value of Euler's number, e.

### `math.math.huge`

Returns a value larger than or equal to any other numerical value (about
2<sup>1024</sup>). Dividing a positive number by zero yields this same
value.

### `math.math.nan`

A NaN value, as defined by the IEEE 754 standard. Comparing directly to
`math.nan` will always return false; use `Library.math.isnan()` instead.

### `math.math.phi`

The value of the golden ratio.

### `math.math.pi`

The value of pi.

### `math.math.sqrt2`

The value of the square root of 2.

### `math.math.tau`

The value of tau, which is defined as `2 * math.pi`.

## Functions

### `math.abs`

Returns the absolute value of `x`.

**Parameters:**

- `x`: `number`

### `math.acos`

Returns the arc cosine of `x`.

**Parameters:**

- `x`: `number`

### `math.asin`

Returns the arc sine of `x`.

**Parameters:**

- `x`: `number`

### `math.atan`

Returns the arc tangent of `x` in radians.

**Parameters:**

- `x`: `number`

### `math.atan2`

Returns the arc tangent of `y`/`x` (in radians) while using the signs of
both parameters to find the quadrant of the result. It also handles
correctly the case of `x` being zero.

**Parameters:**

- `y`: `number`
- `x`: `number`

### `math.ceil`

Returns the smallest integer larger than or equal to `x`.

**Parameters:**

- `x`: `number`

### `math.clamp`

Returns a number between `min` and `max`, inclusive.

**Parameters:**

- `x`: `number`
- `min`: `number`
- `max`: `number`

### `math.cos`

Returns the cosine of `x`, assumed to be in radians.

**Parameters:**

- `x`: `number`

### `math.cosh`

Returns the hyperbolic cosine of `x`.

**Parameters:**

- `x`: `number`

### `math.deg`

Returns the angle `x` (given in radians) in degrees.

**Parameters:**

- `x`: `number`

### `math.exp`

Returns the value `e`^`x`.

**Parameters:**

- `x`: `number`

### `math.floor`

Returns the largest integer smaller than or equal to `x`.

**Parameters:**

- `x`: `number`

### `math.fmod`

Returns the remainder of the division of `x` by `y` that rounds the
quotient towards zero.

**Parameters:**

- `x`: `number`
- `y`: `number`

### `math.frexp`

Returns `m` and `e` such that `x` = `m`\*`2`^`e`. `e` is an integer and
the absolute value of `m` is in the range of `0.5` to `1` (inclusive of
`0.5` but exclusive of `1`), or zero when `x` is zero.

**Parameters:**

- `x`: `number`

### `math.isfinite`

Returns true if `x` is a finite number, meaning it is neither NaN nor
positive or negative infinity (±`Library.math.huge`).

**Parameters:**

- `x`: `number`

### `math.isinf`

Returns true if `x` is positive or negative infinity
(±`Library.math.huge`) and false otherwise.

**Parameters:**

- `x`: `number`

### `math.isnan`

Returns true if `x` is not a number (NaN) and false otherwise.

**Parameters:**

- `x`: `number`

### `math.ldexp`

Returns `x`\*`2`^`e` (`e` should be an integer).

**Parameters:**

- `x`: `number`
- `e`: `int`

### `math.lerp`

Returns the linear interpolation between `a` and `b` based on the factor
`t`.

This function uses the formula `a`+`(b-a)`\*`t`. `t` is typically between
`0` and `1` but values outside this range are acceptable.

**Parameters:**

- `a`: `number` - The starting value.
- `b`: `number` - The ending value.
- `t`: `number` - The interpolation factor, typically between `0` and `1`.

**Returns:** The interpolated value between `a` and `b`.

### `math.log`

Returns the logarithm of `x` using the given base, or the mathematical
constant `e` if no base is provided (natural logarithm).

**Parameters:**

- `x`: `number`
- `base`: `number` - The base of the logarithm, the constant `e` by default.

### `math.log10`

Returns the base-10 logarithm of `x`.

**Parameters:**

- `x`: `number`

### `math.map`

Returns a value that represents `x` mapped linearly from the input range
(`inmin` to `inmax`) to the output range (`outmin` to `outmax`). This is
achieved by determining the relative position of `x` within the input
range and applying that ratio to the output range.

**Parameters:**

- `x`: `number` - The number to be mapped.
- `inmin`: `number` - The lower bound of the input range.
- `inmax`: `number` - The upper bound of the input range.
- `outmin`: `number` - The lower bound of the output range.
- `outmax`: `number` - The upper bound of the output range.

**Returns:** The value of `x` mapped to the output range.

### `math.max`

Returns the maximum value among the numbers passed to the function.

**Parameters:**

- `x`: `number`
- `...`: `number`

### `math.min`

Returns the minimum value among the numbers passed to the function.

**Parameters:**

- `x`: `number`
- `...`: `number`

### `math.modf`

Returns two numbers: the integral part of `x` and the fractional part of
`x`.

**Parameters:**

- `x`: `number`

### `math.noise`

Returns a Perlin noise value. The returned value is most often between the
range of `-1` to `1` (inclusive) but sometimes may be outside that range;
if the interval is critical to you, use `Library.math.clamp(noise, -1, 1)`
on the output.

If you leave arguments out, they will be interpreted as zero, so
`Library.math.noise(1.158)` is equivalent to
`Library.math.noise(1.158, 0, 0)` and `Library.math.noise(1.158, 5.723)`
is equivalent to `Library.math.noise(1.158, 5.723, 0)`.

Note that this function uses a Perlin noise algorithm to assign fixed
values to coordinates. For example, `Library.math.noise(1.158, 5.723)`
will always return `0.48397532105446` and `Library.math.noise(1.158, 6)`
will always return `0.15315161645412`.

If `x`, `y`, and `z` are all integers, the return value will be `0`. For
fractional values of `x`, `y`, and `z`, the return value will gradually
fluctuate between `-0.5` and `0.5`. For coordinates that are close to each
other, the return values will also be close to each other.

The noise repeats with a period of `256` on each axis, so
`Library.math.noise(x, y, z)` and `Library.math.noise(x + 256, y, z)`
return identical values.

**Parameters:**

- `x`: `number`
- `y`: `number`
- `z`: `number`

### `math.pow`

Returns `x`^`y` (you can also use the expression `x`^`y` to compute this
value).

**Parameters:**

- `x`: `number`
- `y`: `number`

### `math.rad`

Returns the angle `x` (given in degrees) in radians.

**Parameters:**

- `x`: `number`

### `math.random`

When called without arguments, returns a uniform pseudo-random real number
in the range of `0` to `1` (inclusive of `0` but exclusive of `1`).

When called with an integer number `m`, returns a uniform pseudo-random
integer in the range of `1` to `m`, inclusive.

When called with two integer numbers `m` and `n`, returns a uniform
pseudo-random integer in the range of `m` to `n`, inclusive.

Internally, this uses a 32-bit PCG (Permuted Congruential Generator) which
achieves excellent statistical performance and makes its output hard to
predict.

**Parameters:**

- `m`: `number`
- `n`: `number`

### `math.randomseed`

Sets `x` as the seed for the pseudo-random generator: equal seeds produce
equal sequences of numbers.

**Parameters:**

- `x`: `number`

### `math.round`

Returns the integer with the smallest difference between it and the given
number. For example, the value `5.8` returns `6`.

For values like `0.5` that are equidistant to two integers, the value with
the greater difference between it and zero is chosen. In other words, the
function "rounds away from zero" such that `0.5` rounds to `1` and `-0.5`
rounds to `-1`.

**Parameters:**

- `x`: `number` - The value to be rounded.

### `math.sign`

Returns `-1` if `x` is less than `0`, `0` if `x` equals `0`, or `1` if `x`
is greater than `0`.

**Parameters:**

- `x`: `number`

### `math.sin`

Returns the sine of `x`, assumed to be in radians.

**Parameters:**

- `x`: `number`

### `math.sinh`

Returns the hyperbolic sine of `x`.

**Parameters:**

- `x`: `number`

### `math.sqrt`

Returns the square root of `x`. You can also use the expression `x`^`0.5`
to compute this value.

**Parameters:**

- `x`: `number`

### `math.tan`

Returns the tangent of `x`, assumed to be in radians.

**Parameters:**

- `x`: `number`

### `math.tanh`

Returns the hyperbolic tangent of `x`.

**Parameters:**

- `x`: `number`
