---
title: StartPageService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# StartPageService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.StartPageService:generateTempUrlInContentProvider`

``generateTempUrlInContentProvider(url: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.StartPageService:getDaysSinceFirstUserLogin`

``getDaysSinceFirstUserLogin()`` -> `int`
   {security: RobloxScriptSecurity}

### `Class.StartPageService:getLocalGamesFromRegistry`

``getLocalGamesFromRegistry()`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.StartPageService:getRecentAPIGamesFromRegistry`

``getRecentAPIGamesFromRegistry()`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.StartPageService:getTempUrlInContentProvider`

``getTempUrlInContentProvider(url: `string`)`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.StartPageService:isTutorialBannerClosed`

``isTutorialBannerClosed()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.StartPageService:isTutorialPopupClosed`

``isTutorialPopupClosed()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.StartPageService:openLink`

``openLink(link: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.StartPageService:openLocalFile`

``openLocalFile(filePath: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.StartPageService:openPlace`

``openPlace(placeId: `int64`, universeId: `int64`, launchTutorial: `bool`, shouldSkipSafetyChecks: `bool`, openAsLocalCopy: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.StartPageService:removeAPIGameFromRegistry`

``removeAPIGameFromRegistry(gameId: `int64`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.StartPageService:removeLocalFileFromRegistry`

``removeLocalFileFromRegistry(fileName: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.StartPageService:setTutorialBannerClosed`

``setTutorialBannerClosed(closed: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.StartPageService:setTutorialPopupClosed`

``setTutorialPopupClosed(closed: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.StartPageService:shouldShowMacOSDeprecationWarning`

``shouldShowMacOSDeprecationWarning()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.StartPageService:shouldShowWinOSDeprecationWarning`

``shouldShowWinOSDeprecationWarning()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.StartPageService:startTutorial`

``startTutorial()`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.StartPageService.ImageImportedSignal`

Fires with: (urlImported: `string`, temporaryId: `string`)

### `Class.StartPageService.LocalGamesFromRegistryUpdatedSignal`

Fires with: (localGames: `Array`)

### `Class.StartPageService.RecentApiGamesFromRegistryUpdatedSignal`

Fires with: (recentGames: `Array`)
