---
title: ServiceProvider
type: class
superclass: Instance
tags: [NotCreatable, NotBrowsable]
---

# ServiceProvider

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotBrowsable]

## Methods

### `Class.ServiceProvider:FindService`

``FindService(className: `string`)`` → `Class.Instance`

### `Class.ServiceProvider:GetService`

``GetService(className: `string`)`` → `Class.Instance`

### `Class.ServiceProvider:getService`

``getService(className: `string`)`` → `Class.Instance`
  [Deprecated]

### `Class.ServiceProvider:service`

``service(className: `string`)`` → `Class.Instance`
  [Deprecated]

## Events

### `Class.ServiceProvider.Close`

Fires with: ()

### `Class.ServiceProvider.CloseLate`

Fires with: ()

### `Class.ServiceProvider.ServiceAdded`

Fires with: (service: `Class.Instance`)

### `Class.ServiceProvider.ServiceRemoving`

Fires with: (service: `Class.Instance`)
