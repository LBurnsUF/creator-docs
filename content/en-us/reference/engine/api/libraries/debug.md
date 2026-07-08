---
title: debug
type: library
---

# `debug`

This library provides functions useful for debugging and profiling code.

## Description

Provides a few basic functions for debugging code in Roblox. Unlike the
`Library.debug` library found in Lua natively, this version has been heavily
sandboxed.

## Functions

### `debug.traceback`

Returns a traceback of the current function call stack as a string; in
other words, a description of the functions that have been called up to
this point. During debugging, this behaves like an error stack trace but
does not stop execution of the script.

The `level` parameter specifies what level of the call stack to consider,
with `1` being the call of `Library.debug.traceback()` itself, `2` being
the call of the function calling `Library.debug.traceback()`, and so on.
See the code sample below for an example of sequential function calls.

Note that this function will often return inaccurate results (compared to
the original source code) and that the format of the returned traceback
may change at any time. You should **not** parse the return value for
specific information such as script names or line numbers.

The following example includes sequential function calls; `fnB()` is
called, and it calls `fnA()` which then calls `Library.debug.traceback()`.

```lua
local function fnA()
	print(debug.traceback("Specific moment during fnA()"))
end

local function fnB()
	fnA()
end

-- Call function fnB() to begin traceback
fnB()
```

**Parameters:**

- `message`: `string` - The first line of the returned string.
- `level`: `number` - The number of calls "up" the call stack to return.

**Returns:** Traceback of the current function call stack.

### `debug.traceback`

Returns a traceback of the current function call stack as a string; in
other words, a description of the functions that have been called up to
this point. During debugging, this behaves like an error stack trace but
does not stop execution of the script.

The `level` parameter specifies what level of the call stack to consider,
with `1` being the call of `Library.debug.traceback()` itself, `2` being
the call of the function calling `Library.debug.traceback()`, and so on.
See the code sample below for an example of sequential function calls.

Note that this function will often return inaccurate results (compared to
the original source code) and that the format of the returned traceback
may change at any time. You should **not** parse the return value for
specific information such as script names or line numbers.

The following example includes sequential function calls; `fnB()` is
called, and it calls `fnA()` which then calls `Library.debug.traceback()`.

```lua
local function fnA()
	print(debug.traceback("Specific moment during fnA()"))
end

local function fnB()
	fnA()
end

-- Call function fnB() to begin traceback
fnB()
```

**Parameters:**

- `thread`: `thread` - A thread as returned by `Library.coroutine.create()`.
- `message`: `string` - The first line of the returned string.
- `level`: `number` - The number of calls "up" the call stack to return.

**Returns:** Traceback of the current function call stack.

### `debug.info`

Allows programmatic inspection of the call stack. This function differs
from `Library.debug.traceback()` in that it guarantees the format of the
data it returns. This is useful for general logging and filtering purposes
as well as for sending the data to systems expecting structured input,
such as crash aggregation.

```lua
local function fnA()
	-- Output source identifier ("s") and line ("l") at levels 1 and 2
	print(debug.info(1, "sl"))  --> fnA() 3
	print(debug.info(2, "sl"))  --> fnA() 7
end

fnA()
```

