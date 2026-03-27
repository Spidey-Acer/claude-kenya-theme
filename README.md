# Claude Kenya — Savanna Dusk & Dawn

A VS Code color theme crafted by **Claude Community Kenya (CCK)** — East Africa's first official Claude developer community.

Inspired by Anthropic's brand palette fused with the golden-hour tones of the East African savanna.

[![VS Code Marketplace](https://img.shields.io/visual-studio-marketplace/v/claude-community-kenya.claude-kenya-theme?label=Marketplace&color=d97757&style=flat-square)](https://marketplace.visualstudio.com/items?itemName=claude-community-kenya.claude-kenya-theme)
[![Installs](https://img.shields.io/visual-studio-marketplace/i/claude-community-kenya.claude-kenya-theme?color=788c5d&style=flat-square)](https://marketplace.visualstudio.com/items?itemName=claude-community-kenya.claude-kenya-theme)
[![Rating](https://img.shields.io/visual-studio-marketplace/r/claude-community-kenya.claude-kenya-theme?color=6a9bcc&style=flat-square)](https://marketplace.visualstudio.com/items?itemName=claude-community-kenya.claude-kenya-theme)
[![License: MIT](https://img.shields.io/badge/License-MIT-5da1a3?style=flat-square)](LICENSE)

---

## Variants

### Savanna Dusk (Dark)

A deep, warm dark theme with charcoal backgrounds tinged with brown undertones. Terracotta orange accents cut through the darkness like campfire light across the Maasai Mara at dusk.

- 215 workbench color overrides
- 59 TextMate token scopes
- 19 semantic token rules

<!-- Add screenshot: ![Savanna Dusk](screenshots/dusk-preview.png) -->

### Savanna Dawn (Light)

A soft, parchment-toned light theme that captures the warm golden light of an East African sunrise. Muted earth tones keep readability high while maintaining warmth.

- 170 workbench color overrides
- 44 TextMate token scopes
- 16 semantic token rules

<!-- Add screenshot: ![Savanna Dawn](screenshots/dawn-preview.png) -->

---

## Installation

### VS Code Marketplace (recommended)

1. Open VS Code
2. `Ctrl+Shift+X` to open Extensions
3. Search **"Claude Kenya"**
4. Click **Install**
5. `Ctrl+K Ctrl+T` and select **Claude Kenya — Savanna Dusk** or **Savanna Dawn**

### From VSIX

```bash
code --install-extension claude-kenya-theme-1.0.1.vsix
```

### Manual

```bash
git clone https://github.com/Spidey-Acer/claude-kenya-theme.git
cp -r claude-kenya-theme ~/.vscode/extensions/
# Restart VS Code, then Ctrl+K Ctrl+T to select the theme
```

---

## Color Palette

Every color maps to the East African landscape and Anthropic's brand identity.

| Role | Dusk | Dawn | Inspired By |
|------|------|------|-------------|
| **Keywords** | `#d97757` | `#c25a3a` | Terracotta sunsets |
| **Functions** | `#6a9bcc` | `#4a7daa` | Kenyan sky |
| **Strings** | `#788c5d` | `#5a7340` | Acacia leaves |
| **Classes** | `#c9956b` | `#a07840` | Savanna grass |
| **Types** | `#5da1a3` | `#3d8082` | Indian Ocean teal |
| **Decorators** | `#8b7ec8` | `#6e62a6` | Jacaranda blossoms |
| **Errors** | `#e05252` | `#c23030` | Kenyan flag red |

Both variants share the same hue families, adjusted for contrast against their respective backgrounds. All text colors meet WCAG AA contrast ratios (4.5:1 minimum).

---

## Language Support

Optimized syntax highlighting for:

- **JavaScript / TypeScript** (including JSX/TSX)
- **Python**
- **Rust**
- **Go**
- **HTML / CSS / SCSS**
- **JSON / YAML / TOML**
- **Markdown**
- **Shell / Bash**
- **Dockerfile**
- **SQL**

Plus semantic highlighting support for any language with an LSP server.

---

## Project Structure

```
claude-kenya-theme/
  package.json                              # Extension manifest
  icon.png                                  # Marketplace icon (CCK logo)
  themes/
    savanna-dusk-color-theme.json            # Dark variant (864 lines)
    savanna-dawn-color-theme.json            # Light variant (644 lines)
```

No dependencies. No build step. Purely declarative JSON theme files.

---

## Contributing

This theme is open source and community-driven.

1. Fork the repo
2. Press `F5` in VS Code to launch the Extension Development Host
3. Edit the theme JSON files in `themes/`
4. Test against multiple languages (JS/TS, Python, Rust at minimum)
5. Ensure WCAG AA contrast compliance
6. Submit a PR with before/after screenshots

### Guidelines

- No trailing commas in theme JSON files (VS Code schema rejects them)
- Keep both Dusk and Dawn variants in sync: same hue families, adjusted for contrast
- Test the full workbench, not just syntax: sidebar, tabs, terminal, status bar, minimap

---

## Packaging & Publishing

```bash
# Install vsce (one-time)
npm install -g @vscode/vsce

# Package into .vsix
vsce package

# Publish (requires Personal Access Token)
vsce publish
```

---

## Credits

- **[Claude Community Kenya](https://claudekenya.org)** — East Africa's first official Claude developer community
- Color palette derived from [Anthropic's brand](https://anthropic.com) and the East African landscape
- Built with Claude Code from Nairobi

## License

[MIT](LICENSE) — use it, share it, remix it.
