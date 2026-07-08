---
title: SaveFilter
type: enum
---

# `Enum.SaveFilter`

Used by `Class.DataModel.SavePlace` to determine the type of save operation
This enum determines which aspects of the current place are saved, based on
the following options.

The `Enum.SaveFilter` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.SaveFilter.SaveWorld` | 0 | Saves only the world-related data. |
| `Enum.SaveFilter.SaveGame` | 1 | Saves only the game-related data. |
| `Enum.SaveFilter.SaveAll` | 2 | Saves all data, including both world and game-related information. |
