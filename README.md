# Our Rations are All Stolen, So Why on Earth are We Still Adventuring in This Dungeon?

SDSC5976 Final Project

---

## Overview

An interactive narrative experience combining film and game.

This project is the final chapter of the story — the Boss Battle. The experience flows as follows:

1. **Prologue (AI short film):** Recaps the four characters' backgrounds and adventures, and introduces the dungeon world
2. **Boss Battle (mini-game):** The player controls a character to fight the final Boss
3. **Ending (AI short film):** Win and Ending A plays; lose and Ending B plays

---

## Characters

| Character | Race | Class | Goal |
|-----------|------|-------|------|
| Mr.Star | Magical creature (dog-bear hybrid) | Cute pet / Mysterious Boss | Reclaim dark power and turn the world into food |
| Cheri | Elf | Monk / Mage | Discover her true self and escape the temple she grew up in |
| Enos | Half-elf | Mage | Gather material for his thesis inside the dungeon |
| Oreo | Cat-folk | Ninja Assassin | Find the legendary medicine that can cure the ninja grandfather who raised her |

Character data source: [polyu-storyworld](https://github.com/venetanji/polyu-storyworld/tree/main/characters)

---

## How to Run

Open `index.html` directly in a browser. No installation or dependencies required.

---

## Project Structure

```
/
├── index.html            # Main file: prologue video + game + ending video
├── game/                 # Game assets (character sprites, stage images, etc.)
├── videos/               # AI-generated short films
│   ├── intro.mp4         # Prologue
│   ├── ending_a.mp4      # Ending A (victory)
│   └── ending_b.mp4      # Ending B (defeat)
└── workflow/             # Each member's AI video production process
    ├── mrstar/
    ├── cheri/
    ├── enos/
    └── oreo/
```

---

## Team Responsibilities

| Member | Role |
|--------|------|
| Mr.Star lead | Prologue short film, Mr.Star character segment, workflow documentation |
| Cheri lead | Cheri character segment, Ending A short film, workflow documentation |
| Enos lead | Enos character segment, Ending B short film, workflow documentation |
| Oreo lead | Game code, video integration in index.html, win/lose logic, workflow documentation |

---

## AI Tools Used

- Video generation: Kling AI
- Development assistance: Claude Code

---

## Links

- Character database: [polyu-storyworld](https://github.com/venetanji/polyu-storyworld/tree/main/characters)
