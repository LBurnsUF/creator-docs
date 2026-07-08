---
title: table
type: library
---

# `table`

A library of table functions.

## Description

This library provides generic functions for table/array manipulation,
providing all its functions inside the global `Library.table` variable. Most
functions in the `Library.table` library assume that the table represents an
array or a list. For these functions, the "length" of a table means the result
of the length operator.

## Functions

### `table.clear`

Sets the value for all keys within the given table to `nil`. This causes
the `#` operator to return `0` for the given table. The allocated capacity
of the table's array portion is maintained, which allows for efficient
re-use of the space.

```lua
local grades = {95, 82, 71, 92, 100, 60}
print(grades[4], #grades) --> 92, 6
table.clear(grades)
print(grades[4], #grades) --> nil, 0
-- If grades is filled again with the same number of entries,
-- no potentially expensive array resizing will occur
-- because the capacity was maintained by table.clear.
```

This function does not delete/destroy the table provided to it. This
function is meant to be used specifically for tables that are to be
re-used.

**Parameters:**

- `table`: `table` - The table whose keys will be cleared.

### `table.clone`

Returns an unfrozen shallow copy of the provided table.

```lua
local original = {
	key = "value",
	engine = "Roblox",
	playerID = 505306092
}

local clone = table.clone(original)
```

**Parameters:**

- `t`: `table` - The table to be cloned.

**Returns:** The clone of the provided table.

### `table.concat`

Given an array where all elements are strings or numbers, returns the
string `t[i] ... sep ... t[i+1] ... sep ... t[j]`. The default value for
sep is an empty string, the default for `i` is 1, and the default for `j`
is #t. If i is greater than `j`, returns the empty string.

**Parameters:**

- `t`: `Array` - The table that will be converted into a string.
- `sep`: `string` - The string that will be concatenated between each entry in the table.
- `i`: `int` - The starting index of the table concatenation.
- `j`: `int` - The ending index of the table concatenation.

### `table.create`

Creates a table with the array portion allocated to the given `number` of
elements, optionally filled with the given `value`.

```lua
local t = table.create(3, "Roblox")
print(table.concat(t)) --> RobloxRobloxRoblox
```

If you are inserting into large array-like tables and are certain of a
reasonable upper limit to the number of elements, it's recommended to use
this function to initialize the table. This ensures the table's array
portion of its memory is sufficiently sized, as resizing it can be
expensive. For small quantities this is typically not noticeable.

**Parameters:**

- `count`: `number`
- `value`: `Variant`

### `table.find`

Within the given array-like table `haystack`, find the first occurrence of
value `needle`, starting from index `init` or the beginning if not
provided. If the value is not found, `nil` is returned.

