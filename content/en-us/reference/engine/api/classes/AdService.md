---
title: AdService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# AdService

The service responsible for in-experience advertising.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

`Class.AdService` is responsible for in-experience advertising. This includes
[rewarded video](../../../production/promotion/rewarded-video-ads.md) and
[ad integrations](../../../production/promotion/ad-integrations.md).

## Methods

### `Class.AdService:CreateAdRewardFromDevProductId`

``CreateAdRewardFromDevProductId(devProductId: `int64`)`` -> `Datatype.AdReward`

### `Class.AdService:GetAdAvailabilityNowAsync`

``GetAdAvailabilityNowAsync(adFormat: `Enum.AdFormat`)`` -> `Dictionary`
  [Yields]

### `Class.AdService:GetAdAvailabilityNowForUniverseAsync`

``GetAdAvailabilityNowForUniverseAsync(adFormat: `Enum.AdFormat`, universeId: `int64`, isUniversalAppDM: `bool`)`` -> `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AdService:GetAdTeleportInfo`

``GetAdTeleportInfo()`` -> `Tuple`
   {security: RobloxScriptSecurity}

### `Class.AdService:GetCampaignEligibilityAsync`

``GetCampaignEligibilityAsync(campaignId: `string`, player: `Class.Player`)`` -> `Dictionary`
  [Yields]

### `Class.AdService:GetReportAdInfo`

``GetReportAdInfo()`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.AdService:GetUniversalAppAdsEligibility`

``GetUniversalAppAdsEligibility()`` -> `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.AdService:HandleWhyThisAdClicked`

``HandleWhyThisAdClicked(advertiserName: `string`, payerName: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AdService:HideEudsaDisclosure`

``HideEudsaDisclosure()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AdService:OnDemandVideoCompleteFromUI`

``OnDemandVideoCompleteFromUI(result: `Enum.ShowAdResult`, encryptedAdTrackingData: `string`, encryptionMetadata: `string`, rewardDetails: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AdService:RegisterAdOpportunityAsync`

``RegisterAdOpportunityAsync(instance: `Class.Instance`, placementId: `int64?`)`` -> `null`
  [Yields]

### `Class.AdService:RegisterDisclosureButton`

``RegisterDisclosureButton(disclosureButton: `Class.GuiButton`, adIntegrationPlacementId: `string`)`` -> `null`

### `Class.AdService:ReturnToPublisherExperience`

``ReturnToPublisherExperience(adTeleportMethod: `Enum.AdTeleportMethod`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AdService:SetAdGuiInteractivityHandlerInitialized`

``SetAdGuiInteractivityHandlerInitialized()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AdService:ShowRewardedVideoAdAsync`

``ShowRewardedVideoAdAsync(player: `Class.Player`, reward: `Datatype.AdReward`, placementId: `int64?`)`` -> `Enum.ShowAdResult`
  [Yields]

### `Class.AdService:ShowRewardedVideoAdAtClientAsync`

``ShowRewardedVideoAdAtClientAsync(universeId: `int64`)`` -> `Enum.ShowAdResult`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AdService:ShowVideoAd`

``ShowVideoAd()`` -> `null`
  [Deprecated]

### `Class.AdService:SubmitAdNotification`

``SubmitAdNotification(universeId: `int64`, isShowAdSuccessful: `bool`, earnedReward: `bool`, rewardProductName: `string`, rewardProductImageAssetId: `int64`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AdService:UnregisterAdOpportunity`

``UnregisterAdOpportunity(instance: `Class.Instance`)`` -> `null`

## Events

### `Class.AdService.AdTeleportEnded`

Fires with: ()

### `Class.AdService.AdTeleportInitiated`

Fires with: ()

### `Class.AdService.RewardedVideoAdEnded`

Fires with: ()

### `Class.AdService.RewardedVideoAdStarted`

Fires with: ()

### `Class.AdService.ShowDynamicEudsaDisclosure`

Fires with: (advertiserName: `string`, payerName: `string`)

### `Class.AdService.ShowReportAdPopup`

Fires with: (adInfo: `Dictionary`)

### `Class.AdService.VideoAdClosed`

Fires with: (adShown: `bool`)
  [Deprecated]

### `Class.AdService.adGuiRegisterUI`

Fires with: (adGui: `Class.Instance`)

## Callbacks

### `Class.AdService.OnImmersiveBrandedAdDisclosureButtonActivated`

``OnImmersiveBrandedAdDisclosureButtonActivated(data: `Dictionary`)`` -> `null`
  [NoYield]

### `Class.AdService.onDemandVideoPlayInUI`

``onDemandVideoPlayInUI(data: `Dictionary`)`` -> `Class.VideoFrame`
