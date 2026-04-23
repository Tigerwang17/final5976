# Storyboard Frames

This folder stores the **first frame** and **last frame** of each AI-generated video clip.

## Why First + Last Frames?

Documenting the first and last frame of each clip shows:
- The visual starting point used as a reference for the AI generation
- The output state — useful for ensuring continuity when clips are edited together
- Evidence of the AI generation process for assessment purposes

## Folder Structure

```
frames/
├── prologue/          # First/last frames for each clip in prologue.mp4
├── ending_a/          # First/last frames for each clip in ending_a.mp4
└── ending_b/          # First/last frames for each clip in ending_b.mp4
```

## Naming Convention

For each clip, save two files:
- `clip_01_start.png` — first frame
- `clip_01_end.png` — last frame

Increment the clip number for each new clip: `clip_02_start.png`, `clip_02_end.png`, etc.

## How to Export Frames

**From 即梦AI + Lovart:**
- Download the generated clip as MP4
- Use any video player (e.g. QuickTime, VLC) to jump to first and last frame, then take a screenshot
- Or use ffmpeg: `ffmpeg -i clip.mp4 -vframes 1 clip_01_start.png` and `ffmpeg -sseof -0.1 -i clip.mp4 -vframes 1 clip_01_end.png`

## Status

| Folder | Status |
|--------|--------|
| `prologue/` | （待添加） |
| `ending_a/` | （待添加） |
| `ending_b/` | （待添加） |
