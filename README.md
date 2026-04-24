# Our Rations are All Stolen, So Why on Earth are We Still Adventuring in This Dungeon?

**SD5976 Final Project**

---

## Overview / 项目简介

An interactive narrative experience combining AI-generated short films and a browser-based mini-game, presented as a single HTML webpage.

一个结合AI生成短片与浏览器小游戏的互动叙事体验，以单一HTML网页形式呈现。

The experience flows as:

1. **Prologue / 序章 (AI short film ~90s):** Introduces the four characters, the dungeon world, Mr. Star's betrayal, and the journey to the final chamber
2. **Game Stage 1 / 游戏第一关:** Two players cooperate to defeat the Dragon — the dungeon's first great boss (恶龙)
3. **Cutscene / 过场:** Dragon falls; Mr. Star absorbs its dark power and transforms into boss form
4. **Game Stage 2 / 游戏第二关:** Fight Mr. Star in complete form — Mr. Star cannot be selected as a player character
5. **Ending / 结局 (AI short film ~60s):** Win → Ending A (Mr. Star moved by teammates' bonds, expels dark power, adventure continues); Lose → Ending B (teammates defeated, world becomes 美食星球)

**Total video runtime / 总视频时长: ~3.5 minutes (~210 seconds)**

---

## How to Run / 如何运行

Open `final.html` in a browser. No installation or server required.

在浏览器中打开 `final.html`，无需安装或服务器。

> The game alone (without videos) can be run from `game/index.html`.
> 仅游戏部分（不含视频）可从 `game/index.html` 单独运行。

> Edited video files are in `videos/Edited/`. Ensure the filenames referenced in `final.html` match those in that folder.
> 剪辑后的视频位于 `videos/Edited/`，请确认 `final.html` 中引用的文件名与该目录一致。

---

## Characters / 角色

| Character | Race / 种族 | Class / 职业 | Goal / 目标 |
|-----------|------------|-------------|-------------|
| **Mr.Star** | Magical creature, dog-bear hybrid / 魔法生物，狗熊混血 | Cute pet / Secret Boss | Reclaim dark power; turn the entire world into food / 夺回黑暗力量，把全世界变成食物 |
| **Cheri** | Elf / 精灵 | Monk / Mage | Discover his true self and escape the temple he grew up in / 发现真实自我，逃离从小生活的神殿 |
| **Enos** | Half-elf / 半精灵 | Wizard | Gather materials for his graduation thesis / 收集适合毕业论文的研究材料 |
| **Oreo** | Catfolk / 猫族 | Ninja-Assassin | Find the legendary medicine to cure her ninja grandfather / 寻找传说中能治愈忍者爷爷的药 |

Character reference: [polyu-storyworld](https://github.com/venetanji/polyu-storyworld/tree/main/characters)

---

## Story Summary / 故事概要

Enos leads a peculiar party deep into the underground dungeon for his graduation thesis. Mr. Star joins as the team mascot — incredibly huggable, and supposedly useful for detecting dark power. What the team does not know: Mr. Star was once human, his soul now possessing a 42cm dog-bear hybrid body, and his one true goal is to obtain the dungeon's dark power and turn the entire world into food.

After surviving the brutal Void Hole challenge, the exhausted team falls asleep — and wakes to find every ration gone. Mr. Star, bloated and crumb-covered, can no longer hide the truth. The team pushes on regardless, reaching the dungeon's final chamber: the Dragon. When the dragon falls, its dark power floods into Mr. Star. The transformation begins. The real final battle starts.

Enos率领一支奇特的队伍深入地下城收集毕业论文材料。Mr.Star以吉祥物身份加入——极其可爱，据说还能探测黑暗力量。队伍不知道的是：Mr.Star曾经是人类，灵魂寄居于一个42厘米的狗熊混血身体中，唯一目标是获得黑暗力量，把整个世界变成食物。

在勉强撑过"虚空之洞"后，疲惫的队伍沉睡，醒来发现所有口粮全部消失。圆滚滚、沾着碎屑的Mr.Star再也无法隐瞒真相。黑暗力量将他吞噬。最终决战开始。

---

## Project Structure / 项目结构

```
final_project_SD5976/
│
├── final.html                          # Main entry: prologue → game → ending
├── README.md
├── cover.JPG                           # Project cover image
├── story_outline.png                   # Story overview diagram
│
├── game/                               # Boss battle mini-game (zero-dependency HTML)
│   ├── index.html
│   ├── character_pixel/                # Pixel character sprites (PNG)
│   │   ├── dog.PNG                     # Mr.Star
│   │   ├── dog_weapon.png
│   │   ├── wizard.PNG                  # Enos
│   │   ├── wizard_weapon.png
│   │   ├── knight.PNG                  # Cheri
│   │   ├── knight_weapon.png
│   │   ├── cat.PNG                     # Oreo
│   │   ├── cat_weapon.png
│   │   ├── dragon.png                  # Stage 1 boss
│   │   ├── boss2.PNG                   # Mr.Star boss form (Stage 2)
│   │   ├── boss2_bomb.PNG
│   │   ├── boss1_bomb.png
│   │   └── Pixel_of_4.PNG
│   ├── stages/                         # Background and result screens
│   │   ├── background.png
│   │   ├── black1.jpeg
│   │   ├── black2.jpg
│   │   ├── star_black.jpeg
│   │   ├── gamewin_1.jpg
│   │   ├── gamewin_2.jpg
│   │   ├── gameover_1.jpg
│   │   └── gameover_2.png
│   ├── music/                          # Battle and result BGM/SFX
│   │   ├── Battle1_Shatter the Core.mp3
│   │   ├── Battle2_Void Hunger.mp3
│   │   ├── black.mp3
│   │   ├── victory.mp3
│   │   └── fail.mp3
│   └── README.md
│
├── videos/                             # AI-generated short films and raw clips
│   ├── Edited/                         # Final edited videos used in final.html
│   │   ├── Opening.mp4
│   │   ├── Prologue.mp4
│   │   ├── Boss2 CG.mp4
│   │   ├── HE_A.mp4                    # Ending A — Victory
│   │   └── BE EndingB.mp4             # Ending B — Defeat
│   ├── [raw clip files].mp4            # Unedited AI-generated clips (即梦AI output)
│   ├── Narration.mp3                   # Narration audio
│   ├── narration2.mp3
│   ├── Narratione.mp3
│   ├── NoteGPT_Speech_*.mp3
│   └── README.md
│
├── storyboard/                         # Storyboard scripts and key frames
│   ├── README.md                       # Scene-by-scene overview
│   ├── text/                           # AI video text prompts (bilingual EN/中文)
│   │   ├── prologue.md                 # 9 scenes × ~10s
│   │   ├── ending_a.md                 # 4 scenes × ~15s (victory)
│   │   ├── ending_b.md                 # 4 scenes × ~15s (defeat)
│   │   └── narration.txt               # Narration script
│   └── frames/                         # First/last frame images for 即梦AI / Lovart
│       ├── prologue/
│       ├── ending_a/
│       └── ending_b/
│
├── character_pics/                     # Character reference artwork
│   ├── Mr.Star/
│   ├── cheri/
│   ├── enos/
│   └── oreo/
│
├── group_work_contribution_and _workflow/   # Per-member work documentation
│   ├── 25057915g_LIYanling/            # LI Yanling
│   │   ├── README.md                   # Contribution overview
│   │   ├── prompts.md                  # Prompt records
│   │   ├── reflection.md               # AI tool reflection
│   │   ├── workflow_1.png
│   │   ├── workflow_2.png
│   │   └── workflow_3.png
│   ├── 25053695g_PANYiting/            # PAN Yiting
│   │   ├── README.md
│   │   ├── prompts.md
│   │   ├── reflection.md
│   │   ├── workflow1.png
│   │   └── workflow2.png
│   ├── 25054114g_SHENZiqi/             # SHEN Ziqi
│   │   ├── README.md
│   │   ├── prompts.md
│   │   ├── reflection.md
│   │   └── workflow.png
│   └── 25042425g_WANGDongni/           # WANG Dongni
│       ├── Contruibution.md
│       ├── reflection.md
│       ├── agent_text_to_image.png
│       ├── ai_platfrom_image_to_image.png
│       ├── comfyui_workflow_audio.jpg
│       └── cursor_vibecoding.png
│
├── ppt/                                # PPT slides
├── presentation/                       # Presentation materials
│   └── README.md
```

---

## Team Responsibilities / 分工

| Member / 成员 | Tasks / 负责内容 |
|--------------|----------------|
| **LI Yanling — 25057915g** | Project file architecture · Storyboard text prompts (all 3 videos, bilingual) · Main story content · `final.html` HTML display · PPT opening & story background slides |
| **PAN Yiting — 25053695g** | Cheri character segment · Storyboard generation · Video generation · Presentation PPT · Prologue& Ending A short film production and editing · Workflow docs |
| **SHEN Ziqi — 25054114g** | Enos character segment · Ending B short film production · Workflow docs |
| **WANG Dongni — 25042425g** | Game code (`game/index.html`) · Music generation (ComfyUI ACE-Step) · Game asset generation · `final.html` video integration · Win/lose logic · Workflow docs |

---

## AI Tools Used / 使用的AI工具

| Tool / 工具 | Purpose / 用途 |
|------------|---------------|
| **即梦AI (Jimeng AI)** | AI image generation for storyboard keyframes (first frame / last frame) / 生成分镜首帧和尾帧图片；also used for video clip generation / 亦用于生成视频片段 |
| **Lovart** | AI video generation from image pairs + motion prompts / 基于首尾帧图片和运动提示生成AI视频 |
| **ComfyUI ACE-Step 1.5** | Battle and result music/SFX generation / 生成战斗音乐与音效 |
| **Cursor** | Vibe coding for game development (`game/index.html`) / 游戏代码开发 |
| **Claude Code** | Storyboard prompt writing assistance, HTML integration / 分镜提示词写作辅助、HTML集成 |

---

## Video Production Workflow / 视频制作流程

```
Story script (storyboard/text/*.md)
        ↓
Generate first frame image — 即梦AI   [首帧图片]
Generate last frame image  — 即梦AI   [尾帧图片]
        ↓
Upload first + last frame to Lovart
Input motion prompt (视频运作提示词)
        ↓
Export video clip (~10–15s per clip)
        ↓
Edit and assemble clips → final .mp4
        ↓
Place in videos/ folder
```

Each scene in `storyboard/text/` contains **4 elements per clip**:
- 首帧 / First Frame Prompt (EN + 中文)
- 尾帧 / Last Frame Prompt (EN + 中文)
- 视频运作 / Motion Prompt (EN + 中文)
- Story Narration / 故事旁白 (EN + 中文)

---

## Assessment Criteria / 评估标准

| Criterion | How We Address It |
|-----------|------------------|
| Value / Novelty (25%) | Original game + AI narrative films; unique dual-ending interactive structure |
| GitHub repo — code works (50%) | `final.html` + `game/index.html` both run in-browser, zero dependencies |
| GitHub repo — workflow documented (50%) | `group_work_contribution_and _workflow/` — prompts + reflections for all 4 members |
| Uses polyu-storyworld / MCP (50%) | Characters sourced from [venetanji/polyu-storyworld](https://github.com/venetanji/polyu-storyworld) |
| All members contributed (50%) | Each member has their own workflow folder with documented process |
| Reflection (25%) | `*/reflection.md` — AI tool impact on pipeline, quality, and authorship |

---

#### Links / 链接

- Character database: [polyu-storyworld](https://github.com/venetanji/polyu-storyworld/tree/main/characters)
- Videos (external): （填写 Google Drive 或其他分享链接）
