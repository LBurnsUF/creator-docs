---
title: SharedTable
type: datatype
---

# `Datatype.SharedTable`

Provides sharable, table-like storage for key/value pairs.

## Description

Represents a table-like data structure that can be shared across execution
contexts. While it can be used for various sorts of general data storage, it
is designed especially for use with
[Parallel Luau](../../../scripting/multithreading.md), where it can be used to
share state across scripts parented under different `Class.Actor` instances.

There are a couple idiomatic ways to communicate shared tables between
scripts. One method is to store and retrieve `Datatype.SharedTable` objects in
the `Class.SharedTableRegistry`. The registry lets any script in the same data
model get or set a `Datatype.SharedTable` by name. Another method is to use
`Class.Actor:SendMessage()` to send a shared table to another `Class.Actor`
inside a message.

Like a Luau table, a `Datatype.SharedTable` object stores a set of key-value
element pairs. Unlike a Luau table, only selected types of objects may be
stored in a SharedTable, similar to other restrictions you'll find elsewhere
in the Roblox Engine.

Keys must either be (1) a string or (2) a nonnegative integer number less than
2<sup>32</sup>. Other kinds of keys are not supported.

Values must have one of the following types: Boolean, Number, Vector, String,
`Datatype.SharedTable`, or a serializable data type. The ability to store a
`Datatype.SharedTable` as a value in another `Datatype.SharedTable` permits
the construction of nested and recursive data structures.

`Datatype.SharedTable` objects are distinct and different
`Datatype.SharedTable` objects never compare equal, even if they have contents
that would compare equal.

Like a Luau table, a `Datatype.SharedTable` object may be frozen, in which
case it is read-only. An attempt to modify a frozen `Datatype.SharedTable`
will raise an error. A frozen `Datatype.SharedTable` can be created by first
creating a (non-frozen, modifiable) `Datatype.SharedTable` with the desired
contents, and then calling `Datatype.SharedTable.cloneAndFreeze()` to create a
frozen clone of it.

## Constructors

### `SharedTable.new`

Returns a new, empty `Datatype.SharedTable`.

```lua
local st = SharedTable.new()
```

### `SharedTable.new`

Returns a new `Datatype.SharedTable` containing elements equivalent to
those in the provided Luau table.

If the provided Luau table contains any keys or values that cannot be
stored in a `Datatype.SharedTable`, construction of the
`Datatype.SharedTable` fails.  See the summary at the top of this page for
a list of types of objects that can be stored in a `Datatype.SharedTable`.
If the Luau table contains any table as a value, that table is converted
into a new `Datatype.SharedTable`.

```lua
local t = {}
t.x = 1
t.y = 2
t.z = {"a", "b", "c"}

local st = SharedTable.new(t)
assert(st.x == 1)
assert(st.y == 2)
assert(st.z[1] == "a")
assert(st.z[2] == "b")
assert(st.z[3] == "c")
```

Note that in some cases it may be desirable to store a `Datatype.SharedTable` in the `Class.SharedTableRegistry`. The `Class.ShareTableRegistry:GetSharedTable()` method provides a convenient way to accomplish this.

**Parameters:**

- `t`: `table` - The Luau table whose elements are to be stored in the new
`Datatype.SharedTable`.

## API Usage (2 locations)

### Used as Parameter Type

- `Class.SharedTableRegistry:SetSharedTable` (parameter `st`)

### Used as Return Type

- `Class.SharedTableRegistry:GetSharedTable`
