# Enos — Workflow

**Responsible member:** Shen Ziqi 25054114G
**Character:** Enos (Half-elf Mage)

**Tasks:** Video production (P1, P2, P3, P4, video_Wan2.7_r2v_00001_(1), end_A, endA, ENDB) · Workflow documentation



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

## Reflection on Demo Video and PPT Production

In addition to the technical contributions, I took on the task of creating a demo video and preparing the reflection section for our project PPT. This process allowed me to synthesize our group's efforts and reflect on the overall project experience.

### Demo Video Production
- **Process:** I compiled footage from our game development, including gameplay clips, character animations, and video assets (such as P1-P4 and ending sequences). Using video editing software, I synchronized the clips with narrative voiceover and background music to create a cohesive demo that showcases the game's features, story, and mechanics.
- **Challenges:** Managing large video files was a significant hurdle, especially with GitHub's size limits. This led to experimenting with compression techniques and Git LFS. However, Git LFS caused issues where the online webpage (GitHub Pages) could not read the videos properly. Ultimately, we chose to compress the videos instead of using LFS to ensure compatibility and successful deployment. Resolving this required multiple iterations of file optimization and repository adjustments.
- **Learnings:** This task enhanced my skills in video editing and highlighted the importance of asset management in web projects. It also emphasized the need for early testing of deployment pipelines to avoid last-minute issues.

### PPT Reflection
- **Process:** For the PPT, I summarized reflections on our workflow, technical challenges overcome (e.g., game logic bugs, video integration), and how the project aligned with our initial story concept.
- **Challenges:** Condensing complex technical details into concise, engaging slides while maintaining a reflective tone was tricky. Balancing factual reporting with personal insights required several revisions.
- **Learnings:** Preparing the reflection helped me appreciate the collaborative nature of the project. It reinforced lessons in version control, debugging, and cross-functional teamwork, and I gained a deeper understanding of how narrative elements (like our dual endings) integrate with interactive gameplay.

Overall, these tasks not only documented our progress but also provided valuable insights into improving future projects, such as better planning for asset sizes and more frequent integration testing.
