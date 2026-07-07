---
title: MessageBusService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# MessageBusService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **Call**(`key: string`, `input: Variant`) -> `Variant`
- **GetLast**(`mid: string`) -> `Variant`
- **GetMessageId**(`domainName: string`, `messageName: string`) -> `string`
- **GetProtocolMethodRequestMessageId**(`protocolName: string`, `methodName: string`) -> `string`
- **GetProtocolMethodResponseMessageId**(`protocolName: string`, `methodName: string`) -> `string`
- **MakeRequest**(`protocolName: string`, `methodName: string`, `message: Variant`, `callback: Function`, `customTelemetryData: Variant`) -> `null`
- **Publish**(`mid: string`, `params: Variant`) -> `null`
- **PublishProtocolMethodRequest**(`protocolName: string`, `methodName: string`, `message: Variant`, `customTelemetryData: Variant`) -> `null`
- **PublishProtocolMethodResponse**(`protocolName: string`, `methodName: string`, `message: Variant`, `responseCode: int`, `customTelemetryData: Variant`) -> `null`
- **SetRequestHandler**(`protocolName: string`, `methodName: string`, `callback: Function`) -> `null`
- **Subscribe**(`mid: string`, `callback: Function`, `once: bool`, `sticky: bool`) -> `Instance`
- **SubscribeToProtocolMethodRequest**(`protocolName: string`, `methodName: string`, `callback: Function`, `once: bool`, `sticky: bool`) -> `Instance`
- **SubscribeToProtocolMethodResponse**(`protocolName: string`, `methodName: string`, `callback: Function`, `once: bool`, `sticky: bool`) -> `Instance`
