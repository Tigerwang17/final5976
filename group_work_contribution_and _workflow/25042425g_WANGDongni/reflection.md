# Reflection — Oreo

**Member:** Wang Dongni
**Character:** Oreo · Game Development · HTML Integration

---

## How Did AI Tools Affect Your Production Pipeline?

**Tools used:** Cursor (game development), ComfyUI\Agent Bot\Lovart (Game assets generation)

**Before AI tools, this task would have required:**

- Writing most Canvas gameplay logic manually (movement, collision, boss patterns, stage flow, and UI states)
- Building and testing each feature with slower trial-and-error debugging across many small code edits
- Manually coordinating visual/audio asset integration, path management, and repeated browser validation
- Handling GitHub update synchronization and commit organization with higher communication and time cost

**With AI tools, the process became:**

- Converting feature ideas into prompt-driven implementation cycles, then refining details through fast iterations
- Reusing AI-assisted code edits for repeated tasks (UI text updates, stage transitions, audio triggers, and state logic)
- Integrating generated assets (images/music) faster with immediate path checks and in-browser validation
- Keeping GitHub updates cleaner by committing focused batches after each completed gameplay change

**Unexpected challenges:**

- Prompt precision mattered: vague requirements often produced correct code structure but incorrect gameplay behavior
- Audio autoplay/browser policy limits required fallback handling and extra testing for reliable playback
- Asset consistency across tools (Lovart, ComfyUI, Agent Bot) still required manual curation and naming discipline
- AI output was fast but not always aligned with project style, so human review remained essential

---

## What Were the Implications of Including AI Tools in Your Output?

**Creative implications:**
AI tools expanded the range of ideas we could test in limited time. Instead of committing to one design early, I explored multiple stage flows, result screens, and feedback effects (BGM, hit SFX, transition pages) before selecting the final version. This made the game feel more intentional, but it also meant I had to actively control consistency so the visual and interaction style stayed coherent.

**Quality implications:**  
AI-assisted coding significantly improved development speed, but quality still depended on human verification. Most generated logic needed at least one review pass for edge cases (state switching, event timing, audio overlap, and route jumps). In practice, AI produced a strong draft, while final stability came from manual testing and correction.

---

## Key Learnings

1. **Prompt quality directly affects code quality.** Clear constraints and expected outcomes reduce rework.
2. **Fast generation still needs disciplined review.** AI speed is valuable only when paired with structured testing.
3. **Tool diversity is useful when roles are clear.** Platform AI, ComfyUI, and Agent Bot each work best in different stages.

---

## If I Did It Again…

I would define a stricter production checklist at the start: naming conventions, asset specs, stage-state mapping, and audio behavior rules. I would also prepare reusable prompt templates for recurring game tasks (UI updates, event wiring, and transition logic) and schedule checkpoint-based QA after each feature block to reduce late-stage fixes.