---
title: Roblox globals
type: globals
---

# Roblox globals

Built-in functions and constants unique to Roblox.

Roblox provides several unique built-in functions and variables in its
embedding of Luau. These are only found on Roblox and are not packaged by
default with Luau or Lua.

## Properties

### `Enum`

A reference to the Enums data type, which stores all of the available
enums that can be used on Roblox.

### `game`

A reference to the `Class.DataModel`, which is the root Instance of
Roblox's parent/child hierarchy.

### `plugin`

A reference to the `Class.Plugin` object that represents the plugin being
run from this `Class.Script`. This reference exists only in the context
where a script is executed as a plugin and is not passed to
`Class.ModuleScript|ModuleScripts` within the plugin. To use this
reference in a `Class.ModuleScript`, you must explicitly pass it.

```lua
assert(plugin, "This script must be run as a plugin!")
-- Code beyond this point will execute only if the script is run as a plugin
```

### `shared`

A table that is shared across all scripts that share the same execution
context level. This serves the exact same purpose as `_G`.

### `script`

A reference to the script object that is executing the code you are
writing. It can be either a `Class.Script`, a `Class.LocalScript`, or a
`Class.ModuleScript`. This variable is not available when executing code
from Roblox Studio's command bar.

### `workspace`

A reference to the `Class.Workspace` service, which contains all of the
physical components of a Roblox world.

## Functions

### `delay`

Schedules a function to be executed after `delayTime` seconds have passed,
without yielding the current thread. This function allows multiple Luau
threads to be executed in parallel from the same stack. The delay will
have a minimum duration of 29 milliseconds, but this minimum may be higher
depending on the target framerate and various throttling conditions. If
the `delayTime` parameter is not specified, the minimum duration will be
used.

**Parameters:**

- `delayTime`: `number` - The amount of time that this function will be queued before being
executed.
- `callback`: `function` - The function that will be executed once `delayTime` seconds have
passed.

### `DebuggerManager`

Returns the legacy `DebuggerManager` class which acts as an interface for
Roblox's Luau debugger feature.

This function is not recognized by Luau's analysis tool and will raise an
undefined global warning.

### `elapsedTime`

Returns how much time has elapsed since the current instance of Roblox was
started. In Roblox Studio, this begins counting up from the moment Roblox
Studio starts running, not just when opening a place.

### `PluginManager`

Returns the `Class.PluginManager` which is a deprecated singleton that was
previously required to create plugins. It still has some applicable uses,
such as if you need to create a `Class.Plugin` object from Studio's
[Command Bar](../../../studio/ui-overview.md#command-bar).

### `printidentity`

Prints `Current identity is [ID]` to the output, where [ID] corresponds to
the current thread's security context level.

**Parameters:**

- `prefix`: `string`

### `settings`

Returns the `Class.GlobalSettings` object, which can be used to access the
settings objects that are used in Roblox Studio's settings menu.

### `spawn`

Runs the specified callback function in a separate thread, without
yielding the current thread.

The function will be executed the next time Roblox's Task Scheduler runs
an update cycle. This delay will take at least 29 milliseconds but can
arbitrarily take longer, depending on the target framerate and various
throttling conditions.

The callback function is invoked with two arguments:

1. The first being the amount of time which elapsed from when spawn was
   called to when the function was invoked.
2. The second being equivalent to elapsedTime() or roughly how long the
   engine has been running.

```lua
spawn(print) -- 0.0079617658390703 451.55683163643
```

**Parameters:**

- `callback`: `function` - The function that will be executed.

### `stats`

Returns the `Class.Stats` service. It is preferred that developers use
`Class.ServiceProvider:GetService()` to retrieve it instead.

### `tick`

Returns how much time has elapsed, in seconds, since the Unix epoch, on
the current local session's computer. The Unix epoch is represented by
00:00:00 on 1 January 1970.

`tick()` isn't officially deprecated, but has a variety of issues. It can
be off by up to one second and returns inconsistent results across time
zones and operating systems. Use `Library.os.time()`,
`Library.os.clock()`, or `Global.RobloxGlobals.time()` instead. Also
consider `Datatype.DateTime.UnixTimestamp` and
`Datatype.DateTime.UnixTimestampMillis`.

### `time`

Returns the amount of time, in seconds, that has elapsed since the current
game instance started running. If the current game instance is not
running, this will be `0`.

If `Class.Workspace.AuthorityMode` is `Enum.AuthorityMode.Server`, this
value is synchronized between client and server.

### `typeof`

Returns the type of the object specified, as a string. This function is
more accurate than Luau's native `type` function, as it does not denote
Roblox-specific types as `userdata`.

**Parameters:**

- `object`: `Variant` - The Luau type that will have its type checked.

### `UserSettings`

Returns the `Class.UserSettings` object, which is used to read information
from the current user's game menu settings.

### `version`

Returns the current version of Roblox as a string. The integers in the
version string are separated by periods, and each integers represent the
following, in order:

- Generation - The current generation of the application shell that is
  hosting the client.
- Version - The current release version of Roblox.
- Patch - The current patch number for this version of Roblox.
- Commit - The ID of the last internal commit that was accepted into this
  version of the client.

### `wait`

Yields the current thread until the specified amount of seconds have
elapsed.

The delay will have a minimum duration of 29 milliseconds, but this
minimum may be higher depending on the target framerate and various
throttling conditions. If the `seconds` parameter is not specified, the
minimum duration will be used. This function returns:

- Actual time yielded (in seconds).
- Total time since the software was initialized (in seconds).

**Parameters:**

- `seconds`: `number` - Specifies how long the thread should yield for.

### `warn`

Behaves identically to Luau's print function, except the output is styled
as a warning, with yellow text and a timestamp. This function accepts any
number of arguments, and will attempt to convert them into strings which
will then be joined together with spaces between them.

**Parameters:**

- `params`: `Tuple` - This function accepts any number of arguments, and will attempt to
convert them into strings which will then be joined together with
spaces between them.

### `ypcall`

Legacy function to work around an old task scheduling limitation of
`Global.LuaGlobals.pcall()`; should not be used for new work (use
`Global.LuaGlobals.pcall()` instead).

**Parameters:**

- `f`: `function` - The function to be called in protected mode.
- `args`: `Tuple`
