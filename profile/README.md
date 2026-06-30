Copyright (C) 2026 ZionXiaoxiSuOGLocGo
SPDX-License-Identifier: GPL-3.0-or-later

# Zion's Store

AI agent skills and tools for game development. Compatible with [opencode](https://opencode.ai), Claude Code, Codex, Cursor, and other agent platforms.

---

## Projects

### [project-ledger](https://github.com/Zions-store/project-ledger)
Project analysis and documentation skills for AI agents.

| Skill | Description |
|-------|-------------|
| [**project-onboard**](https://github.com/Zions-store/project-ledger/tree/master/project-onboard) | Auto-detect project type and generate `AGENTS.md` — 11 rule packs, zero dependencies |
| [**project-docs**](https://github.com/Zions-store/project-ledger/tree/master/project-docs) | Three-document project knowledge system with type-specific templates and LLM-native multi-language |

### [unreal-manual](https://github.com/Zions-store/unreal-manual)
Comprehensive UE5 engine reference for AI agents — core concepts, C++/Blueprint patterns, GAS, MCP, delegates, smart pointers (2300+ lines, UE 5.0–5.8).

### [unity-manual](https://github.com/Zions-store/unity-manual)
Comprehensive Unity engine reference for AI agents — C# scripting, URP/HDRP, Shader Graph, architecture patterns, mobile optimization (1800+ lines, Unity 2022.3–Unity 6).

---

## Installation

```bash
# Clone individual repositories
git clone https://github.com/Zions-store/project-ledger.git
git clone https://github.com/Zions-store/unreal-manual.git
git clone https://github.com/Zions-store/unity-manual.git

# opencode Junctions (Windows)
mklink /J %USERPROFILE%\.config\opencode\skills\project-onboard  project-ledger\project-onboard
mklink /J %USERPROFILE%\.config\opencode\skills\project-docs     project-ledger\project-docs
mklink /J %USERPROFILE%\.config\opencode\skills\unreal-manual    unreal-manual
mklink /J %USERPROFILE%\.config\opencode\skills\unity-manual     unity-manual
```

## License

All projects are GPL-3.0. See each project for details.
