---
title: NetworkSettings
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated, NotBrowsable]
---

# NetworkSettings

Settings related to networked engine behaviors.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated] [NotBrowsable]

## Description

`NetworkSettings` is a class that allows you to debug several features with
Roblox's server/client networking. It can be found in Roblox Studio's settings
under the **Network** tab.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.NetworkSettings.EmulatedTotalMemoryInMB` | `int` | [Hidden] [NotReplicated] {security: PluginSecurity} |
| `Class.NetworkSettings.FreeMemoryMBytes` | `float` | [Hidden] [ReadOnly] [NotReplicated] {security: PluginSecurity} |
| `Class.NetworkSettings.HttpProxyEnabled` | `bool` |  {write: RobloxScriptSecurity} |
| `Class.NetworkSettings.HttpProxyURL` | `string` |  {write: RobloxScriptSecurity} |
| `Class.NetworkSettings.InboundNetworkJitterMs` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.NetworkSettings.InboundNetworkLossPercent` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.NetworkSettings.InboundNetworkMinDelayMs` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.NetworkSettings.IncomingReplicationLag` | `double` |  |
| `Class.NetworkSettings.OutboundNetworkJitterMs` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.NetworkSettings.OutboundNetworkLossPercent` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.NetworkSettings.OutboundNetworkMinDelayMs` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.NetworkSettings.PrintJoinSizeBreakdown` | `bool` |  |
| `Class.NetworkSettings.PrintPhysicsErrors` | `bool` |  |
| `Class.NetworkSettings.PrintStreamInstanceQuota` | `bool` |  |
| `Class.NetworkSettings.RandomizeJoinInstanceOrder` | `bool` |  |
| `Class.NetworkSettings.RenderStreamedRegions` | `bool` |  |
| `Class.NetworkSettings.ShowActiveAnimationAsset` | `bool` |  |
