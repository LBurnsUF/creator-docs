---
title: BrowserService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# BrowserService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.BrowserService:CloseBrowserWindow`

``CloseBrowserWindow()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.BrowserService:CopyAuthCookieFromBrowserToEngine`

``CopyAuthCookieFromBrowserToEngine()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.BrowserService:EmitHybridEvent`

``EmitHybridEvent(moduleName: `string`, eventName: `string`, params: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.BrowserService:ExecuteJavaScript`

``ExecuteJavaScript(javascript: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.BrowserService:OpenBrowserWindow`

``OpenBrowserWindow(url: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.BrowserService:OpenNativeOverlay`

``OpenNativeOverlay(title: `string`, url: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.BrowserService:OpenWeChatAuthWindow`

``OpenWeChatAuthWindow()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.BrowserService:ReturnToJavaScript`

``ReturnToJavaScript(callbackId: `string`, success: `bool`, params: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.BrowserService:SendCommand`

``SendCommand(command: `string`)`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.BrowserService.AuthCookieCopiedToEngine`

Fires with: ()

### `Class.BrowserService.BrowserWindowClosed`

Fires with: ()

### `Class.BrowserService.BrowserWindowWillNavigate`

Fires with: (url: `string`)

### `Class.BrowserService.JavaScriptCallback`

Fires with: (content: `string`)
