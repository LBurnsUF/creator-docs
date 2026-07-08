---
title: AudioChannelLayout
type: enum
---

# `Enum.AudioChannelLayout`

Describes the channel layout of an audio stream.

The `AudioChannelLayout` enum describes the channel layout of an audio stream.
Audio streams contain one or more channels that are intended to be rendered
simultaneously with a particular arrangement of speakers. In general, more
channels impact performance but provide higher spatial quality.

The `Enum.AudioChannelLayout` enum has 7 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.AudioChannelLayout.Mono` | 0 | Monaural audio streams contain only one **Center** channel.  <img src="/assets/engine-api/enums/Audi |
| `Enum.AudioChannelLayout.Stereo` | 1 | Stereophonic audio streams consist of two channels: **Left** and **Right**.  <img src="/assets/engin |
| `Enum.AudioChannelLayout.Quad` | 2 | Quadrophonic audio streams consist of four channels: **Left**, **Right**, **BackLeft**, and **BackRi |
| `Enum.AudioChannelLayout.Surround_5` | 3 | Surround sound audio streams consist of five channels: **Left**, **Right**, **Center**, **BackLeft** |
| `Enum.AudioChannelLayout.Surround_5_1` | 4 | 5.1 surround sound consists of six channels: **Left**, **Right**, **Center**, **BackLeft**, **BackRi |
| `Enum.AudioChannelLayout.Surround_7_1` | 5 | 7.1 surround sound consists of eight channels: **Left**, **Right**, **Center**, **SurroundLeft**, ** |
| `Enum.AudioChannelLayout.Surround_7_1_4` | 6 | 7.1.4 surround sound consists of twelve channels: **Left**, **Right**, **Center**, **SurroundLeft**, |
