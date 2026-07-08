---
title: GeneratedFolder
type: class
superclass: Folder
---

# GeneratedFolder

A container that stores `Class.ProceduralModel` generation results.

**Inherits from:** `Class.Folder` > `Class.Instance` > `Class.Object`

## Description

`GeneratedFolder` is a container used to represent non-source-of-truth data in
the `Class.DataModel`. These are branches that are deterministically generated
from other parts of the `Class.DataModel` instead of containing
source-of-truth data.

`GeneratedFolder` is primarily used by `Class.ProceduralModel` to store
generation results. It can also be used by plugins or other tools to organize
generated content.

## Methods

### `Class.GeneratedFolder:SetPrimaryPart`

``SetPrimaryPart(part: `Class.BasePart`)`` -> `null`
