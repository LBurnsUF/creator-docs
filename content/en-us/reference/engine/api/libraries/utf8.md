---
title: utf8
type: library
---

# `utf8`

This library provides basic support for `UTF-8` encoding.

## Description

This library provides basic support for `UTF-8` encoding. This library does
not provide any support for Unicode other than the handling of the encoding.
Any operation that needs the meaning of a character, such as character
classification, is outside its scope.

Unless stated otherwise, all functions that expect a byte position as a
parameter assume that the given position is either the start of a byte
sequence or one plus the length of the subject string. As in the string
library, negative indices count from the end of the string.

You can find a large catalog of usable `UTF-8` characters
[here](https://www.w3schools.com/charsets/ref_html_utf8.asp).

## Properties

### `utf8.utf8.charpattern`

The pattern `"[%z\x01-\x7F\xC2-\xF4][\x80-\xBF]*"`, which matches exactly
zero or more UTF-8 byte sequence, assuming that the subject is a valid
UTF-8 string.

## Functions

### `utf8.char`

Receives zero or more codepoints as integers, converts each one to its
corresponding UTF-8 byte sequence and returns a string with the
concatenation of all these sequences.

**Parameters:**

- `codepoints`: `Tuple<int>`

### `utf8.codes`

Returns an iterator function so that the construction:

```lua
for position, codepoint in utf8.codes(str) do
	-- body
end
```

will iterate over all codepoints in string `str`. It raises an error if it
meets any invalid byte sequence.

**Parameters:**

- `str`: `string` - The string to iterate over.

### `utf8.codepoint`

Returns the codepoints (as integers) from all codepoints in the provided
string (str) that start between byte positions `i` and `j` (both
included). The default for `i` is `1` and for `j` is `i`. It raises an
error if it meets any invalid byte sequence.

**Parameters:**

- `str`: `string`
- `i`: `int` - The index of the codepoint that should be fetched from this string.
- `j`: `int` - The index of the last codepoint between `i` and `j` that will be
returned. If excluded, this will default to the value of `i`.

### `utf8.len`

Returns the number of UTF-8 codepoints in the string _str_ that start
between positions `i` and `j` (both inclusive). The default for `i` is `1`
and for `j` is `-1`. If it finds any invalid byte sequence, returns a nil
value plus the position of the first invalid byte.

**Parameters:**

- `s`: `string`
- `i`: `int` - The starting position.
- `j`: `int` - The ending position.

### `utf8.offset`

Returns the position (in bytes) where the encoding of the `n`‑th codepoint
of `s` (counting from byte position `i`) starts. A negative `n` gets
characters before position `i`. The default for `i` is `1` when `n` is
non-negative and `#s + 1` otherwise, so that `utf8.offset(s, -n)` gets the
offset of the `n`‑th character from the end of the string. If the
specified character is neither in the subject nor right after its end, the
function returns `nil`.

**Parameters:**

- `s`: `string`
- `n`: `int`
- `i`: `int`

### `utf8.graphemes`

Returns an iterator function so that

```lua
for first, last in utf8.graphemes(str) do
	local grapheme = s:sub(first, last)
	-- body
end
```

will iterate the grapheme clusters of the string.

**Parameters:**

- `str`: `string`
- `i`: `number`
- `j`: `number`

### `utf8.nfcnormalize`

Converts the input string to Normal Form C, which tries to convert
decomposed characters into composed characters.

**Parameters:**

- `str`: `string`

### `utf8.nfdnormalize`

Converts the input string to Normal Form D, which tries to break up
composed characters into decomposed characters.

**Parameters:**

- `str`: `string` - The string to convert.
