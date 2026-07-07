---
title: StartPageService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# StartPageService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **generateTempUrlInContentProvider**(`url: string`) -> `null`
- **getDaysSinceFirstUserLogin**() -> `int`
- **getLocalGamesFromRegistry**() -> `Array`
- **getRecentAPIGamesFromRegistry**() -> `Array`
- **getTempUrlInContentProvider**(`url: string`) -> `string`
- **isTutorialBannerClosed**() -> `bool`
- **isTutorialPopupClosed**() -> `bool`
- **openLink**(`link: string`) -> `null`
- **openLocalFile**(`filePath: string`) -> `null`
- **openPlace**(`placeId: int64`, `universeId: int64`, `launchTutorial: bool`, `shouldSkipSafetyChecks: bool = false`, `openAsLocalCopy: bool = false`) -> `null`
- **removeAPIGameFromRegistry**(`gameId: int64`) -> `null`
- **removeLocalFileFromRegistry**(`fileName: string`) -> `null`
- **setTutorialBannerClosed**(`closed: bool`) -> `null`
- **setTutorialPopupClosed**(`closed: bool`) -> `null`
- **shouldShowMacOSDeprecationWarning**() -> `bool`
- **shouldShowWinOSDeprecationWarning**() -> `bool`
- **startTutorial**() -> `null`

## Events

- **ImageImportedSignal**(`urlImported: string`, `temporaryId: string`)
- **LocalGamesFromRegistryUpdatedSignal**(`localGames: Array`)
- **RecentApiGamesFromRegistryUpdatedSignal**(`recentGames: Array`)
