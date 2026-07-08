---
title: NegateOperation
type: class
superclass: PartOperation
---

# NegateOperation

Result of a part that has been negated for use in solid modeling.

**Inherits from:** `Class.PartOperation` > `Class.TriangleMeshPart` > `Class.BasePart` > `Class.PVInstance` > `Class.Instance` > `Class.Object`

## Description

A **NegateOperation** is the result of a part that has been negated through
Studio's solid modeling **Negate** tool.

A negated part turns pink and translucent as an indicator of its state. If the
negated part is then unioned with a normal part using the **Union** tool,
sections where the negated part overlaps the normal part will be cut out.

Note that you can undo part negation by selecting the negated part and
clicking **Negate** again.

See [Solid Modeling](../../../parts/solid-modeling.md) to learn more about
Studio's solid modeling tools and methods.
