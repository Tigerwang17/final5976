# LI Yanling (25057915g) — Work Contribution & Workflow

**Student ID:** 25057915g
**Name:** LI Yanling
**Project:** SD5976 Final Project — *Our Rations Are All Stolen, So Why on Earth Are We Still Adventuring in This Dungeon?*

---

## Contribution Overview

| Area | Task | Output |
|------|------|--------|
| Project Structure | Designed and built the entire repository file architecture | Repo folder structure, README files, `.gitignore`, storyboard/frames/text scaffold |
| Storyboard Text | Wrote all storyboard text prompts for 即梦AI + Lovart | `storyboard/text/prologue.md`, `storyboard/text/ending_a.md`, `storyboard/text/ending_b.md` |
| Story Content | Authored main narrative content, scene descriptions, and character arc logic | Story narrations embedded in all storyboard files |
| HTML Display | Contributed to `final.html` — the main project showcase webpage | `final.html` |
| PPT | Produced the opening section and story background introduction slides | PPT file (separate submission) |

---

## 1. Repository File Architecture (制作整个文件架构)

Built the complete project directory structure from scratch, including:

```
final_project_SD5976/
├── final.html                         # Main showcase webpage
├── README.md                          # Project overview
├── game/                              # Interactive boss battle game
│   ├── index.html
│   ├── character_pixel/
│   └── stages/
├── storyboard/
│   ├── text/                          # AI video text prompts (my work)
│   │   ├── prologue.md
│   │   ├── ending_a.md
│   │   └── ending_b.md
│   └── frames/                        # First/last frame images for 即梦AI + Lovart
│       ├── prologue/
│       ├── ending_a/
│       └── ending_b/
├── videos/                            # Generated video output
├── group_members_workflow/            # Per-member workflow documentation
│   └── 25057915g_LIYanling/
├── character_pics/                    # Character reference images
└── cover.JPG
```

**Decisions made:**
- Separated `storyboard/text/` (prompt writing) from `storyboard/frames/` (image files) to keep assets organized
- Created per-ending structure (prologue / ending_a / ending_b) matching the HTML interactive flow
- Set up `group_members_workflow/` with per-student-ID naming convention for clear attribution

---

## 2. Storyboard Text Prompts (分镜文字 Prompt 写作)

Wrote complete storyboard prompt documents for all three video segments. Each scene contains:

- **首帧 First Frame Prompt** — detailed image generation prompt for the starting keyframe
- **尾帧 Last Frame Prompt** — detailed image generation prompt for the ending keyframe  
- **视频运作 Motion Prompt** — camera movement, animation direction, timing for 即梦AI + Lovart
- **Story Narration** — the narrative text/dialogue for the scene

### Prologue (`storyboard/text/prologue.md`)
9 scenes × ~10s = ~90 seconds total

| # | Scene | Purpose |
|---|-------|---------|
| 01 | World Establishing Shot | Dungeon world introduction |
| 02 | Team March | Introduce all 4 characters together |
| 03 | Cheri's Flashback | Character backstory — temple escape |
| 04 | Enos's Introduction | Character backstory — thesis research |
| 05 | Oreo's Introduction | Character backstory — medicine hunt |
| 06 | Mr. Star's Secret | Foreshadowing — dark power absorption |
| 07 | Aftermath of Battle | Setup — team vulnerable, food visible |
| 08 | Betrayal! Food Gone | Inciting incident — Mr. Star eats everything |
| 09 | Dark Power Rises | Transition to boss battle — transformation begins |

### Ending A — Victory (`storyboard/text/ending_a.md`)
4 scenes × ~15s = ~60 seconds total

| # | Scene | Purpose |
|---|-------|---------|
| 01 | Dark Power Shatters | Mr. Star moves by teammate bond, expels darkness |
| 02 | Mr. Star Returns | Falls back to 42cm form, apologizes |
| 03 | Escape Together | Team runs through collapsing dungeon |
| 04 | Into the Sunlight | Epilogue — sunny meadow, adventure continues |

### Ending B — Defeat (`storyboard/text/ending_b.md`)
4 scenes × ~15s = ~60 seconds total

| # | Scene | Purpose |
|---|-------|---------|
| 01 | Heroes Fall | Team defeated one by one |
| 02 | Mr. Star Triumphant | Boss victory, cross-star eyes close-up |
| 03 | World Becomes Food | 美食星球 transformation sequence |
| 04 | Food Planet Epilogue | Lonely peak, heroes' eyes open, "to be continued" |

**Total video duration:** ~210 seconds (~3.5 minutes), plus interactive game

---

## 3. Story Text Content (故事文本主要内容)

Authored the core narrative logic and scene-by-scene story flow, drawing from:
- The character profiles in `7915g.yaml` (Mr. Star's full character arc)
- The worldbuilding premise (dungeon, death-revival system, monster cuisine)
- Each character's personal goal (Cheri: self-discovery / Enos: thesis / Oreo: medicine / Mr. Star: world domination via food)

**Key narrative decisions:**
- The **Ending A redemption arc** centers on Mr. Star seeing Enos shield Oreo — the act of selfless protection breaks through the dark power, because Mr. Star has no framework for valuing something over food until he witnesses this
- **Ending B** deliberately makes the food world *beautiful* rather than horrifying, to honor Mr. Star's consistent perspective — from his view it IS the ideal world; the melancholy comes from the emptiness on his face alone at the peak
- The **prologue structure** front-loads the three heroes' goals before the food-theft incident, so players understand what's at stake before the boss battle

---

## 4. HTML Display Contribution (展示的 HTML 部分贡献)

Contributed to `final.html` — the main project showcase page which:
- Displays the prologue video
- Connects to the interactive boss battle game (`game/index.html`)
- Triggers `ending_a.mp4` or `ending_b.mp4` based on game outcome
- Provides character introduction panels and project information

See `final.html` for full implementation.

---

## 5. PPT — Opening & Story Background (PPT 开场及故事背景介绍)

Responsible for the PPT sections covering:
- **Opening slides** — project title, team introduction, overall concept
- **Story background slides** — worldbuilding (underground dungeon, revival system, adventurer culture), character introductions (Cheri / Enos / Oreo / Mr. Star), the inciting food-theft incident
- Visual style: consistent with the cute anime aesthetic of the project

---

## Prompt Writing Process

See `prompts.md` for detailed 即梦AI + Lovart prompt records with generation results and rejected alternatives.

## Reflection

See `reflection.md` for personal reflection on the AI-assisted production process.
