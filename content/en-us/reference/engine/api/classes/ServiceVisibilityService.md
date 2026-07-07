---
title: ServiceVisibilityService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# ServiceVisibilityService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Properties

- **HiddenServices**: `BinaryString` (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **VisibleServices**: `BinaryString` (Security: Read=RobloxSecurity, Write=RobloxSecurity)

## Methods

- **SetServiceVisibilityPreference**(`service: Instance`, `visible: bool`) -> `null`

## Events

- **ServiceVisibilityChanged**(`serviceName: string`)
