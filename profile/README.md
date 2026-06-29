Copyright (C) 2026 ZionXiaoxiSuOGLocGo
SPDX-License-Identifier: GPL-3.0-or-later

# Zion's Store

AI agent skills and tools for game development. Compatible with [opencode](https://opencode.ai), Claude Code, Codex, Cursor, and other agent platforms.

---

## Projects

### [project-ledger](https://github.com/Zions-store/project-ledger)

Project structure analysis and development logging — a pair of skills that give AI agents persistent project context.

| Skill | Description |
|-------|-------------|
| [**project-onboard**](https://github.com/Zions-store/project-ledger/tree/master/project-onboard) | Auto-detect project type and generate `AGENTS.md` — 11 rule packs (Unity, Unreal, Node.js, Python, Rust, Go, Java, C/C++, C#, Lua, General), zero dependencies |
| [**project-docs**](https://github.com/Zions-store/project-ledger/tree/master/project-docs) | Three-document project knowledge system — `AGENTS.md` + `PROJECT_STATE.md` + `DEVLOG.md` with multi-language support |

### Workflow

```
project-onboard    →  AGENTS.md         (understand the project)
     ↓
project-docs       →  PROJECT_STATE.md  (track status)
                   →  DEVLOG.md         (record history)
```

## Installation

```bash
# Clone the monorepo
git clone https://github.com/Zions-store/project-ledger.git

# Symlink skills to your agent's directory
# opencode
mklink /J %USERPROFILE%\.config\opencode\skills\project-onboard  project-ledger\project-onboard
mklink /J %USERPROFILE%\.config\opencode\skills\project-docs     project-ledger\project-docs

# Claude Code
ln -s $(pwd)/project-ledger/project-onboard ~/.claude/skills/project-onboard
ln -s $(pwd)/project-ledger/project-docs    ~/.claude/skills/project-docs
```

## License

All projects are GPL-3.0. See each project for details.
