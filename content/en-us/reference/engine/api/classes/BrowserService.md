---
title: BrowserService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# BrowserService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **CloseBrowserWindow**() -> `null`
- **CopyAuthCookieFromBrowserToEngine**() -> `null`
- **EmitHybridEvent**(`moduleName: string`, `eventName: string`, `params: string`) -> `null`
- **ExecuteJavaScript**(`javascript: string`) -> `null`
- **OpenBrowserWindow**(`url: string`) -> `null`
- **OpenNativeOverlay**(`title: string`, `url: string`) -> `null`
- **OpenWeChatAuthWindow**() -> `null`
- **ReturnToJavaScript**(`callbackId: string`, `success: bool`, `params: string`) -> `null`
- **SendCommand**(`command: string`) -> `null`

## Events

- **AuthCookieCopiedToEngine**()
- **BrowserWindowClosed**()
- **BrowserWindowWillNavigate**(`url: string`)
- **JavaScriptCallback**(`content: string`)
