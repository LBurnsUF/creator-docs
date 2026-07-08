---
title: buffer
type: library
---

# `buffer`

A library of buffer functions.

## Description

A buffer is an object that represents a fixed-size mutable block of memory.
The buffer library provides functions for creation and manipulation of buffer
objects, providing all its functions inside the global `Library.buffer`
variable.

Buffer is intended to be used a low-level binary data storage structure,
replacing the uses of `Library.string.pack()` and `Library.string.unpack()`.
Use cases include reading and writing existing binary formats, working with
data in a more compact form, serialization to custom binary formats, and
general work with native memory types like fixed-length integers and floats.

When passed through Roblox APIs, including sending a buffer through custom
events, the identity of the buffer object is not preserved and the target will
receive a copy. Similar to other limitations, the same buffer object cannot be
used from multiple `Class.Actor` scripts (Parallel Luau).

Many of the functions accept an offset in bytes from the start of the buffer.
Offset of `0` from the start of the buffer memory block accesses the first
byte. All offsets, counts and sizes should be non-negative integer numbers. If
the bytes that are accessed by any read or write operation are outside the
buffer memory, an error is thrown.

The `read` and `write` methods that work with integers and floats use
[little-endian](https://en.wikipedia.org/wiki/Endianness) encoding.

## Functions

### `buffer.create`

Creates a buffer of the requested size with all bytes initialized to `0`.
Size limit is 1 GiB, or 1,073,741,824 bytes. Keep in mind that larger
buffers might fail to allocate if device is running low on memory.

**Parameters:**

- `size`: `number` - Size of the buffer in bytes. Must be a positive integer.

### `buffer.fromstring`

Creates a buffer initialized to the contents of the string. The size of
the buffer equals the length of the string.

**Parameters:**

- `str`: `string`

### `buffer.tostring`

Returns the buffer data as a string.

**Parameters:**

- `b`: `buffer`

### `buffer.len`

Returns the size of the buffer in bytes.

**Parameters:**

- `b`: `buffer`

### `buffer.readbits`

Reads a range of bits into an unsigned integer from the buffer based on a
specific `bitCount` integer from `0` to `32`, inclusive. For example:

- `buffer.readbits(b, 0, 8)` is equivalent to
  `Library.buffer.readu8(b, 0)`.
- `buffer.readbits(b, 0, 16)` is equivalent to
  `Library.buffer.readu16(b, 0)`.
- `buffer.readbits(b, 0, 32)` is equivalent to
  `Library.buffer.readu32(b, 0)`.
- `buffer.readbits(b, 0, 24)` reads 24 bits from the buffer.

Note that `0` bit width is supported only to not error in generalized
cases where bit count is dynamic, and reading 0 bits returns `0`. Also
note that, since the max size of the buffer is 1&nbsp;GB, `bitOffset`
cannot be handled as a 32‑bit integer number like byte offset in other
buffer functions.

**Parameters:**

- `b`: `buffer`
- `bitOffset`: `number` - Offset from the beginning of the buffer memory, starting from `0`.
- `bitCount`: `number` - Integer bit count to read. Error is thrown if this value is not in
range of `0` to `32`, inclusive.

### `buffer.readi8`

Reads the data from the buffer by reinterpreting bytes at the offset as an
8-bit signed integer and converting it into a number.

**Parameters:**

- `b`: `buffer`
- `offset`: `number` - Offset from the beginning of the buffer memory, starting from `0`.

### `buffer.readu8`

Reads the data from the buffer by reinterpreting bytes at the offset as an
8-bit unsigned integer and converting it into a number.

**Parameters:**

- `b`: `buffer`
- `offset`: `number` - Offset from the beginning of the buffer memory, starting from `0`.

### `buffer.readi16`

Reads the data from the buffer by reinterpreting bytes at the offset as a
16-bit signed integer and converting it into a number.

**Parameters:**

- `b`: `buffer`
- `offset`: `number` - Offset from the beginning of the buffer memory, starting from `0`.

### `buffer.readu16`

Reads the data from the buffer by reinterpreting bytes at the offset as a
16-bit unsigned integer and converting it into a number.

**Parameters:**

- `b`: `buffer`
- `offset`: `number` - Offset from the beginning of the buffer memory, starting from `0`.

### `buffer.readi32`

Reads the data from the buffer by reinterpreting bytes at the offset as a
32-bit signed integer and converting it into a number.

**Parameters:**

- `b`: `buffer`
- `offset`: `number` - Offset from the beginning of the buffer memory, starting from `0`.

### `buffer.readu32`

Reads the data from the buffer by reinterpreting bytes at the offset as a
32-bit unsigned integer and converting it into a number.

**Parameters:**

- `b`: `buffer`
- `offset`: `number` - Offset from the beginning of the buffer memory, starting from `0`.

### `buffer.readf32`

Reads the data from the buffer by reinterpreting bytes at the offset as a
32-bit floating-point value and converting it into a number. If the
floating-point value matches any bit patterns that represent `NaN` (not a
number), the returned value may be converted to a different quiet `NaN`
representation.

**Parameters:**

- `b`: `buffer`
- `offset`: `number` - Offset from the beginning of the buffer memory, starting from `0`.

### `buffer.readf64`

Reads the data from the buffer by reinterpreting bytes at the offset as a
64-bit floating-point value and converting it into a number. If the
floating-point value matches any bit patterns that represent `NaN` (not a
number), the returned value may be converted to a different quiet `NaN`
representation.

**Parameters:**

- `b`: `buffer`
- `offset`: `number` - Offset from the beginning of the buffer memory, starting from `0`.

### `buffer.writebits`

Writes data to the buffer based on a specific `bitCount` integer from `0`
to `32`, inclusive. `value` is treated as an unsigned 32‑bit number and
only `bitCount` least significant bits are written.

Note that `0` bit width is supported only to not error in generalized
cases where bit count is dynamic, and writing 0 bits has no effect. Also
note that, since the max size of the buffer is 1&nbsp;GB, `bitOffset`
cannot be handled as a 32‑bit integer number like byte offset in other
buffer functions.

**Parameters:**

- `b`: `buffer`
- `bitOffset`: `number` - Offset from the beginning of the buffer memory, starting from `0`.
- `bitCount`: `number` - Integer bit count to write. Error is thrown if this value is not in
range of `0` to `32`, inclusive.
- `value`: `number` - Unsigned 32‑bit number. Only `bitCount` least significant bits are
written.

### `buffer.writei8`

Writes data to the buffer by converting the number into an 8-bit signed
integer and writing a single byte.

**Parameters:**

- `b`: `buffer`
- `offset`: `number` - Offset from the beginning of the buffer memory, starting from `0`.
- `value`: `number` - An integer number in range [-128, 127].

### `buffer.writeu8`

Writes data to the buffer by converting the number into an 8-bit unsigned
integer and writing a single byte.

**Parameters:**

- `b`: `buffer`
- `offset`: `number` - Offset from the beginning of the buffer memory, starting from `0`.
- `value`: `number` - An integer number in range [0, 255].

### `buffer.writei16`

Writes data to the buffer by converting the number into a 16-bit signed
integer and reinterpreting it as individual bytes.

**Parameters:**

- `b`: `buffer`
- `offset`: `number` - Offset from the beginning of the buffer memory, starting from `0`.
- `value`: `number` - An integer number in range [-32,768, 32,767].

### `buffer.writeu16`

Writes data to the buffer by converting the number into a 16-bit unsigned
integer and reinterpreting it as individual bytes.

**Parameters:**

- `b`: `buffer`
- `offset`: `number` - Offset from the beginning of the buffer memory, starting from `0`.
- `value`: `number` - An integer number in range [0, 65,535].

### `buffer.writei32`

Writes data to the buffer by converting the number into a 32-bit signed
integer and reinterpreting it as individual bytes.

**Parameters:**

- `b`: `buffer`
- `offset`: `number` - Offset from the beginning of the buffer memory, starting from `0`.
- `value`: `number` - An integer number in range [-2,147,483,648, 2,147,483,647].

### `buffer.writeu32`

Writes data to the buffer by converting the number into a 32-bit unsigned
integer and reinterpreting it as individual bytes.

**Parameters:**

- `b`: `buffer`
- `offset`: `number` - Offset from the beginning of the buffer memory, starting from `0`.
- `value`: `number` - An integer number in range [0, 4,294,967,295].

### `buffer.writef32`

Writes data to the buffer by converting the number into a 32-bit
floating-point value and reinterpreting it as individual bytes.

**Parameters:**

- `b`: `buffer`
- `offset`: `number` - Offset from the beginning of the buffer memory, starting from `0`.
- `value`: `number` - A single-precision floating-point number.

### `buffer.writef64`

Writes data to the buffer by converting the number into a 64-bit
floating-point value and reinterpreting it as individual bytes.

**Parameters:**

- `b`: `buffer`
- `offset`: `number` - Offset from the beginning of the buffer memory, starting from `0`.
- `value`: `number` - A double-precision floating-point number.

### `buffer.readstring`

Reads a string of length `count` from the buffer at the specified
`offset`.

**Parameters:**

- `b`: `buffer`
- `offset`: `number` - Offset from the beginning of the buffer memory, starting from `0`.
- `count`: `number` - Length to read.

### `buffer.writestring`

Writes data from a string into the buffer at the specified `offset`. If an
optional `count` is specified, only `count` bytes are taken from the
string.

**Parameters:**

- `b`: `buffer`
- `offset`: `number` - Offset from the beginning of the buffer memory, starting from `0`.
- `value`: `string` - Data to write.
- `count`: `number?` - Number of bytes to take from the string. This value cannot be larger
than the string length.

### `buffer.copy`

Copies `count` bytes from `source` starting at offset `sourceOffset` into
the `target` at `targetOffset`.

It's possible for `source` and `target` to be the same. Copying an
overlapping region inside the same buffer acts as if the source region is
copied into a temporary buffer and then that buffer is copied over to the
target.

**Parameters:**

- `target`: `buffer` - Buffer to copy data into.
- `targetOffset`: `number` - Offset from the beginning of the buffer memory, starting from `0`.
- `source`: `buffer` - Buffer to take the data from.
- `sourceOffset`: `number?` - Offset from the beginning of the buffer memory, starting from `0`.
- `count`: `number?` - Number of bytes to copy. If omitted, the whole `source` data starting
from `sourceOffset` is taken.

### `buffer.fill`

Sets `count` bytes in the buffer starting at the specified `offset` to
`value`.

**Parameters:**

- `b`: `buffer` - Buffer to write the data into.
- `offset`: `number` - Offset from the beginning of the buffer memory, starting from `0`.
- `value`: `number` - An integer number in range [0, 255].
- `count`: `number?` - Number of bytes to write. If omitted, all bytes after the specified
offset are set.
