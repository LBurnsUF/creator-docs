---
title: SignalBehavior
type: enum
---

# `Enum.SignalBehavior`

Determines when the engine resumes event handlers.

Determines when the engine resumes event handlers. At some future point, the
default mode will be `Deferred` but opt-out will still be possible through use
of `Immediate`.

For more information, see
[Deferred Events](../../../scripting/events/deferred.md).

The `Enum.SignalBehavior` enum has 4 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.SignalBehavior.Default` | 0 | The default behavior; currently equivalent to `Immediate` but this will eventually change to `Deferr |
| `Enum.SignalBehavior.Immediate` | 1 | Event handlers are resumed immediately when the event occurs. |
| `Enum.SignalBehavior.Deferred` | 2 | All events are deferred and their handlers resumed at specific resumptions points each frame. |
| `Enum.SignalBehavior.AncestryDeferred` | 3 | Equivalent to `Deferred` but only for events triggered by changes in ancestry. |
