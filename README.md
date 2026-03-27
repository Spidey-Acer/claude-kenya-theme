# Claude Kenya — Savanna Dusk & Dawn 🌅

A stunning VS Code color theme crafted by **Claude Community Kenya (CCK)** — East Africa's first official Claude developer community.

Inspired by the warmth of Anthropic's brand palette fused with the golden-hour tones of the East African savanna. Every color tells a story: terracotta sunsets, acacia greens, sky blues, and the deep charcoal of volcanic soil.

## 🎨 Two Variants

### Savanna Dusk (Dark)
A deep, warm dark theme with charcoal backgrounds tinged with brown undertones. Terracotta orange accents cut through the darkness like campfire light across the Maasai Mara at dusk.

### Savanna Dawn (Light)
A soft, parchment-toned light theme that captures the warm golden light of an East African sunrise. Muted earth tones keep readability high while maintaining warmth.

## Color Philosophy

| Role | Dusk (Dark) | Dawn (Light) | Inspired By |
|------|-------------|--------------|-------------|
| **Keywords** | `#d97757` | `#c25a3a` | Anthropic terracotta / sunset |
| **Functions** | `#6a9bcc` | `#4a7daa` | Anthropic blue / Kenyan sky |
| **Strings** | `#788c5d` | `#5a7340` | Anthropic green / acacia leaves |
| **Classes** | `#c9956b` | `#a07840` | Amber / savanna grass |
| **Types** | `#5da1a3` | `#3d8082` | Indian Ocean teal |
| **Decorators** | `#8b7ec8` | `#6e62a6` | Jacaranda blossoms |
| **Errors** | `#e05252` | `#c23030` | Kenyan flag red |

## Installation

### From VS Code Marketplace
1. Open VS Code
2. Go to Extensions (`Ctrl+Shift+X`)
3. Search for **"Claude Kenya"**
4. Click **Install**
5. `Ctrl+K Ctrl+T` → Select **Claude Kenya — Savanna Dusk** or **Savanna Dawn**

### Manual Installation
1. Clone or download this repo
2. Copy the `claude-kenya-theme` folder to `~/.vscode/extensions/`
3. Restart VS Code
4. Select the theme from Color Theme picker

### From VSIX
```bash
# If you have the .vsix file:
code --install-extension claude-kenya-theme-1.0.0.vsix
```

## Publishing to Marketplace

```bash
# Install vsce
npm install -g @vscode/vsce

# Package the extension
cd claude-kenya-theme
vsce package

# Publish (requires Personal Access Token)
vsce publish
```

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
- And all languages supported by VS Code's TextMate grammars

## Contributing

This theme is open source and community-driven. PRs welcome!

1. Fork the repo
2. Make your color changes in the theme JSON files
3. Test locally by copying to `~/.vscode/extensions/`
4. Submit a PR with before/after screenshots

## Credits

- **Claude Community Kenya** — [claudekenya.org](https://claudekenya.org)
- Color palette derived from [Anthropic's brand guidelines](https://anthropic.com)
- Built with love from Nairobi 🇰🇪

## License

MIT — use it, share it, remix it.

---

*"Every line of code deserves a sunset."* — CCK
