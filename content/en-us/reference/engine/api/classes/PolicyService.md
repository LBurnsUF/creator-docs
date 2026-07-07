---
title: PolicyService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# PolicyService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.PolicyService.IsLuobuServer` | `Enum.TriStateBoolean` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.PolicyService.LuobuWhitelisted` | `Enum.TriStateBoolean` | [Hidden] {security: RobloxScriptSecurity} |

## Methods

### `Class.PolicyService:CanViewBrandProjectAsync`

``CanViewBrandProjectAsync(player: `Class.Player`, brandProjectId: `string`)`` → `bool`
  [Yields]

### `Class.PolicyService:GetPolicyInfoForPlayerAsync`

``GetPolicyInfoForPlayerAsync(player: `Class.Instance`)`` → `Dictionary`
  [Yields]

### `Class.PolicyService:GetPolicyInfoForServerRobloxOnlyAsync`

``GetPolicyInfoForServerRobloxOnlyAsync()`` → `Dictionary`
  [Yields] {security: RobloxScriptSecurity}
