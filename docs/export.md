# Export

Export scenes, assets, and metadata for consumption by video generation models.

---

## Overview

When you're ready to produce clips, Whatif exports:

- **Scenes** — Structured scene data (location, characters, dialogue, directions)
- **Assets** — Storyboard frames, character visuals, location skyboxes, audio
- **Prompts** — Generation-ready descriptions for video models

---

## Video Generation Integration

Output is designed to feed into video gen models such as:

- **Veo** — Google's video generation model
- **Runway** — Referenced in [ingestion](ingestion.md) pipeline config
- **Pika, Kling** — Other supported providers

---

## Pipeline

The [ingestion](ingestion.md) docs describe the pipeline: storyboard generation, render tracking, and director approvals. Renders are stored under `scenes/{act}/{scene_id}/renders/` with metadata in `pipeline/renders/`.

---

## Export Formats

(To be expanded: exact output format, API shape, and integration examples.)
