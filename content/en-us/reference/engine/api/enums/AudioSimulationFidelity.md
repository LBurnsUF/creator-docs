---
title: AudioSimulationFidelity
type: enum
---

# `Enum.AudioSimulationFidelity`

Enum which determines how detailed audio simulation should be for
`Class.AudioEmitter|AudioEmitters` and `Class.AudioListener|AudioListeners`.

This enum, used with `Class.AudioEmitter.SimulationFidelity` and
`Class.AudioListener.SimulationFidelity`, determines how detailed audio
simulation should be.

The `Enum.AudioSimulationFidelity` enum has 2 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.AudioSimulationFidelity.None` | 0 | No acoustic simulation occurs; only direction and distance are taken into account. |
| `Enum.AudioSimulationFidelity.Automatic` | 1 | The audio engine simulates transmission, diffraction, and reflections at a level of detail suitable  |
