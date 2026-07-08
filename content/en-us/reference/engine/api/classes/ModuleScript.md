---
title: ModuleScript
type: class
superclass: LuaSourceContainer
---

# ModuleScript

A script type that runs once when `Global.LuaGlobals.require()` is called with
it. Returns exactly one value, usually a table of functions, to used by other
scripts. Useful for compartmentalizing code.

**Inherits from:** `Class.LuaSourceContainer` > `Class.Instance` > `Class.Object`

## Description

A `Class.ModuleScript` is a script type that returns exactly one value by a
call to `Global.LuaGlobals.require()`. `Class.ModuleScript|ModuleScripts` run
once and only once per Luau environment and return the exact same value for
subsequent calls to `Global.LuaGlobals.require()`.

`Class.ModuleScript|ModuleScripts` are essential objects for adhering to the
"Don't Repeat Yourself" (DRY) principle, allowing you to write a function only
once and use it everywhere. Having multiple copies of a function is
problematic when you need to change their behavior, so you should define
functions or groups of functions in `Class.ModuleScript|ModuleScripts` and
have your `Class.Script|Scripts` and `Class.LocalScript|LocalScripts` call
`Global.LuaGlobals.require()` on those modules.

It's important to know that return values from
`Class.ModuleScript|ModuleScripts` are independent with regards to
`Class.Script|Scripts` and `Class.LocalScript|LocalScripts`, and other
environments like the
[Command&nbsp;Bar](../../../studio/ui-overview.md#command-bar). Using
`Global.LuaGlobals.require()` on a `Class.ModuleScript` in a
`Class.LocalScript` will run the code on the client, even if a `Class.Script`
did so already on the server. Therefore, be careful if you're using a
`Class.ModuleScript` on the client and server at the same time, or debugging
it within Studio.

Note that the first call to `Global.LuaGlobals.require()` will not yield
(halt) unless the `Class.ModuleScript` yields (calls `Library.task.wait()` for
example), in which case the current thread that called
`Global.LuaGlobals.require()` will yield until the `Class.ModuleScript`
returns a value. If a `Class.ModuleScript` is attempting to
`Global.LuaGlobals.require()` another `Class.ModuleScript` that in turn tries
to `Global.LuaGlobals.require()` it, the thread will **hang and never halt**
(cyclic `Global.LuaGlobals.require()` calls do not generate errors). Be
mindful of your module dependencies in large projects!

If a `Class.ModuleScript` is uploaded to Roblox and the root module has the
name set to `MainModule`, it can be uploaded as a model and required using
`Global.LuaGlobals.require()` with the model's asset ID. Then it can be loaded
into your experience, although this logic only works on the server and will
error on the client. If other users want to use the module, it must be public.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ModuleScript.LinkedSource` | `Datatype.ContentId` | [Deprecated] |
| `Class.ModuleScript.Source` | `Datatype.ProtectedString` |  |
