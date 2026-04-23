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

### Prologue (~90 seconds, 6 scenes)

| # | Scene | Duration | Key Beat |
|---|-------|----------|----------|
| P-01 | World + Team | ~15s | Dungeon aerial + all 4 characters + Mr. Star in backpack |
| P-02 | Character Backstories Montage | ~15s | Cheri / Enos / Oreo intros + Mr. Star's secret hint |
| P-03 | Betrayal Morning | ~15s | Empty food bags, round belly, comedic horror |
| P-04 | Truth & Darkness | ~15s | Confrontation, dark power stirs but retreats — not yet |
| P-05 | The Dragon Awaits | ~15s | Team approaches dragon chamber, doors explode → **Game Stage 1** |
| P-06 | Dragon Falls, Darkness Rises | ~15s | Dragon defeated, Mr. Star absorbs dark power, transforms → **Game Stage 2** |

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
