---
title: Hint
type: class
superclass: Message
tags: [Deprecated]
---

# Hint

A Hint is an object that creates a small black bar at the very top of the
screen with text.

**Inherits from:** `Class.Message` > `Class.Instance` > `Class.Object`

**Tags:** [Deprecated]

## Description

A Hint is an object that creates a small black bar at the very top of the
screen with text. Its appearance cannot be customized in any way.

Notes:

- When a Hint is placed in the `Class.Workspace`, it will be visible to
  everyone
- When placed under a player's `Class.PlayerGui`, it will be visible only to
  that player
- Hints will render if placed in the `Class.CoreGui`

> **Deprecated:** With the introduction of Roblox's GUI features hints have been deprecated and
`Class.TextLabel|TextLabels` should be used instead for new work. The
`Class.TextLabel` object offers a wide range of features for displaying and
customizing text that hints do not.
