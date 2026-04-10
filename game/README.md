# Pixel Co-op Shooter (Dungeon Game)

A zero-dependency, browser-only two-player local co-op mini game. Open `index.html` to play—character select, two boss stages, result screens, and a Happy Ending.

## Features

- **Single file**: HTML, CSS, and JavaScript live in `index.html`
- **Same-screen co-op**: Player 1 and Player 2 move and shoot independently
- **Character select**: Pick a character for each player before starting
- **Two stages**: Beat stage 1 to unlock stage 2 (with a special restriction)
- **HUD**: Boss HP bar, character names, and lives (hearts)
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

### Player 2

- `9` / `0` (or `Numpad9` / `Numpad0`) — move left / right
- `=` — fire

### Both players

- `R` — restart the current stage (also works from some result screens)

## Win & lose

- **Win**: Boss HP reaches zero
- **Lose**: Both players run out of lives

## Progression

1. On the overlay, choose characters for Player 1 and Player 2
2. After clearing stage 1, pick characters again for stage 2
3. In stage 2, **Mr. Star** is corrupted and **cannot** be selected
4. After clearing stage 2, open the **HAPPY ENDING** screen

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
- A third stage or boss attack patterns
- Per-character stats (fire rate, bullet pattern, lives)
- Pause menu and remappable keys
