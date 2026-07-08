---
title: TickCountSampleMethod
type: enum
---

# `Enum.TickCountSampleMethod`

Controls the precision of a timer.

Compute time using a faster, but less precise method.

The `Enum.TickCountSampleMethod` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.TickCountSampleMethod.Fast` | 0 | Compute time using a faster, but less precise method. |
| `Enum.TickCountSampleMethod.Benchmark` | 1 | Dynamically decide between using ''Fast'' and ''Precise'' depending on performance. |
| `Enum.TickCountSampleMethod.Precise` | 2 | Compute time using a precise method. |
