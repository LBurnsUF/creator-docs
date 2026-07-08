---
title: KeyCodeStringFormat
type: enum
---

# `Enum.KeyCodeStringFormat`

Determines the string format returned by
`Class.UserInputService:GetStringForKeyCode()`.

This enum is used with `Class.UserInputService:GetStringForKeyCode()` to
control how the returned key string is formatted. The `Abbreviated` option
provides shortened labels suitable for compact UI elements such as keybind
hints, tooltips, or on-screen button prompts where space is limited.

The `Enum.KeyCodeStringFormat` enum has 2 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.KeyCodeStringFormat.Default` | 0 | Default behavior which returns the full key string, for example `"LeftControl"`, `"Backspace"`, or ` |
| `Enum.KeyCodeStringFormat.Abbreviated` | 1 | Returns a shortened key string when available, for example `"LCtrl"`, `"Bksp"`, or `"Esc"`. |
