---
title: DeveloperMemoryTag
type: enum
---

# `Enum.DeveloperMemoryTag`

A memory tracking category.

A list of memory categories, and a description of what they are allocated to.

The `Enum.DeveloperMemoryTag` enum has 24 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.DeveloperMemoryTag.Internal` | 0 | General data that doesn't have any categorization. This could be due to either internal reasons, or  |
| `Enum.DeveloperMemoryTag.HttpCache` | 1 | A cache of HTTP responses. |
| `Enum.DeveloperMemoryTag.Instances` | 2 | All the Instances present in memory. |
| `Enum.DeveloperMemoryTag.Signals` | 3 | Events, signals, connections, etc. |
| `Enum.DeveloperMemoryTag.LuaHeap` | 4 | All of the data in Luau, including everything happening in core scripts, built-in data types, etc. |
| `Enum.DeveloperMemoryTag.Script` | 5 | All memory being manipulated and referenced by scripts. |
| `Enum.DeveloperMemoryTag.PhysicsCollision` | 6 | Collision detection in the `Class.Workspace`. |
| `Enum.DeveloperMemoryTag.BaseParts` | 7 | 3D parts used for simulation. |
| `Enum.DeveloperMemoryTag.GraphicsSolidModels` | 8 | Rendering solid models (stuff made with Union, Negate, etc.). |
| `Enum.DeveloperMemoryTag.GraphicsMeshParts` | 10 | Rendering of mesh parts. |
| `Enum.DeveloperMemoryTag.GraphicsParticles` | 11 | Rendering of particles from ParticleEmitters. |
| `Enum.DeveloperMemoryTag.GraphicsParts` | 12 | Rendering of regular parts. |
| `Enum.DeveloperMemoryTag.GraphicsSpatialHash` | 13 | Spatial hash lookup tables of the game world that are used for rendering. |
| `Enum.DeveloperMemoryTag.GraphicsTerrain` | 14 | Rendering of terrain geometry. |
| `Enum.DeveloperMemoryTag.GraphicsTexture` | 15 | Rendering of textures in the game world. |
| `Enum.DeveloperMemoryTag.GraphicsTextureCharacter` | 16 | Rendering of texture composition maps that are generated for Humanoids. |
| `Enum.DeveloperMemoryTag.Sounds` | 17 | Data of sounds in-game. |
| `Enum.DeveloperMemoryTag.StreamingSounds` | 18 | Playback of sounds in-game. |
| `Enum.DeveloperMemoryTag.TerrainVoxels` | 19 | Occupancy/Material data of the Terrain. |
| `Enum.DeveloperMemoryTag.Gui` | 21 | Gui element data and rendering. |
| `Enum.DeveloperMemoryTag.Animation` | 22 | Playback of Animations on Humanoids and AnimationControllers. |
| `Enum.DeveloperMemoryTag.Navigation` | 23 | Pathfinding for Humanoids via the PathfindingService. |
| `Enum.DeveloperMemoryTag.GeometryCSG` | 24 |  |
| `Enum.DeveloperMemoryTag.GraphicsSlimModels` | 25 |  |
