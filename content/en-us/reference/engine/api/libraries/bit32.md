---
title: bit32
type: library
---

# `bit32`

A library of functions to perform bitwise operations.

## Description

This library provides functions to perform bitwise operations.

#### Number Limitations

This library treats numbers as unsigned 32-bit integers; numbers will be
converted to this before being used (see image below). Numbers with decimal
numbers are rounded to the nearest whole number.

<img src="../../../assets/engine-api/libraries/bit32/32-Bit-Restriction.png" width="500" alt="32-bit integer conversion (in hexadecimal)" />

## Functions

### `bit32.arshift`

Returns the number `x` shifted `disp` bits to the right. The number `disp`
may be any representable integer. Negative displacements shift to the
left.

This shift operation is what is called arithmetic shift. Vacant bits on
the left are filled with copies of the higher bit of `x`; vacant bits on
the right are filled with zeros. In particular, displacements with
absolute values higher than 31 result in zero or 0xFFFFFFFF (all original
bits are shifted out).

**Parameters:**

- `x`: `number` - The number whose bits shall be shifted.
- `disp`: `number` - The integer number of bits to shift by.

### `bit32.band`

Returns the bitwise AND of all provided numbers.

Each bit is tested against the following truth table:

<table>
  <thead>
    <tr>
      <th>A</th>
      <th>B</th>
      <th>Output</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>0</td>
      <td>0</td>
      <td>0</td>
    </tr>
    <tr>
      <td>1</td>
      <td>0</td>
      <td>0</td>
    </tr>
    <tr>
      <td>0</td>
      <td>1</td>
      <td>0</td>
    </tr>
    <tr>
      <td>1</td>
      <td>1</td>
      <td>1</td>
    </tr>
  </tbody>
</table>

<img src="../../../assets/engine-api/libraries/bit32/AND.png" width="500" alt="Bitwise AND of 3 numbers" />

**Parameters:**

- `numbers`: `Tuple`

### `bit32.bnot`

Returns the bitwise negation of `x`.

<img src="../../../assets/engine-api/libraries/bit32/NOT.png" width="500" alt="Negation of a provided number" />

For any integer `x`, the following identity holds:

```lua
assert(bit32.bnot(x) == (-1 - x) % 2^32)
```

**Parameters:**

- `x`: `number`

### `bit32.bor`

Returns the bitwise OR of all provided numbers.

Each bit is tested against the following truth table:

<table>
  <thead>
    <tr>
      <th>A</th>
      <th>B</th>
      <th>Output</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>0</td>
      <td>0</td>
      <td>0</td>
    </tr>
    <tr>
      <td>1</td>
      <td>0</td>
      <td>1</td>
    </tr>
    <tr>
      <td>0</td>
      <td>1</td>
      <td>1</td>
    </tr>
    <tr>
      <td>1</td>
      <td>1</td>
      <td>1</td>
    </tr>
  </tbody>
</table>

<img src="../../../assets/engine-api/libraries/bit32/OR.png" width="500" alt="Bitwise OR of 3 numbers" />

**Parameters:**

- `numbers`: `Tuple`

### `bit32.btest`

Returns a boolean signalling whether the bitwise _and_ of its operands is
different from zero.

**Parameters:**

- `numbers`: `Tuple`

### `bit32.bxor`

Returns the bitwise XOR of all provided numbers.

Each bit is tested against the following truth table:

<table>
  <thead>
    <tr>
      <th>A</th>
      <th>B</th>
      <th>Output</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>0</td>
      <td>0</td>
      <td>0</td>
    </tr>
    <tr>
      <td>1</td>
      <td>0</td>
      <td>1</td>
    </tr>
    <tr>
      <td>0</td>
      <td>1</td>
      <td>1</td>
    </tr>
    <tr>
      <td>1</td>
      <td>1</td>
      <td>0</td>
    </tr>
  </tbody>
</table>

<img src="../../../assets/engine-api/libraries/bit32/XOR.png" width="580" alt="Bitwise XOR of 3 numbers" />

**Parameters:**

- `numbers`: `Tuple`

### `bit32.byteswap`

Returns the given number with the order of the bytes swapped.

**Parameters:**

- `x`: `number`

### `bit32.countlz`

Returns the number of consecutive zero bits in the 32-bit representation
of the provided number starting from the left-most (most significant) bit.
Returns 32 if the provided number is zero.

**Parameters:**

- `n`: `number`

### `bit32.countrz`

Returns the number of consecutive zero bits in the 32-bit representation
of the provided number starting from the right-most (least significant)
bit. Returns 32 if the provided number is zero.

**Parameters:**

- `n`: `number`

### `bit32.extract`

Returns the unsigned number formed by the bits `field` to
`field + width - 1` from `n`. Bits are numbered from 0 (least significant)
to 31 (most significant). All accessed bits must be in the range [0, 31].
The default for `width` is 1.

**Parameters:**

- `n`: `number`
- `field`: `number`
- `width`: `number`

### `bit32.replace`

Returns a copy of `n` with the bits `field` to `field + width - 1`
replaced by the value `v`. See `Library.bit32.extract()` for details about
`field` and `width`.

**Parameters:**

- `n`: `number`
- `v`: `number`
- `field`: `number`
- `width`: `number`

### `bit32.lrotate`

Returns the number `x` rotated `disp` bits to the left. The number `disp`
may be any representable integer. For any valid displacement, the
following identity holds:

```lua
assert(bit32.lrotate(x, disp) == bit32.lrotate(x, disp % 32))
```

In particular, negative displacements rotate to the right.

**Parameters:**

- `x`: `number`
- `disp`: `number`

### `bit32.lshift`

Returns the number `x` shifted `disp` bits to the left. The number `disp`
may be any representable integer. Negative displacements shift to the
right. In any direction, vacant bits are filled with zeros. In particular,
displacements with absolute values higher than 31 result in zero (all bits
are shifted out).

<img src="../../../assets/engine-api/libraries/bit32/LSHIFT.png" width="500" alt="Number shifted 3 to the left" />

For positive displacements, the following equality holds:

```lua
assert(bit32.lshift(b, disp) == (b * 2^disp) % 2^32)
```

**Parameters:**

- `x`: `number`
- `disp`: `number`

### `bit32.rrotate`

Returns the number `x` rotated `disp` bits to the right. The number `disp`
may be any representable integer.

For any valid displacement, the following identity holds:

```lua
assert(bit32.rrotate(x, disp) == bit32.rrotate(x , disp % 32))
```

In particular, negative displacements rotate to the left.

**Parameters:**

- `x`: `number`
- `disp`: `number`

### `bit32.rshift`

Returns the number `x` shifted `disp` bits to the right. The number `disp`
may be any representable integer. Negative displacements shift to the
left. In any direction, vacant bits are filled with zeros. In particular,
displacements with absolute values higher than 31 result in zero (all bits
are shifted out).

<img src="../../../assets/engine-api/libraries/bit32/RSHIFT.png" width="500" alt="Number shifted 3 to the right" />

For positive displacements, the following equality holds:

```lua
assert(bit32.rshift(b, disp) == (b % 2^32 / 2^disp) // 1)
```

This shift operation is what is called logical shift.

**Parameters:**

- `x`: `number`
- `disp`: `number`
