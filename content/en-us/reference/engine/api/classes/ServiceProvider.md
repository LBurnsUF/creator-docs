---
title: ServiceProvider
type: class
superclass: Instance
tags: [NotCreatable, NotBrowsable]
---

# ServiceProvider

A ServiceProvider is an abstract class, which stores, and provides certain
singleton classes, depending on what inherited class you are using its members
with.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotBrowsable]

## Description

A ServiceProvider is an abstract class, which stores, and provides certain
singleton classes, depending on what inherited class you are using its members
with.

## Methods

### `Class.ServiceProvider:FindService`

``FindService(className: `string`)`` -> `Class.Instance`

### `Class.ServiceProvider:GetService`

``GetService(className: `string`)`` -> `Class.Instance`

### `Class.ServiceProvider:getService`

``getService(className: `string`)`` -> `Class.Instance`
  [Deprecated]

### `Class.ServiceProvider:service`

``service(className: `string`)`` -> `Class.Instance`
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
