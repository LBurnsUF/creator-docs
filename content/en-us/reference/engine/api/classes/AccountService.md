---
title: AccountService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# AccountService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **DeviceAccessTokenAvailable**() -> `bool`
- **DeviceIntegrityAvailable**() -> `bool`
- **GetCredentialsHeaders**() -> `string` [Yields]
- **GetDeviceAccessToken**() -> `string` [Yields]
- **GetDeviceIntegrityToken**(`data: string`) -> `string`
- **GetDeviceIntegrityTokenYield**(`data: string`) -> `string` [Yields]
- **MagicLogin**(`data: string`) -> `null`

## Events

- **MagicLoginEvent**(`data: string`)
