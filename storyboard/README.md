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

| Video | Duration (est.) | Description |
|-------|----------------|-------------|
| Prologue (`intro.mp4`) | ~2–3 min | Recaps the four characters' backgrounds and journey to the dungeon |
| Ending A (`ending_a.mp4`) | ~1–2 min | Victory ending — heroes defeat Mr. Star |
| Ending B (`ending_b.mp4`) | ~1–2 min | Defeat ending — Mr. Star wins, darkness spreads |
