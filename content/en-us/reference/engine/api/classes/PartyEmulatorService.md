---
title: PartyEmulatorService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# PartyEmulatorService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **CreateNewParty**() -> `string`
- **DeleteParty**(`partyId: string`) -> `null`
- **GetEmulatedPartyAsync**(`partyId: string`) -> `Array` [Yields]
- **GetEmulatedPartyConfiguration**() -> `Dictionary`
- **GetIsEmulationEnabled**() -> `bool`
- **OnTestPlayerCountChanged**(`newPlayerCount: int`) -> `null`
- **SetIsEmulationEnabled**(`isEnabled: bool`) -> `null`
- **SetPlayerPartyId**(`userId: int64`, `partyId: string`) -> `null`
- **applyPartyIdToPlayer**(`player: Player`) -> `null`

## Events

- **ConfigurationChanged**(`configuration: Dictionary`)
