---
title: ThreadPoolConfig
type: enum
---

# `Enum.ThreadPoolConfig`

Thread pooling scheme for the task scheduler.

Controls the thread pooling scheme of the underlying 'TaskScheduler'.

See TaskScheduler for details.

The `Enum.ThreadPoolConfig` enum has 11 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.ThreadPoolConfig.Auto` | 0 | Let task scheduler make a decision internally. |
| `Enum.ThreadPoolConfig.Threads1` | 1 | Utilize 1 worker thread, ignore the physical CPU core count. |
| `Enum.ThreadPoolConfig.Threads2` | 2 | Utilize 2 worker threads, ignore the physical CPU core count. |
| `Enum.ThreadPoolConfig.Threads3` | 3 | Utilize 3 worker threads, ignore the physical CPU core count. |
| `Enum.ThreadPoolConfig.Threads4` | 4 | Utilize 4 worker threads, ignore the physical CPU core count. |
| `Enum.ThreadPoolConfig.Threads8` | 8 | Utilize 8 worker threads, ignore the physical CPU core count. |
| `Enum.ThreadPoolConfig.Threads16` | 16 | Utilize 16 worker threads, ignore the physical CPU core count. |
| `Enum.ThreadPoolConfig.PerCore1` | 101 | Utilize 1 worker thread per available physical CPU core. |
| `Enum.ThreadPoolConfig.PerCore2` | 102 | Utilize 2 worker threads per available physical CPU core. |
| `Enum.ThreadPoolConfig.PerCore3` | 103 | Utilize 3 worker threads per available physical CPU core. |
| `Enum.ThreadPoolConfig.PerCore4` | 104 | Utilize 4 worker threads per available physical CPU core. |
