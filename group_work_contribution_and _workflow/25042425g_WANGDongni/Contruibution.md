# Oreo — Workflow

**Responsible member:** Wang Dongni
**Character:** Oreo (Cat-folk Ninja Assassin)
**Tasks:** Game code · Music Generation · Video integration in final.html · Win/lose logic · Workflow documentation

---

## Deliverables

- [x] Game code: `game/index.html` (two-player co-op boss battle)
- [x] Root integration page: `final.html` (prologue → game → endings)
- [x] Music Generation:
- [ ] Oreo character segment (part of `videos/prologue.mp4`)
- [ ] Prompts documented: `group_work_contribution_and _workflow/WANGDongni/prompts.md`
- [ ] Reflection written: `group_work_contribution_and _workflow/WANGDongni/reflection.md`

---

## Character Reference
`https://github.com/Tigerwang17/final5976/tree/main/character_pics/oreo`
- **Race:** Cat-folk
- **Class:** Ninja Assassin
- **Goal:** Find the legendary medicine to cure her grandfather

---

## Game Development Notes

The game (`game/index.html`) is a zero-dependency, single-file browser game built with HTML5 Canvas.

**Key features implemented:**
- Two-player local co-op (Player 1: WASD+Space, Player 2: 90+=)
- Character select screen for both players
- Stage 1 boss: Dragon (恶龙) — team fights together
- Stage 2 boss: Mr. Star in complete dark form — Mr. Star locked as unselectable (he is the enemy)
- Win/lose overlays with result screens
- Happy Ending screen after Stage 2 clear

**Integration (`final.html`):**
- Prologue video → Stage 1 Dragon game → cutscene → Stage 2 Mr. Star game → Ending video
- Ending A plays on Stage 2 victory; Ending B plays on Stage 2 defeat
- Navigation bar for all sections

---

## Game Production Process

### Step 1 — Game Design 
I first broke the gameplay into clear modules: player controls, boss behavior, collision rules, win/lose states, and stage transitions.  
Then I mapped the full experience flow: character select -> Stage 1 -> transition scene -> Stage 2 -> ending branches.

### Step 2 — Prompt Writing
For each implementation task, I wrote requirement prompts that described:
- target behavior (what should happen),
- interaction details (keys, UI text, transitions),
- expected outputs (code changes and assets wiring),
- constraints (single-file canvas game, existing folder structure).

### Step 3 — Vibe Coding
Using Cursor, I iterated quickly through implementation, debugging, and refinement.  
Most game logic updates (boss replacement, hit effects, stage flow, result routing, BGM/SFX triggering, and GitHub synchronization) were completed through prompt-driven coding iterations.

### Step 4 — Music Generation

The battle/result music pipeline was produced with **ComfyUI ACE-Step 1.5**.  
Generated outputs were integrated into `game/music/` and connected to stage/state-based playback logic in `game/index.html`.

### Step 5 — Images Generation

For visual assets (video key frames + game materials), I tested three AI tool types:

- **Platform tools (Lovart)**  
  - Strengths: **High-quality**, **User-friendly**  
  - Weakness: **Costly**

- **ComfyUI workflow**  
  - Strengths: **Controllable**, **Co-Built**  
  - Weakness: **Hardware-demanding**

- **Agent Bot**  
  - Strengths: **Autonomous**, **Remotely operable**  
  - Weakness: **Lower controllability**

In practice, I combined them by using platform tools for fast polished output, ComfyUI for controllable workflow-based generation, and Agent Bot for autonomous remote task execution.
