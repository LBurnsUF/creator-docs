---
title: ScriptVariableScope
type: enum
---

# `Enum.ScriptVariableScope`

Indicates the scope category of a variable returned by the debugger.

Used in `Datatype.ScriptVariable` to classify the scope of a variable returned
by `Class.ScriptDebuggerService:GetRootVariables()` or
`Class.ScriptDebuggerService:GetVariables()`. Children of a variable inherit
the parent's scope.

The `Enum.ScriptVariableScope` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.ScriptVariableScope.Local` | 0 | A local variable declared in the current function scope. |
| `Enum.ScriptVariableScope.Upvalue` | 1 | A variable captured from an enclosing function scope. |
| `Enum.ScriptVariableScope.Global` | 2 | A global variable. |
