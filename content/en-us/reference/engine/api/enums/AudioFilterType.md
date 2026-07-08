---
title: AudioFilterType
type: enum
---

# `Enum.AudioFilterType`

Filter types used for `Class.AudioFilter` instances.

Families of curves that `Class.AudioFilter` can use to process incoming audio.
Each filter type is applied at a specified
`Class.AudioFilter.Frequency|Frequency` and may be shaped by additional
`Class.AudioFilter.Gain|Gain` or `Class.AudioFilter.Q|Q` parameters.

The `Enum.AudioFilterType` enum has 12 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.AudioFilterType.Peak` | 0 | Filter that boosts or reduces sound near a specified `Class.AudioFilter.Frequency/Frequency`. |
| `Enum.AudioFilterType.LowShelf` | 1 | Filter that boosts or reduces sound below a specified `Class.AudioFilter.Frequency/Frequency`. |
| `Enum.AudioFilterType.HighShelf` | 2 | Filter that boosts or reduces sound above a specified `Class.AudioFilter.Frequency/Frequency`. |
| `Enum.AudioFilterType.Lowpass12dB` | 3 | Filter that cuts sound above a specified `Class.AudioFilter.Frequency/Frequency`, at a slope of -12d |
| `Enum.AudioFilterType.Lowpass24dB` | 4 | Filter that cuts sound above a specified `Class.AudioFilter.Frequency/Frequency`, at a slope of -24d |
| `Enum.AudioFilterType.Lowpass48dB` | 5 | Filter that cuts sound above a specified `Class.AudioFilter.Frequency/Frequency`, at a slope of -48d |
| `Enum.AudioFilterType.Highpass12dB` | 6 | Filter that cuts sound below a specified `Class.AudioFilter.Frequency/Frequency`, at a slope of -12d |
| `Enum.AudioFilterType.Highpass24dB` | 7 | Filter that cuts sound below a specified `Class.AudioFilter.Frequency/Frequency`, at a slope of -24d |
| `Enum.AudioFilterType.Highpass48dB` | 8 | Filter that cuts sound below a specified `Class.AudioFilter.Frequency/Frequency`, at a slope of -48d |
| `Enum.AudioFilterType.Bandpass` | 9 | Filter that only allows sound near a specified `Class.AudioFilter.Frequency/Frequency` to be heard. |
| `Enum.AudioFilterType.Notch` | 10 | Filter that cuts sound near a specified `Class.AudioFilter.Frequency/Frequency`. |
| `Enum.AudioFilterType.Lowpass6dB` | 11 | Filter that cuts sound above a specified `Class.AudioFilter.Frequency/Frequency`, at a slope of -6dB |
