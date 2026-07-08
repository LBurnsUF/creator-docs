---
title: MessageBusService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# MessageBusService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.MessageBusService:Call`

``Call(key: `string`, input: `Variant`)`` -> `Variant`
   {security: RobloxScriptSecurity}

### `Class.MessageBusService:GetLast`

``GetLast(mid: `string`)`` -> `Variant`
   {security: RobloxScriptSecurity}

### `Class.MessageBusService:GetMessageId`

``GetMessageId(domainName: `string`, messageName: `string`)`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.MessageBusService:GetProtocolMethodRequestMessageId`

``GetProtocolMethodRequestMessageId(protocolName: `string`, methodName: `string`)`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.MessageBusService:GetProtocolMethodResponseMessageId`

``GetProtocolMethodResponseMessageId(protocolName: `string`, methodName: `string`)`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.MessageBusService:MakeRequest`

``MakeRequest(protocolName: `string`, methodName: `string`, message: `Variant`, callback: `Datatype.Function`, customTelemetryData: `Variant`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MessageBusService:Publish`

``Publish(mid: `string`, params: `Variant`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MessageBusService:PublishProtocolMethodRequest`

``PublishProtocolMethodRequest(protocolName: `string`, methodName: `string`, message: `Variant`, customTelemetryData: `Variant`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MessageBusService:PublishProtocolMethodResponse`

``PublishProtocolMethodResponse(protocolName: `string`, methodName: `string`, message: `Variant`, responseCode: `int`, customTelemetryData: `Variant`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MessageBusService:SetRequestHandler`

``SetRequestHandler(protocolName: `string`, methodName: `string`, callback: `Datatype.Function`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MessageBusService:Subscribe`

``Subscribe(mid: `string`, callback: `Datatype.Function`, once: `bool`, sticky: `bool`)`` -> `Class.Instance`
   {security: RobloxScriptSecurity}

### `Class.MessageBusService:SubscribeToProtocolMethodRequest`

``SubscribeToProtocolMethodRequest(protocolName: `string`, methodName: `string`, callback: `Datatype.Function`, once: `bool`, sticky: `bool`)`` -> `Class.Instance`
   {security: RobloxScriptSecurity}

### `Class.MessageBusService:SubscribeToProtocolMethodResponse`

``SubscribeToProtocolMethodResponse(protocolName: `string`, methodName: `string`, callback: `Datatype.Function`, once: `bool`, sticky: `bool`)`` -> `Class.Instance`
   {security: RobloxScriptSecurity}
