# Enter Interactive World

After [ingestion](ingestion.md), your project is live. This phase is about entering a scene and exploring it interactively.

---

## Overview

You select a scene at a specific point in the storyline. The system loads the world state at that moment: which characters are present, what they know, where they are, and how the scene is staged.

---

## What You Can Do

| Action | Description |
|--------|-------------|
| **Pick a scene** | Navigate to a scene by act and scene ID (e.g. `act2/scene_005`). |
| **Set the time** | The scene is evaluated at a specific event or timestamp. Characters' knowledge and emotional states reflect that moment. |
| **View characters** | Characters present in the scene appear in the 3D viewer. |
| **Adjust camera** | Change the 3D viewer camera angle, zoom, and target. Save to `camera.yaml`. |
| **Move characters** | Drag characters in the 3D viewer to reposition them. Save to `blocking.yaml`. |
| **Impersonate** | Step into a character's perspective—see what they know, don't know, and believe. Useful for dialogue and improvisation. |

---

## Configuration

See [Scene Configuration](scene-config.md) for details on:

- `camera.yaml` — camera angles, shot list, viewer settings
- `blocking.yaml` — character positions and movements
- `lighting.yaml` — key, fill, ambient

---

## Flow

```
Select scene → Load world state at time T → 3D viewer (camera, blocking, lighting)
                                            → Optional: impersonate character
```
