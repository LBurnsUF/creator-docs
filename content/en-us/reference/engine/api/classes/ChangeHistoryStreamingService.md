---
title: ChangeHistoryStreamingService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# ChangeHistoryStreamingService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Events

### `Class.ChangeHistoryStreamingService.SendCreateInstanceFromStudio`

Fires with: (parentInstance: `Class.Instance`, instance: `Class.Instance`)

### `Class.ChangeHistoryStreamingService.SendDeleteInstanceFromStudio`

Fires with: (instance: `Class.Instance`, setParentToNull: `bool`)

### `Class.ChangeHistoryStreamingService.SendReparentInstanceFromStudio`

Fires with: (parentInstance: `Class.Instance`, instance: `Class.Instance`)

### `Class.ChangeHistoryStreamingService.SendTerrainChangeFromStudio`

Fires with: (instance: `Class.Instance`, chunkX: `int`, chunkY: `int`, chunkZ: `int`, cells: `string`)
