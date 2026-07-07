---
title: PlayerEmulatorService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# PlayerEmulatorService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Properties

- **CustomPoliciesEnabled**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **EmulatedCountryCode**: `string` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **EmulatedGameLocale**: `string` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **PlayerEmulationEnabled**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **PseudolocalizationEnabled**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **SerializedEmulatedPolicyInfo**: `BinaryString` [Hidden] [NotReplicated] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **TextElongationFactor**: `int` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **GetEmulatedPolicyInfo**() -> `Dictionary`
- **RegionCodeWillHaveAutomaticNonCustomPolicies**(`regionCode: string`) -> `bool`
- **SetEmulatedPolicyInfo**(`emulatedPolicyInfo: Dictionary`) -> `null`
