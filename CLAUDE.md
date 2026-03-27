# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

VS Code color theme extension by Claude Community Kenya (CCK). Two theme variants:
- **Savanna Dusk** — dark theme (`themes/savanna-dusk-color-theme.json`)
- **Savanna Dawn** — light theme (`themes/savanna-dawn-color-theme.json`)

Publisher: `claude-community-kenya` | VS Code engine: `^1.60.0`

## Build & Package Commands

```bash
# Install vsce globally (required for packaging/publishing)
npm install -g @vscode/vsce

# Package into .vsix
vsce package

# Publish to VS Code Marketplace (requires PAT)
vsce publish
```

No build step, no tests, no dependencies — the extension is purely declarative JSON theme files.

## Local Testing

Copy the entire `claude-kenya-theme` folder to `~/.vscode/extensions/`, restart VS Code, then select the theme via `Ctrl+K Ctrl+T`.

Alternatively, press `F5` in VS Code to launch an Extension Development Host with the theme loaded.

## Architecture

This is a static VS Code theme extension — no executable code:

- **`package.json`** — Extension manifest. Declares both themes under `contributes.themes` with `uiTheme` set to `vs-dark` (Dusk) and `vs` (Dawn).
- **`themes/*.json`** — Theme definitions following the [VS Code Color Theme schema](https://code.visualstudio.com/api/references/theme-color). Each contains:
  - `colors` — Workbench/UI color overrides (editor, sidebar, tabs, terminal, status bar, etc.)
  - `tokenColors` — TextMate token scopes for syntax highlighting
  - `semanticHighlighting` / `semanticTokenColors` — LSP-based semantic token overrides

## Color Palette Convention

Both themes share a semantic color mapping derived from Anthropic's brand palette + East African landscape tones:

| Role | Dusk hex | Dawn hex |
|------|----------|----------|
| Keywords / accents | `#d97757` | `#c25a3a` |
| Functions | `#6a9bcc` | `#4a7daa` |
| Strings | `#788c5d` | `#5a7340` |
| Classes | `#c9956b` | `#a07840` |
| Types | `#5da1a3` | `#3d8082` |
| Decorators | `#8b7ec8` | `#6e62a6` |
| Errors | `#e05252` | `#c23030` |

When modifying colors, keep both variants in sync — each role should use the same hue family, just adjusted for contrast against the respective background.

## Editing Guidelines

- Theme JSON files have no trailing commas — VS Code's schema validator will reject them.
- Test changes against multiple languages (JS/TS, Python, Rust at minimum) since token scopes vary.
- Ensure sufficient contrast ratios: WCAG AA (4.5:1) for text against backgrounds.
- The `$schema` reference at the top of each theme file enables IntelliSense in VS Code for valid color keys.