A [linear search](https://en.wikipedia.org/wiki/Linear_search) algorithm
is performed.

```lua
local t = {"a", "b", "c", "d", "e"}
print(table.find(t, "d")) --> 4
print(table.find(t, "z")) --> nil, because z is not in the table
print(table.find(t, "b", 3)) --> nil, because b appears before index 3
```

**Parameters:**

- `haystack`: `table`
- `needle`: `Variant`
- `init`: `number`

### `table.foreach`

Iterates over the provided table, passing the key and value of each
iteration over to the provided function. This function has been deprecated
and is not recommended for use in new code; use a `for` loop instead.

**Parameters:**

- `t`: `table` - The table to be iterated over.
- `f`: `function` - The function that will be used for the iteration. This function will
receive 2 arguments for each iteration, where the 1st argument is the
key, and the 2nd argument is the value.

### `table.foreachi`

This is similar to `Library.table.foreach()` except that index-value pairs
are passed, not key-value pairs. This function has been deprecated and is
not recommended for use in new code; use a `for` loop instead.

**Parameters:**

- `t`: `Array` - The table to be iterated over.
- `f`: `function` - The function that will be used for the iteration. This function will
receive 2 arguments for each iteration, where the 1st argument is the
index, and the 2nd argument is the value.

### `table.freeze`

This function makes the given table read-only, effectively "freezing" it
in its current state. Attempting to modify a frozen table throws an error.

This freezing effect is shallow, which means that you can write to a table
within a frozen table. To deep freeze a table, call this function
recursively on all of the descending tables.

**Parameters:**

- `t`: `table` - The table to be frozen.

**Returns:** The frozen table.

### `table.getn`

Returns the number of elements in the table passed. This function has been
deprecated and is not recommended for use in new code; use `#t` instead.

**Parameters:**

- `t`: `Array` - The table whose size is being measured.

### `table.insert`

Inserts the provided value to the target position of the array.

**Parameters:**

- `t`: `Array` - The table that is being appended to.
- `pos`: `number` - The position at which the value will be inserted.
- `value`: `Variant` - The value that will be appended to the table.

### `table.insert`

Appends the provided value to the end of the array.

**Parameters:**

- `t`: `Array` - The table that is being appended to.
- `value`: `Variant` - The value that will be appended to the table.

### `table.isfrozen`

This function returns `true` if the given table is frozen and `false` if
it isn't frozen. You can freeze tables using `Library.table.freeze()`.

**Parameters:**

- `t`: `table` - The table to check.

**Returns:** Whether the table is frozen from `Library.table.freeze()`.

### `table.maxn`

Returns the maximum numeric key of the provided table, or zero if the
table has no numeric keys. Gaps in the table are ignored.

**Parameters:**

- `t`: `table`

### `table.move`

Copies elements in table `src` from `src[a]` up to `src[b]` into table
`dst` starting at index `t`. Equivalent to the assignment statement
`dst[t], ..., dst[t + (b - a)] = src[a], ..., src[b]`.

The default for `dst` is `src`. The destination range may overlap with the
source range. Returns `dst` for convenience.

```lua
local sourceTable = {4, 5} -- Table of data to copy from
local destTable = {1, 2, 3} -- Table to add copied data to

table.move(
	sourceTable, -- Source table
	1, -- Index to start from in source table
	#sourceTable, -- Index up to (and including) from source table
	#destTable + 1, -- Index within destination table to move data into
	destTable -- Destination table
)
print(destTable) --> {1, 2, 3, 4, 5}
```

**Parameters:**

- `src`: `table` - Source table.
- `a`: `number` - Start copying at `src[a]`.
- `b`: `number` - Copy up to and including `src[b]`.
- `t`: `number` - Copy into `dst[t], ...`.
- `dst`: `table` - Destination table.

**Returns:** `dst` for convenience.

### `table.pack`

Returns a new table with all arguments stored into keys 1, 2, etc. and
with a field "n" with the total number of arguments. Note that the
resulting table may not be a sequence.

```lua
local t = table.pack(1, 2, 3)
print(table.concat(t, ", ")) --> 1, 2, 3
```

**Parameters:**

- `values...`: `Variant`

### `table.remove`

Removes from array t the element at position pos, returning the value of
the removed element. When pos is an integer between `1` and `#t`, it
shifts down the elements `t[pos+1], t[pos+2], ..., t[#t]` and erases
element `t[#t]`. If the pos parameter is not provided, pos defaults to the
length of the table removing the last element.

**Parameters:**

- `t`: `Array` - The table that is having an element removed.
- `pos`: `number` - The index of the element being removed.

### `table.sort`

Sorts elements of array t in a given order, from `t[1]` to `t[#t]`. If
`comp` is given, then it must be a function that receives two elements and
returns true when the first element must come before the second in the
final order.

The error `invalid order function for sorting` is thrown if both
`comp(a, b)` and `comp(b, a)` return `true`.

If `comp` is not given, then the standard Luau operator `<` is used
instead.

**Parameters:**

- `t`: `Array`
- `comp`: `function` - An optional comparison function to be used when comparing elements in
the table. This function receives two elements, and should return true
if the first element should be sorted before the second in the final
order.

### `table.unpack`

Returns the elements from the given list. By default, `i` is 1 and `j` is
the length of `list`.

Note that this same functionality is also provided by the global
`Global.LuaGlobals.unpack()` function.

**Parameters:**

- `list`: `table` - The list of elements to be unpacked.
- `i`: `number` - The index of the first element to unpack.
- `j`: `number` - The index of the last element to unpack.
