# What-If Exploration

The core creative loop. You ask "what if..." and the world branches. State propagates; you review, approve, and commit.

---

## Overview

As director, you assert intent in natural language (e.g. "what if Marcus confronts Jane in scene 005?"). The system:

1. Creates a new decision node
2. Branches the affected YAML (characters, events, scenes)
3. Propagates knowledge, emotional states, and world state to downstream scenes
4. Reindexes SQLite
5. Optionally triggers generation (storyboards, renders)

---

## The Loop

```
IDLE → DECIDE → BRANCH → PROPAGATE → REINDEX → GENERATE
  ↑                                                      │
  └──────────── director approves/rejects ───────────────┘
```

Every cycle produces a new decision, updated YAML, a reindexed SQLite, and a git commit.

---

## Why It Matters

This is the "fun" part. After watching a film, audiences can enter that world and explore alternatives. What if the character had chosen differently? What if someone else knew the truth? Whatif makes those branches concrete and exportable.

---

## Technical Details

For the full state machine, agent read/write patterns, and decision/timeline structure, see [Ingestion — State Machine Transitions](ingestion.md#state-machine-transitions).
