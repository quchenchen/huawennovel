# The Cursed Bond (Overseas Short Story)

**English werewolf romance for overseas platforms (GoodNovel / Dreame / Webnovel)**  
*A Bond that is law, not love. A secret that could topple a kingdom.*

---

## 📊 Project Status

- **Target**: 28,000–30,000 words (short story, pay-per-volume)
- **Current**: 20,724 words (v2 draft, 17 chapters)  
- **Progress**: ~74% of target
- **Chapters**: 17/17 drafted (v2), all in `chapters/v2/`
- **Exports**: `export/The-Cursed-Bond-v2-Final.docx` (latest draft)
- **Git**: Local commits only (no remote push due to network; history intact)

> 💡 This README is updated with each major milestone. See commit history for detailed progress.

---

## 🧭 How to Use This Project

This project uses the **huawennovel-skills** (v2.6.1) for standardized creation.  
All interactions with the skill happen through natural language prompts in the chat.

### Common Commands

| Prompt | What It Does |
|--------|--------------|
| `初始化小说项目` | Initialize a new novel project (creates folder structure, base files) |
| `写第一章` / `创作下一章` | Start writing a chapter (follows the 9-step creation flow) |
| `修改第X章` | Rewrite an existing chapter (triggers optimization workflow) |
| `更新读者反馈` | Paste reader feedback → record → analyze → suggest actions |
| `更新写作指导` | Scan `docs/` → extract writing rules → update `references/writing-guide.md` |
| `查看项目状态` | Show current word count, chapter count, git status, etc. |
| `回滚到第X次提交` | Revert project to a historical commit (with backup) |

> 📌 **Tip**: The skill has two modes:  
> - **Novice Mode**: Guided walkthrough (for first projects)  
> - **Standard Mode**: Full control (for experienced users)  
> Mode is auto-detected via `.skill-mode` file. Complete a full short story or 10+ chapters to graduate to Standard.

---

## 📁 Project Structure

```
werewolf-overseas/
├── chapters/                  # Chapter manuscripts
│   └── v2/                    # v2 short story draft (17 chapters)
│       ├── Chapter-001-The-Bond.md
│       ├── Chapter-002-The-Refusal.md
│       └── ...                # up to Chapter-017-Getting-There.md
├── chapter-outlines/          # Archived chapter outlines (creation-step 3)
│   └── v2/                    # v2 outlines (if archived)
├── references/                # Core reference files (single source of truth)
│   ├── outline.md             # Global story outline (v2 short story)
│   ├── outline-v2-short.md    # Alternative: v2 short story outline
│   ├── characters.md          # Character bible
│   ├── writing-guide.md       # Writing rules (from docs/ + experience)
│   ├── reader-feedback.md     # Reader feedback log
│   └── blurb.md               # Overseas short story blurb (back-cover copy)
├── docs/                      # Source material (raw references)
│   ├── writing-guide/         # External guides (e.g., Alpha Things analysis)
│   ├── characters/            # Raw character notes
│   └── reader-feedback/       # Raw feedback screenshots/notes
├── export/                    # Generated exports
│   ├── build_docx_final.py    # Script to build DOCX from markdown
│   └── The-Cursed-Bond-v2-Final.docx
├── README.md                  # This file
└── .skill-mode                # Tracks skill mode (novice/standard) [auto-managed]
```

---

## 📈 Progress Tracking

Word count is tracked via `wc -w` (English word count) on the manuscript files.  
Updates to this README happen at key milestones:

| Milestone | Word Count | Chapters | Notes |
|-----------|------------|----------|-------|
| v1 Long Attempt | ~14,120 | Ch1-10 | Abandoned for pacing mismatch |
| v2 Draft Complete | 20,724 | 17 | First full short story draft |
| **Target** | **28,000–30,000** | **17–22** | Pay-per-volume sweet spot |

> 🔢 **Word count rule**: Only the manuscript text counts (no titles, markdown, or metadata).  
> Use `wc -w chapters/v2/*.md \| tail -1` to verify.

---

## 🛠️ Current Skill Version

- **Skill**: `huawennovel-skills` (v2.6.1)
- **Location**: `/Users/quchenchen/.copaw/workspaces/xiaoshuo/skills/`
- **Key Features Active**:
  - ✅ Novice/Standard mode system (auto-detected)
  - ✅ Batch mode rules (for rewrites like v1→v2)
  - ✅ Mandatory chapter summaries (for retroactive logging)
  - ✅ `wc -w` standard for word counting (no estimates)
  - ✅ Overseas short story blurb rules (Section 8)

> 🔧 Skill updates are pushed to: https://github.com/quchenchen/huawennovel.git  
> Latest commit: `31b4f31` (v2.6.1: batch mode chapter summaries mandatory)

---

## 📝 Notes & Conventions

- **Language**: English (overseas audience)
- **Naming**: Chapters use `Chapter-XXX-Title.md` format (three-digit)
- **Avoiding IP**: Character names are original (no Alpha Things copies)
- **Core Twist**: The Bond is constitutional law — speaking the binding words forces the King to accountability
- **Ending**: HFN (Happy For Now), not HEA — leaves room for sequels
- **Explicit Content**: None (focus on political intrigue, slow-burn tension)

---

## 🙏 Acknowledgments

- Reference analysis: *Alpha Things.docx* (via python-docx extract)  
- Skill foundation: openclaw/novel-writer-skill  
- Platform research: GoodNovel, Dreame, Webnovel submission guidelines  

---
*Last updated: 2026-05-15*  
*Maintained with huawennovel-skills v2.6.1*