---
# Storyboard

This folder contains the written storyboard and key frames for all AI-generated videos in the project.

## Folder Structure

```
storyboard/
├── text/          # Written storyboard — scene-by-scene descriptions used as AI prompts
│   ├── prologue.md
│   ├── ending_a.md
│   └── ending_b.md
└── frames/        # First and last frame images for each generated clip
    ├── prologue/
    ├── ending_a/
    └── ending_b/
```

## How to Use

- **text/** — Write the dialogue, narration, and visual direction for each scene before generating videos. This serves as documentation of creative intent.
- **frames/** — After generating each video clip, export and save the first frame and last frame as images (PNG/JPG). Name them `clip_01_start.png`, `clip_01_end.png`, etc.

## Videos Overview

| Video | Duration (est.) | Clips | Description |
|-------|----------------|-------|-------------|
| Prologue (`prologue.mp4`) | ~90s | 9 clips × ~10s | Introduces the four characters, the dungeon world, the food-theft betrayal, and Mr. Star's dark transformation — leads into the interactive boss battle |
| Ending A (`ending_a.mp4`) | ~60s | 4 clips × ~15s | Victory ending — Mr. Star is moved by his teammates' bond, expels the dark power, returns to tiny form, team escapes to sunlight |
| Ending B (`ending_b.mp4`) | ~60s | 4 clips × ~15s | Defeat ending — Mr. Star wins, transforms the world into a "美食星球" food planet, bittersweet close with a hint of hope |
| **Total** | **~210s (~3.5 min)** | **17 clips** | Plus interactive game in `game/index.html` |

---

## Storyboard Summary — Scene by Scene

### Prologue (~90 seconds, 9 scenes)

| # | Scene | Duration | Key Beat |
|---|-------|----------|----------|
| P-01 | World Establishing Shot | ~10s | Dungeon aerial → interior corridor, world-building |
| P-02 | Team March | ~10s | All 4 characters + Mr. Star peeking from backpack |
| P-03 | Cheri's Flashback | ~10s | Temple life → walks out the gate alone |
| P-04 | Enos's Introduction | ~10s | Specimen jars, thesis research excitement |
| P-05 | Oreo's Introduction | ~10s | Shadow hunt, glowing medicine, memory of grandpa |
| P-06 | Mr. Star's Secret | ~10s | "Sleeping" but absorbing dark power, star birthmark glows |
| P-07 | Aftermath of Battle | ~10s | Team exhausted and asleep, food bags visible in foreground |
| P-08 | Betrayal! Food Gone! | ~10s | Empty bags, Mr. Star with round belly and crumbs on face |
| P-09 | Dark Power Rises | ~10s | Confrontation → Mr. Star begins transforming → leads to game |

### Ending A — Victory (~60 seconds, 4 scenes)

| # | Scene | Duration | Key Beat |
|---|-------|----------|----------|
| A-01 | Dark Power Shatters | ~15s | Moved by teammates' selfless bond, Mr. Star expels the darkness |
| A-02 | Mr. Star Returns | ~15s | Falls back to 42cm form, Enos catches him, he says "I'm sorry" |
| A-03 | Escape Together | ~15s | Team sprints through collapsing dungeon to the exit |
| A-04 | Into the Sunlight | ~15s | Burst into sunny meadow, picnic epilogue, Mr. Star demands more food |

### Ending B — Defeat (~60 seconds, 4 scenes)

| # | Scene | Duration | Key Beat |
|---|-------|----------|----------|
| B-01 | Heroes Fall | ~15s | Three characters collapse one by one in slow motion |
| B-02 | Mr. Star Triumphant | ~15s | Boss victory pose, cross-star eyes close-up, a tear of dark joy |
| B-03 | World Becomes Food | ~15s | Transformation wave — mountains become cakes, rivers become chocolate |
| B-04 | Food Planet Epilogue | ~15s | Mr. Star alone on cake mountain, heroes' eyes open in darkness, "TO BE CONTINUED...?" |

---

## Prompt Format in `text/`

Each scene in the text files contains four elements:

- **首帧 / First Frame Prompt** — Image generation prompt for the starting keyframe (EN + 中文)
- **尾帧 / Last Frame Prompt** — Image generation prompt for the ending keyframe (EN + 中文)
- **视频运作 / Motion Prompt** — Camera movement and animation direction for 即梦AI + Lovart (EN + 中文)
- **Story Narration / 故事旁白** — Narrative text or dialogue for the scene
