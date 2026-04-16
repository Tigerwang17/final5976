# Our Rations are All Stolen, So Why on Earth are We Still Adventuring in This Dungeon?

SDSC5976 Final Project

---

## Overview

An interactive narrative experience combining AI-generated short films and a browser game.

The experience flows as:

1. **Prologue (AI short film):** Recaps the four characters' backgrounds and introduces the dungeon world
2. **Boss Battle (mini-game):** Two players cooperate to fight the final Boss
3. **Ending (AI short film):** Win → Ending A; Lose → Ending B

---

## How to Run

Open `index.html` in a browser. No installation or dependencies required.

> The game alone (without videos) can be run from `game/index.html`.

---

## Characters

| Character | Race | Class | Goal |
|-----------|------|-------|------|
| Mr.Star | Magical creature (dog-bear hybrid) | Cute pet / Mysterious Boss | Reclaim dark power and turn the world into food |
| Cheri | Elf | Monk / Mage | Discover her true self and escape the temple she grew up in |
| Enos | Half-elf | Mage | Gather material for his thesis inside the dungeon |
| Oreo | Cat-folk | Ninja Assassin | Find the legendary medicine that can cure her grandfather |

Character data: [polyu-storyworld](https://github.com/venetanji/polyu-storyworld/tree/main/characters)

---

## Project Structure

```
/
├── index.html            # Integration page: prologue video → game → ending video
├── README.md
├── story_outline.png     # Story overview diagram
│
├── game/                 # Boss battle mini-game (zero-dependency, single HTML file)
│   ├── index.html
│   ├── character/        # Character sprites (PNG)
│   └── stages/           # Background and result screens
│
├── videos/               # AI-generated short films
│   ├── intro.mp4         # Prologue (add file here)
│   ├── ending_a.mp4      # Ending A — Victory (add file here)
│   ├── ending_b.mp4      # Ending B — Defeat (add file here)
│   └── README.md         # Video links and production notes
│
├── storyboard/           # Written storyboard and key frames
│   ├── text/             # Scene-by-scene storyboard scripts
│   │   ├── prologue.md
│   │   ├── ending_a.md
│   │   └── ending_b.md
│   └── frames/           # First and last frame images for each generated clip
│       ├── prologue/
│       ├── ending_a/
│       └── ending_b/
│
├── character_pics/       # Character reference images
│   └── Mr.Star/
│
├── workflow/             # Each member's AI production process
│   ├── Mr.Star/          # prompts.md, reflection.md, README.md
│   ├── cheri/
│   ├── enos/
│   └── oreo/
│
└── presentation/         # PPT slides and presentation materials
    └── README.md
```

---

## Team Responsibilities

| Member | Character | Tasks |
|--------|-----------|-------|
| （填写） | Mr.Star | Prologue short film · Mr.Star segment · Workflow docs |
| （填写） | Cheri | Cheri segment · Ending A short film · Workflow docs |
| （填写） | Enos | Enos segment · Ending B short film · Workflow docs |
| （填写） | Oreo | Game code · HTML integration · Win/lose logic · Workflow docs |

---

## AI Tools Used

| Tool | Purpose |
|------|---------|
| Kling AI (可灵) | AI video generation for all short films |
| Claude Code | Game development and HTML integration assistance |

---

## Assessment Criteria

| Criterion | How We Address It |
|-----------|------------------|
| Value/Novelty (25%) | Original game code + AI narrative films; uses polyu-storyworld characters |
| GitHub repo — code works (50%) | `index.html` + `game/index.html` both run in browser |
| GitHub repo — workflow documented (50%) | `workflow/` folder: prompts + reflections for all 4 members |
| Uses polyu-storyworld / MCP (50%) | Characters sourced from [venetanji/polyu-storyworld](https://github.com/venetanji/polyu-storyworld) |
| All members contributed (50%) | Each member has their own workflow folder with documented process |
| Reflection (25%) | `workflow/*/reflection.md` — AI impact on pipeline and output |

---

## Links

- Character database: [polyu-storyworld](https://github.com/venetanji/polyu-storyworld/tree/main/characters)
- Videos (external): （填写 Google Drive 或其他链接）
