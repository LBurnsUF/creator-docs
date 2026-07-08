---
title: RecommendationService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# RecommendationService

A service that provides an interface for you to manage and display
personalized content recommendations.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

`RecommendationService` provides an interface for you to manage and display
personalized content recommendations. It supports creating, retrieving,
updating, and deleting recommendation items, as well as generating lists of
recommended content for users. Additionally, it includes functionality for
logging user interactions, such as views and actions, to help refine and
improve recommendation quality. Once set up, you can monitor analytics in the
Creator Dashboard under the **Engagement** section for an experience.

## Methods

### `Class.RecommendationService:GenerateItemListAsync`

``GenerateItemListAsync(generateRecommendationItemListRequest: `Dictionary`)`` -> `Class.RecommendationPages`
  [Yields]

### `Class.RecommendationService:GetRecommendationItemAsync`

``GetRecommendationItemAsync(itemId: `string`)`` -> `Dictionary`
  [Yields]

### `Class.RecommendationService:LogActionEvent`

``LogActionEvent(actionType: `Enum.RecommendationActionType`, itemId: `string`, tracingId: `string`, actionEventDetails: `Dictionary`)`` -> `null`

### `Class.RecommendationService:LogImpressionEvent`

``LogImpressionEvent(impressionType: `Enum.RecommendationImpressionType`, itemId: `string`, tracingId: `string`, impressionEventDetails: `Dictionary`)`` -> `null`

### `Class.RecommendationService:LogPreferenceEvent`

``LogPreferenceEvent(preferenceType: `Enum.RecommendationPreferenceType`, targetType: `Enum.RecommendationPreferenceTargetType`, targetId: `string`, tracingId: `string`, itemId: `string`)`` -> `null`

### `Class.RecommendationService:RegisterItemAsync`

``RegisterItemAsync(player: `Class.Player`, registerRecommendationItemsRequest: `Dictionary`)`` -> `Dictionary`
  [Yields]

### `Class.RecommendationService:RemoveItemAsync`

``RemoveItemAsync(itemId: `string`)`` -> `null`
  [Yields]

### `Class.RecommendationService:UpdateItemAsync`

``UpdateItemAsync(updateRecommendationItemRequest: `Dictionary`)`` -> `null`
  [Yields]
