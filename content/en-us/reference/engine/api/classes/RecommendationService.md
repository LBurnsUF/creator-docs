---
title: RecommendationService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# RecommendationService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Methods

### `Class.RecommendationService:GenerateItemListAsync`

``GenerateItemListAsync(generateRecommendationItemListRequest: `Dictionary`)`` → `Class.RecommendationPages`
  [Yields]

### `Class.RecommendationService:GetRecommendationItemAsync`

``GetRecommendationItemAsync(itemId: `string`)`` → `Dictionary`
  [Yields]

### `Class.RecommendationService:LogActionEvent`

``LogActionEvent(actionType: `Enum.RecommendationActionType`, itemId: `string`, tracingId: `string`, actionEventDetails: `Dictionary`)`` → `null`

### `Class.RecommendationService:LogImpressionEvent`

``LogImpressionEvent(impressionType: `Enum.RecommendationImpressionType`, itemId: `string`, tracingId: `string`, impressionEventDetails: `Dictionary`)`` → `null`

### `Class.RecommendationService:LogPreferenceEvent`

``LogPreferenceEvent(preferenceType: `Enum.RecommendationPreferenceType`, targetType: `Enum.RecommendationPreferenceTargetType`, targetId: `string`, tracingId: `string`, itemId: `string`)`` → `null`

### `Class.RecommendationService:RegisterItemAsync`

``RegisterItemAsync(player: `Class.Player`, registerRecommendationItemsRequest: `Dictionary`)`` → `Dictionary`
  [Yields]

### `Class.RecommendationService:RemoveItemAsync`

``RemoveItemAsync(itemId: `string`)`` → `null`
  [Yields]

### `Class.RecommendationService:UpdateItemAsync`

``UpdateItemAsync(updateRecommendationItemRequest: `Dictionary`)`` → `null`
  [Yields]
