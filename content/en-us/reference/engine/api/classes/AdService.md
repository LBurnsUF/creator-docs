---
title: AdService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# AdService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **CreateAdRewardFromDevProductId**(`devProductId: int64`) -> `AdReward`
- **GetAdAvailabilityNowAsync**(`adFormat: AdFormat`) -> `Dictionary` [Yields]
- **GetAdAvailabilityNowForUniverseAsync**(`adFormat: AdFormat`, `universeId: int64`, `isUniversalAppDM: bool`) -> `Dictionary` [Yields]
- **GetAdTeleportInfo**() -> `Tuple`
- **GetCampaignEligibilityAsync**(`campaignId: string`, `player: Player = nil`) -> `Dictionary` [Yields]
- **GetReportAdInfo**() -> `Array`
- **GetUniversalAppAdsEligibility**() -> `Dictionary`
- **HandleWhyThisAdClicked**(`advertiserName: string`, `payerName: string`) -> `null`
- **HideEudsaDisclosure**() -> `null`
- **OnDemandVideoCompleteFromUI**(`result: ShowAdResult`, `encryptedAdTrackingData: string`, `encryptionMetadata: string`, `rewardDetails: string`) -> `null`
- **RegisterAdOpportunityAsync**(`instance: Instance`, `placementId: int64?`) -> `null` [Yields]
- **RegisterDisclosureButton**(`disclosureButton: GuiButton`, `adIntegrationPlacementId: string`) -> `null`
- **ReturnToPublisherExperience**(`adTeleportMethod: AdTeleportMethod`) -> `null`
- **SetAdGuiInteractivityHandlerInitialized**() -> `null`
- **ShowRewardedVideoAdAsync**(`player: Player`, `reward: AdReward`, `placementId: int64?`) -> `ShowAdResult` [Yields]
- **ShowRewardedVideoAdAtClientAsync**(`universeId: int64`) -> `ShowAdResult` [Yields]
- **ShowVideoAd**() -> `null` [Deprecated]
- **SubmitAdNotification**(`universeId: int64`, `isShowAdSuccessful: bool`, `earnedReward: bool`, `rewardProductName: string`, `rewardProductImageAssetId: int64`) -> `null`
- **UnregisterAdOpportunity**(`instance: Instance`) -> `null`

## Events

- **AdTeleportEnded**()
- **AdTeleportInitiated**()
- **RewardedVideoAdEnded**()
- **RewardedVideoAdStarted**()
- **ShowDynamicEudsaDisclosure**(`advertiserName: string`, `payerName: string`)
- **ShowReportAdPopup**(`adInfo: Dictionary`)
- **VideoAdClosed**(`adShown: bool`) [Deprecated]
- **adGuiRegisterUI**(`adGui: Instance`)

## Callbacks

- **OnImmersiveBrandedAdDisclosureButtonActivated**(`data: Dictionary`) -> `null` [NoYield]
- **onDemandVideoPlayInUI**(`data: Dictionary`) -> `VideoFrame`
