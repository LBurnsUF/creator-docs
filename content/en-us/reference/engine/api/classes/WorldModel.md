---
title: WorldModel
type: class
superclass: WorldRoot
---

# WorldModel

Extends limited physics for its children on to a parent `Class.ViewportFrame`.

**Inherits from:** `Class.WorldRoot` > `Class.Model` > `Class.PVInstance` > `Class.Instance` > `Class.Object`

## Description

When parented to a `Class.ViewportFrame`, `WorldModel` extends limited physics
for its children on to that `Class.ViewportFrame`. For example,
`Class.BasePart|BaseParts` that are parented to the `WorldModel` can be
animated and spatially queried (for example by raycasts) but those parts are
**not** simulated. Furthermore, you can put `Class.Humanoid` characters in the
`WorldModel` and their joints will be set up correctly for animation.

To avoid possible performance issues, make sure to only create `WorldModels`
when you want to show them and to delete `WorldModels` that are currently not
in use.
