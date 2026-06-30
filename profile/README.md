Copyright (C) 2026 ZionXiaoxiSuOGLocGo
SPDX-License-Identifier: GPL-3.0-or-later

# Zion's Store

AI agent skills and tools for game development. Compatible with [opencode](https://opencode.ai), Claude Code, Codex, Cursor, and other agent platforms.

---

## Projects

### [project-ledger](https://github.com/Zions-store/project-ledger)

| Skill | Description |
|-------|-------------|
| [**project-onboard**](https://github.com/Zions-store/project-ledger/tree/master/project-onboard) | Auto-detect project type and generate `AGENTS.md` — 11 rule packs, zero dependencies |
| [**project-docs**](https://github.com/Zions-store/project-ledger/tree/master/project-docs) | Three-document project knowledge system — `AGENTS.md` + `PROJECT_STATE.md` + `DEVLOG.md` with type-specific templates and LLM-native multi-language |
| [**unreal-manual**](https://github.com/Zions-store/project-ledger/tree/master/unreal-manual) | Comprehensive UE5 reference — core concepts, C++/Blueprint patterns, GAS, MCP, advanced gameplay (2300+ lines) |
| [**unity-manual**](https://github.com/Zions-store/project-ledger/tree/master/unity-manual) | Comprehensive Unity reference — C# scripting, URP/HDRP, Shader Graph, architecture patterns, mobile optimization (1800+ lines) |

### Workflow

```
project-onboard    →  AGENTS.md         (understand the project)
     ↓
project-docs       →  PROJECT_STATE.md  (track status, type-specific)
                   →  DEVLOG.md         (record history)
     ↑
unreal-manual      →  engine reference  (how to build it)
unity-manual       →  engine reference
```

## Installation

```bash
git clone https://github.com/Zions-store/project-ledger.git

# opencode Junctions (Windows)
mklink /J %USERPROFILE%\.config\opencode\skills\project-onboard  project-ledger\project-onboard
mklink /J %USERPROFILE%\.config\opencode\skills\project-docs     project-ledger\project-docs
mklink /J %USERPROFILE%\.config\opencode\skills\unreal-manual    project-ledger\unreal-manual
mklink /J %USERPROFILE%\.config\opencode\skills\unity-manual     project-ledger\unity-manual

# Claude Code symlinks
ln -s $(pwd)/project-ledger/project-onboard ~/.claude/skills/project-onboard
ln -s $(pwd)/project-ledger/project-docs    ~/.claude/skills/project-docs
ln -s $(pwd)/project-ledger/unreal-manual   ~/.claude/skills/unreal-manual
ln -s $(pwd)/project-ledger/unity-manual    ~/.claude/skills/unity-manual
```

## License

All projects are GPL-3.0. See each project for details.
