---
title: RecommendationService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# RecommendationService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **GenerateItemListAsync**(`generateRecommendationItemListRequest: Dictionary`) -> `RecommendationPages` [Yields]
- **GetRecommendationItemAsync**(`itemId: string`) -> `Dictionary` [Yields]
- **LogActionEvent**(`actionType: RecommendationActionType`, `itemId: string`, `tracingId: string`, `actionEventDetails: Dictionary = nil`) -> `null`
- **LogImpressionEvent**(`impressionType: RecommendationImpressionType`, `itemId: string`, `tracingId: string`, `impressionEventDetails: Dictionary = nil`) -> `null`
- **LogPreferenceEvent**(`preferenceType: RecommendationPreferenceType`, `targetType: RecommendationPreferenceTargetType`, `targetId: string`, `tracingId: string = `, `itemId: string = `) -> `null`
- **RegisterItemAsync**(`player: Player`, `registerRecommendationItemsRequest: Dictionary`) -> `Dictionary` [Yields]
- **RemoveItemAsync**(`itemId: string`) -> `null` [Yields]
- **UpdateItemAsync**(`updateRecommendationItemRequest: Dictionary`) -> `null` [Yields]
