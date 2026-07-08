---
title: RenderFidelity
type: enum
---

# `Enum.RenderFidelity`

Determines the level of detail that solid modeled and mesh parts will be shown
in.

This enum determines the level of detail that
[meshes](../../../parts/meshes.md) and
[solid modeled](../../../parts/solid-modeling.md) parts will be shown in. The
default is **Automatic**, meaning the object's detail is based on its distance
from the camera as outlined in the following table.

<table>
    <thead>
        <tr>
            <th>Distance From Camera</th>
            <th>Render Fidelity</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Less than 250 studs</td>
            <td>Highest</td>
        </tr>
        <tr>
            <td>250 to 500 studs</td>
            <td>Medium</td>
        </tr>
        <tr>
            <td>500 or more studs</td>
            <td>Lowest</td>
        </tr>
    </tbody>
</table>

The `Enum.RenderFidelity` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.RenderFidelity.Automatic` | 0 | Object's level of detail is dynamically controlled by its distance from the camera (see table above) |
| `Enum.RenderFidelity.Precise` | 1 | Object is rendered in the highest fidelity regardless of its distance from the camera. |
| `Enum.RenderFidelity.Performance` | 2 | Push performance as much as possible, trying to maintain quality if possible, and discarding appeara |
