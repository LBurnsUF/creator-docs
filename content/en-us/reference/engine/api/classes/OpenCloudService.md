---
title: OpenCloudService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated, Deprecated]
---

# OpenCloudService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated] [Deprecated]

> **Deprecated:** This class is deprecated and should not be used for new work. Use
`Class.HttpService` instead and see the
[In-experience HTTP requests guide](../../../cloud-services/http-service.md).

## Methods

### `Class.OpenCloudService:GetApiV1`

``GetApiV1()`` -> `Class.OpenCloudApiV1`
  [Deprecated]

### `Class.OpenCloudService:HttpRequestAsync`

``HttpRequestAsync(options: `Dictionary`)`` -> `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.OpenCloudService:InvokeAsync`

``InvokeAsync(version: `string`, methodName: `string`, arguments: `Dictionary`, headers: `Dictionary`)`` -> `Dictionary`
  [Yields] [Deprecated]

### `Class.OpenCloudService:RegisterOpenCloud`

``RegisterOpenCloud(version: `string`, methodName: `string`, method: `Datatype.Function`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.OpenCloudService:RegistrationComplete`

``RegistrationComplete()`` -> `null`
   {security: RobloxScriptSecurity}
