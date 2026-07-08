---
title: PolicyService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# PolicyService

Helps you query information regarding policy compliance for players around the
world based on age range, location, and platform type.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

`PolicyService` helps you query information regarding policy compliance for
players around the world based on age range, location, and platform type.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.PolicyService.IsLuobuServer` | `Enum.TriStateBoolean` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.PolicyService.LuobuWhitelisted` | `Enum.TriStateBoolean` | [Hidden] {security: RobloxScriptSecurity} |

## Methods

### `Class.PolicyService:CanViewBrandProjectAsync`

``CanViewBrandProjectAsync(player: `Class.Player`, brandProjectId: `string`)`` -> `bool`
  [Yields]

### `Class.PolicyService:GetPolicyInfoForPlayerAsync`

``GetPolicyInfoForPlayerAsync(player: `Class.Instance`)`` -> `Dictionary`
  [Yields]

### `Class.PolicyService:GetPolicyInfoForServerRobloxOnlyAsync`

``GetPolicyInfoForServerRobloxOnlyAsync()`` -> `Dictionary`
  [Yields] {security: RobloxScriptSecurity}
