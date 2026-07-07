---
title: ChangeHistoryStreamingService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# ChangeHistoryStreamingService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Events

- **SendCreateInstanceFromStudio**(`parentInstance: Instance`, `instance: Instance`)
- **SendDeleteInstanceFromStudio**(`instance: Instance`, `setParentToNull: bool`)
- **SendReparentInstanceFromStudio**(`parentInstance: Instance`, `instance: Instance`)
- **SendTerrainChangeFromStudio**(`instance: Instance`, `chunkX: int`, `chunkY: int`, `chunkZ: int`, `cells: string`)
