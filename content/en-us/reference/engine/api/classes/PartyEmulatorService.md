---
title: PartyEmulatorService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# PartyEmulatorService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.PartyEmulatorService:CreateNewParty`

``CreateNewParty()`` → `string`
   {security: RobloxScriptSecurity}

### `Class.PartyEmulatorService:DeleteParty`

``DeleteParty(partyId: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.PartyEmulatorService:GetEmulatedPartyAsync`

``GetEmulatedPartyAsync(partyId: `string`)`` → `Array`
  [Yields] {security: RobloxScriptSecurity}

### `Class.PartyEmulatorService:GetEmulatedPartyConfiguration`

``GetEmulatedPartyConfiguration()`` → `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.PartyEmulatorService:GetIsEmulationEnabled`

``GetIsEmulationEnabled()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.PartyEmulatorService:OnTestPlayerCountChanged`

``OnTestPlayerCountChanged(newPlayerCount: `int`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.PartyEmulatorService:SetIsEmulationEnabled`

``SetIsEmulationEnabled(isEnabled: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.PartyEmulatorService:SetPlayerPartyId`

``SetPlayerPartyId(userId: `int64`, partyId: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.PartyEmulatorService:applyPartyIdToPlayer`

``applyPartyIdToPlayer(player: `Class.Player`)`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.PartyEmulatorService.ConfigurationChanged`

Fires with: (configuration: `Dictionary`)