Note that this function is similar to
[debug.getinfo](https://www.lua.org/pil/23.1.html), an unavailable part of
the standard Lua library which serves a similar purpose.

**Parameters:**

- `level`: `number` - Determines at what level of the call stack the information returned
should describe. A value of `1` represents the function which is
calling `Library.debug.info()`, a value of `2` represents the function
that called that function, and so on.
- `options`: `string` - A string that describes what the returned information should
represent. It must only contain 0 or 1 instances of the characters
`slnaf`, each representing a piece of information:

- `s` ([string](/luau/strings.md)) — The function source identifier,
  equal to the full name of the script the function is defined in.
- `l` ([number](/luau/numbers.md)) — The line number of the function
  call represented by `level`.
- `n` ([string](/luau/strings.md)) — The name of the function; may be
  `nil` for anonymous functions and C functions without an assigned
  debug name.
- `a` ([number](/luau/numbers.md), [boolean](/luau/booleans.md)) —
  Arity of the function, which refers to the parameter count and
  whether the function is variadic.
- `f` ([function](/luau/functions.md)) — The function which was
  inspected.

### `debug.info`

Allows programmatic inspection of the call stack. This function differs
from `Library.debug.traceback()` in that it guarantees the format of the
data it returns. This is useful for general logging and filtering purposes
as well as for sending the data to systems expecting structured input,
such as crash aggregation.

```lua
local function fnA()

end

local function fnB()

end

-- Output line ("l"), name ("n"), and identifier ("f") for both fnA() and fnB()
print(debug.info(fnA, "lnf"))  --> 1 fnA function: 0x75e3d3c398a81252
print(debug.info(fnB, "lnf"))  --> 5 fnB function: 0x6022a6dc5ccf4ab2
```

Note that this function is similar to
[debug.getinfo](https://www.lua.org/pil/23.1.html), an unavailable part of
the standard Lua library which serves a similar purpose.

**Parameters:**

- `function`: `function` - The function of the call stack which the information returned should
describe.
- `options`: `string` - A string that describes what the returned information should
represent. It must only contain 0 or 1 instances of the characters
`slnaf`, each representing a piece of information:

- `s` ([string](/luau/strings.md)) — The function source identifier,
  equal to the full name of the script the function is defined in.
- `l` ([number](/luau/numbers.md)) — The line that `function` is
  defined on.
- `n` ([string](/luau/strings.md)) — The name of the function; may be
  `nil` for anonymous functions and C functions without an assigned
  debug name.
- `a` ([number](/luau/numbers.md), [boolean](/luau/booleans.md)) —
  Arity of the function, which refers to the parameter count and
  whether the function is variadic.
- `f` ([function](/luau/functions.md)) — The function which was
  inspected.

### `debug.info`

Allows programmatic inspection of the call stack. This function differs
from `Library.debug.traceback()` in that it guarantees the format of the
data it returns. This is useful for general logging and filtering purposes
as well as for sending the data to systems expecting structured input,
such as crash aggregation.

```lua
local function fnA()
	-- Output source identifier ("s") and line ("l") at levels 1 and 2
	print(debug.info(1, "sl"))  --> fnA() 3
	print(debug.info(2, "sl"))  --> fnA() 7
end

fnA()
```

Note that this function is similar to
[debug.getinfo](https://www.lua.org/pil/23.1.html), an unavailable part of
the standard Lua library which serves a similar purpose.

**Parameters:**

- `thread`: `thread` - A thread as returned by `Library.coroutine.create()`.
- `level`: `number` - Determines at what level of the call stack the information returned
should describe. A value of `1` represents the function which is
calling `Library.debug.info()`, a value of `2` represents the function
that called that function, and so on.
- `options`: `string` - A string that describes what the returned information should
represent. It must only contain 0 or 1 instances of the characters
`slnaf`, each representing a piece of information:

- `s` ([string](/luau/strings.md)) — The function source identifier,
  equal to the full name of the script the function is defined in.
- `l` ([number](/luau/numbers.md)) — The line number of the function
  call represented by `level`.
- `n` ([string](/luau/strings.md)) — The name of the function; may be
  `nil` for anonymous functions and C functions without an assigned
  debug name.
- `a` ([number](/luau/numbers.md), [boolean](/luau/booleans.md)) —
  Arity of the function, which refers to the parameter count and
  whether the function is variadic.
- `f` ([function](/luau/functions.md)) — The function which was
  inspected.

### `debug.profilebegin`

Starts profiling for a
[MicroProfiler](../../../studio/microprofiler/index.md) label.

**Parameters:**

- `label`: `string` - The text that this
[MicroProfiler](../../../studio/microprofiler/index.md) label
displays.

### `debug.profileend`

Stops profiling for the most recent
[MicroProfiler](../../../studio/microprofiler/index.md) label that
`Library.debug.profilebegin()` opened.

### `debug.getmemorycategory`

Returns the name of the current thread's active memory category.

**Returns:** The current thread's active memory category.

### `debug.setmemorycategory`

Assigns a custom tag name to the current thread's memory category in the
[Developer Console](../../../studio/developer-console.md). Useful for
analyzing memory usage of multiple threads in the same script which would
otherwise be grouped together under the same tag/name. Returns the name of
the current thread's previous memory category.

**Parameters:**

- `tag`: `string`

**Returns:** The current thread's previous memory category.

### `debug.resetmemorycategory`

Resets the tag assigned by `Library.debug.setmemorycategory()` to the
automatically assigned value (typically, the script name).

### `debug.dumpcodesize`

Displays a table of native code size of individual functions and scripts.
This function is only available in the Command Bar in Studio. More details
can be found on the
[Native Code Generation](../../../luau/native-code-gen.md) page.
