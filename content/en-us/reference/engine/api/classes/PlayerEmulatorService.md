---
title: PlayerEmulatorService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# PlayerEmulatorService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.PlayerEmulatorService.CustomPoliciesEnabled` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.PlayerEmulatorService.EmulatedCountryCode` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.PlayerEmulatorService.EmulatedGameLocale` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.PlayerEmulatorService.PlayerEmulationEnabled` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.PlayerEmulatorService.PseudolocalizationEnabled` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.PlayerEmulatorService.SerializedEmulatedPolicyInfo` | `Datatype.BinaryString` | [Hidden] [NotReplicated] {security: RobloxSecurity} |
| `Class.PlayerEmulatorService.TextElongationFactor` | `int` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |

## Methods

### `Class.PlayerEmulatorService:GetEmulatedPolicyInfo`

``GetEmulatedPolicyInfo()`` → `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.PlayerEmulatorService:RegionCodeWillHaveAutomaticNonCustomPolicies`

``RegionCodeWillHaveAutomaticNonCustomPolicies(regionCode: `string`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.PlayerEmulatorService:SetEmulatedPolicyInfo`

``SetEmulatedPolicyInfo(emulatedPolicyInfo: `Dictionary`)`` → `null`
   {security: RobloxScriptSecurity}
