# Enos — Workflow

**Responsible member:** Shen Ziqi 25054114G
**Character:** Enos (Half-elf Mage)

**Tasks:** Enos character segment · Ending B short film ·Opening film ·P1234 · Workflow documentation



***

Game Logic and Integration Support

Beyond the video production for Enos and Ending B, I also provided significant support in debugging, refining, and integrating the core game logic within `game/index.html`.

Key contributions include:

- **Boss AI Overhaul:**
  - Reworked the behavior for both bosses.
  - **Boss 1:** Implemented horizontal movement with random bomb drops.
  - **Boss 2:** Designed a two-phase battle. Phase 1 involves a stationary boss with random bomb spawns and a new floating animation. Phase 2 reverts to the original move-and-drop pattern.
  - Added a new "dive bomb" attack for Boss 1 at half health.
- **Player Character Refinement:**
  - Re-mapped Player 2 controls to the numpad (`1` for left, `3` for right, `0` for attack, `5` for skill).
  - Updated character stats (HP, damage) and implemented a skill system with usage limits and cooldowns.
  - Changed the Ninja's skill from temporary invincibility to a shield that blocks a set number of hits.
- **Bug Fixing and Debugging:**
  - Addressed a critical bug where the boss was not taking damage.
  - Fixed an issue preventing character skills from being triggered.
  - Resolved a UI overflow problem on the character selection screen.
  - Corrected a loading issue that resulted in a blank screen.
- **Video Integration and Git Troubleshooting:**
  - Assisted in integrating all video files into the main `final.html` page.
  - Diagnosed and resolved a complex issue related to **Git LFS** and **GitHub Pages** incompatbility, which prevented videos from playing on the live site.
  - The solution involved migrating files away from LFS, compressing oversized videos to meet GitHub's file size limits, and ultimately resetting the Git history to resolve persistent repository errors.

