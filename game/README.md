# Pixel Co-op Shooter (Dungeon Game)

A zero-dependency, browser-only two-player local co-op mini game. Open `index.html` to play—character select with stats and skills, two boss stages with phases, result screens, and a Happy Ending.

## Features

- **Single file**: HTML, CSS, and JavaScript live in `index.html`
- **Same-screen co-op**: Player 1 and Player 2 move, shoot, and use skills independently
- **Character select**: Pick characters for each player before starting, view stats (HP, DMG) and skill descriptions
- **Two stages**: Beat stage 1 (Dragon Boss) to unlock stage 2 (Mr. Star Boss), each with unique behaviors and phases
- **HUD**: Boss HP bar, player names, lives (hearts), skill uses, and shield indicators
- **Skills**: Each character has unique skills with limited uses (e.g., shield, heal, big shot)
- **Boss Mechanics**: Dynamic movements, bomb drops, dive bombs in phases
- **Preloaded assets**: Character art, stage art, background, and boss sprites

## Quick start

No build step or package manager required.

1. Clone or download this repository
2. Open `index.html` in a modern browser (double-click or drag into the window)

Use a recent **Chrome**, **Edge**, or **Safari** for best results.

## Controls

### Player 1

- `A` / `D` — move left / right
- `Space` — fire
- `C` — use skill (if available)

### Player 2

- `Numpad1` / `Numpad3` — move left / right
- `Numpad0` — fire
- `Numpad5` — use skill (if available)

### Both players

- `R` — restart the current stage (also works from some result screens)

## Characters

Each character has unique stats and skills (2 uses per skill):

- **Mr. Star**: HP 3, DMG 1, Skill: Healing Shot (Fire a shot that heals all players for 1 HP on hit)
- **Ninja Oreo**: HP 2, DMG 2, Skill: Shield (Create a shield that blocks 2 hits)
- **Sage Cheri**: HP 4, DMG 0.5, Skill: Group Heal (Heal all players for 1 HP)
- **Wizard Enos**: HP 3, DMG 1, Skill: Big Shot (Fire a giant bullet that deals 3x damage)

## Boss Stages

- **Stage 1 (Dragon Boss)**:
  - Moves left/right at top, drops bombs randomly
  - Phase 2 (half HP): Summons dive bombs from top
- **Stage 2 (Mr. Star Boss)**:
  - Phase 1 (first half HP): Stationary, bombs drop from random top positions
  - Phase 2: Moves left/right with floating animation, drops bombs from position and randomly from top

## Win & lose

- **Win**: Boss HP reaches zero
- **Lose**: Both players run out of lives

## Progression

1. On the overlay, choose characters for Player 1 and Player 2 (view stats and skills)
2. Clear stage 1 to proceed to stage 2
3. In stage 2, battle the corrupted Mr. Star
4. After clearing stage 2, view the **HAPPY ENDING** screen

## Easter eggs (debug / cheats)

- Type **`nnn`** in sequence — jump to the stage 1 clear screen
- Type **`mmm`** in sequence — jump to the stage 2 clear screen

## Asset layout

Paths are **relative to `index.html`**:

| Folder       | Contents                                      |
| ------------ | --------------------------------------------- |
| `character/` | Player and boss images                        |
| `stages/`    | Background, win/lose art, ending illustration |

File names are **case-sensitive** on many hosts (e.g. Linux/GitHub Pages). Keep extensions exactly as in code (`PNG`, `jpeg`, etc.).

## Project layout

| File         | Role                                                |
| ------------ | --------------------------------------------------- |
| `index.html` | UI, canvas rendering, game logic, input, overlays |

## Deploying (optional)

For static hosts (e.g. [GitHub Pages](https://pages.github.com/)), serve the repo root so `index.html` is the default document. No server-side code is required.

## Possible extensions

- Sound effects and background music
- Additional stages or boss attack patterns
- More characters or skill variations
- Pause menu and remappable keys
