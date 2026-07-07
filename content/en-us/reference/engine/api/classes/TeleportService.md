---
title: TeleportService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# TeleportService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Properties

- **CustomizedTeleportUI**: `bool` [NotReplicated] [Deprecated]

## Methods

- **Block**() -> `null`
- **GetArrivingTeleportGui**() -> `Instance`
- **GetLocalPlayerTeleportData**() -> `Variant`
- **GetPlayerPlaceInstanceAsync**(`userId: User`) -> `Tuple` [Yields]
- **GetTeleportSetting**(`setting: string`) -> `Variant`
- **GetThirdPartyTeleportInfo**(`goForth: bool`) -> `Tuple`
- **PromptExperienceDetailsAsync**(`player: Player`, `universeId: int64`) -> `PromptExperienceDetailsResult` [Yields]
- **PromptExperienceDetailsCompleted**(`resultEnum: PromptExperienceDetailsResult`, `errorMessage: string = `) -> `null`
- **ReserveServer**(`placeId: int64`) -> `Tuple` [Yields] [Deprecated]
- **ReserveServerAsync**(`placeId: int64`) -> `Tuple` [Yields]
- **SetTeleportGui**(`gui: Instance`) -> `null`
- **SetTeleportSetting**(`setting: string`, `value: Variant`) -> `null`
- **Teleport**(`placeId: int64`, `player: Instance = nil`, `teleportData: Variant`, `customLoadingScreen: Instance = nil`) -> `null`
- **TeleportAsync**(`placeId: int64`, `players: Instances`, `teleportOptions: Instance = nil`) -> `Instance` [Yields]
- **TeleportCancel**() -> `null`
- **TeleportPartyAsync**(`placeId: int64`, `players: Instances`, `teleportData: Variant`, `customLoadingScreen: Instance = nil`) -> `string` [Yields]
- **TeleportReconnect**() -> `null`
- **TeleportToPlaceInstance**(`placeId: int64`, `instanceId: string`, `player: Instance = nil`, `spawnName: string = `, `teleportData: Variant`, `customLoadingScreen: Instance = nil`) -> `null`
- **TeleportToPrivateServer**(`placeId: int64`, `reservedServerAccessCode: string`, `players: Instances`, `spawnName: string = `, `teleportData: Variant`, `customLoadingScreen: Instance = nil`) -> `null`
- **TeleportToSpawnByName**(`placeId: int64`, `spawnName: string`, `player: Instance = nil`, `teleportData: Variant`, `customLoadingScreen: Instance = nil`) -> `null`
- **TeleportTrustedBackForth**(`goForth: bool`) -> `null`
- **TeleportTrustedBackHistory**(`placeId: int64`) -> `null`
- **TeleportedPlacesBackHistory**() -> `Array`
- **TeleportedUniversesBackHistory**() -> `Array`
- **UnblockAsync**() -> `Tuple` [Yields]

## Events

- **LocalPlayerArrivedFromTeleport**(`loadingGui: Instance`, `dataTable: Variant`)
- **MenuTeleportAttempt**()
- **OpenExperienceDetailsPrompt**(`universeId: int64`)
- **ReconnectTeleportInitFailed**(`player: Instance`, `teleportResult: TeleportResult`, `errorMessage: string`, `placeId: int64`, `teleportOptions: Instance`)
- **TeleportInitFailed**(`player: Instance`, `teleportResult: TeleportResult`, `errorMessage: string`, `placeId: int64`, `teleportOptions: Instance`)
