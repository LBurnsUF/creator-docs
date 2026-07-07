---
title: ServiceProvider
type: class
superclass: Instance
tags: [NotCreatable, NotBrowsable]
---

# ServiceProvider

**Inherits**: Instance > Object

**Tags**: NotCreatable, NotBrowsable

## Methods

- **FindService**(`className: string`) -> `Instance`
- **GetService**(`className: string`) -> `Instance`
- **getService**(`className: string`) -> `Instance` [Deprecated]
- **service**(`className: string`) -> `Instance` [Deprecated]

## Events

- **Close**()
- **CloseLate**()
- **ServiceAdded**(`service: Instance`)
- **ServiceRemoving**(`service: Instance`)
