---
title: Debris
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# Debris

Allows scheduling the guaranteed destruction of an object without yielding.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

The **Debris** service allows scheduling guaranteed destruction of an object
without yielding.

#### Advantages

Besides creating a bit of a mess, objects that are no longer required can use
up system memory and cause an experience to run slower over time. For this
reason, it's always advised to call `Class.Instance:Destroy()` on objects you
no longer need. In some cases, however, an object may have a specific period
of utility before it can be destroyed.

Consider a wall being smashed into individual bricks. If you want a brick to
linger for 3 seconds before being destroyed, you can use the following code:

```lua
task.wait(3)
brick:Destroy()
```

However, waiting causes the thread to yield which may be undesired. To avoid
yielding, a callback function can be scheduled to run on a new thread after 3
seconds:

```lua
task.delay(3, function()
	brick:Destroy()
end)
```

Or in one line:

```lua
task.delay(3, brick.Destroy, brick)
```

While this now avoids yielding, it has a potential drawback in that the
scheduled callback will never run if the script is disabled or destroyed
before the callback runs.

This is where `Class.Debris` has a specific advantage, as it does not yield
the current thread and runs outside the context of the script, guaranteeing
the instance is eventually destroyed even if the script is disabled or
destroyed. The following code does not yield and guarantees the instance will
be destroyed:

```lua
Debris:AddItem(brick, 3)
```

Note that `Class.Debris` has a hardcoded maximum of 1,000 objects, so if more
than 1,000 items are added, the oldest debris will be destroyed instantly to
make room for new debris.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Debris.MaxItems` | `int` | [Deprecated] |

## Methods

### `Class.Debris:AddItem`

``AddItem(item: `Class.Instance`, lifetime: `double`)`` -> `null`

### `Class.Debris:SetLegacyMaxItems`

``SetLegacyMaxItems(enabled: `bool`)`` -> `null`
   {security: LocalUserSecurity}

### `Class.Debris:addItem`

``addItem(item: `Class.Instance`, lifetime: `double`)`` -> `null`
  [Deprecated]
