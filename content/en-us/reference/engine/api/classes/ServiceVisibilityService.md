---
title: ServiceVisibilityService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# ServiceVisibilityService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.ServiceVisibilityService.HiddenServices` | `Datatype.BinaryString` |  {security: RobloxSecurity} |
| `Class.ServiceVisibilityService.VisibleServices` | `Datatype.BinaryString` |  {security: RobloxSecurity} |

## Methods

### `Class.ServiceVisibilityService:SetServiceVisibilityPreference`

``SetServiceVisibilityPreference(service: `Class.Instance`, visible: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.ServiceVisibilityService.ServiceVisibilityChanged`

Fires with: (serviceName: `string`)
