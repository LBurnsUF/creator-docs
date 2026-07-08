---
title: MessagingService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# MessagingService

Allows servers of the same experience to communicate with each other.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

**MessagingService** allows servers of the same experience to communicate with
each other in real time, typically within 1-2 seconds, using topics. Topics
are developer‑defined strings (1–80 characters) that servers use to send and
receive messages.

Delivery is best effort and not guaranteed. Make sure to architect your
experience so delivery failures are not critical.

[Cross-Server Messaging](../../../cloud-services/cross-server-messaging.md)
explores how to communicate between servers in greater detail.

If you want to publish ad-hoc messages to live game servers, or publish across
experiences, you can use the
[Open Cloud APIs](../../../cloud/guides/usage-messaging.md).

#### Limitations

Note that these limits are subject to change.

<table>
	<thead>
		<tr>
			<th>Limit</th>
			<th>Maximum</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>
				<b>Size of message</b>
			</td>
			<td>
				1kB
			</td>
		</tr>
		<tr>
			<td>
				<b>Messages sent per game server</b>
			</td>
			<td>
				 600 + 240 * (number of players in this game server) per minute
			</td>
		</tr>
		<tr>
			<td>
				<b>Messages received per topic</b>
			</td>
			<td>
				(40 + 80 * number of servers) per minute
			</td>
		</tr>
		<tr>
			<td>
				<b>Messages received for entire game</b>
			</td>
			<td>
				 (400 + 200 * number of servers) per minute
			</td>
		</tr>
    <tr>
			<td>
				<b>Subscriptions allowed per game server</b>
			</td>
			<td>
				 20 + 8 * (number of players in this game server)
			</td>
		</tr>
    <tr>
			<td>
				<b>Subscribe requests per game server</b>
			</td>
			<td>
				 240 requests per minute
			</td>
		</tr>
	</tbody>
</table>

## Methods

### `Class.MessagingService:PublishAsync`

``PublishAsync(topic: `string`, message: `Variant`)`` -> `null`
  [Yields]

### `Class.MessagingService:SubscribeAsync`

``SubscribeAsync(topic: `string`, callback: `Datatype.Function`)`` -> `Datatype.RBXScriptConnection`
  [Yields]
