# 🛠 Installation Guide - Mushin Theme

> *"A journey of a thousand miles begins with a single step."*

This guide will help you install the **Mushin** Obsidian theme and achieve zen in your note-taking experience.

## 📋 Requirements

- **Obsidian**: Version 0.16.0 or higher
- **Operating System**: Windows, macOS, or Linux
- **Storage**: ~25KB for theme files

## 🚀 Quick Installation

### Method 1: Manual Installation (Recommended)

1. **Download the Theme**
   - Visit the [Releases page](../../releases)
   - Download the latest `mushin-theme-v1.0.0.zip`
   - Or clone this repository: `git clone https://github.com/Vlad3Design/mushin-obsidian-theme.git`

2. **Locate Your Themes Folder**
   
   **Windows:**
   ```
   %APPDATA%\Obsidian\themes\
   ```
   
   **macOS:**
   ```
   ~/Library/Application Support/obsidian/themes/
   ```
   
   **Linux:**
   ```
   ~/.config/obsidian/themes/
   ```

3. **Install the Theme**
   - Extract the downloaded zip file
   - Copy the `Mushin` folder to your themes directory
   - The final path should look like: `[themes-folder]/Mushin/theme.css`

4. **Activate the Theme**
   - Open Obsidian
   - Go to **Settings** → **Appearance** → **Themes**
   - Select **"Mushin"** from the dropdown
   - Experience zen ✨

### Method 2: Community Themes (Coming Soon)

The theme will be available through Obsidian's Community Themes browser in a future update.

## 🎨 First Time Setup

### Recommended Settings

For the optimal Mushin experience, adjust these settings:

```
Settings → Editor:
├── Show line numbers: OFF
├── Fold headings: ON
├── Fold indents: ON
└── Auto-pair brackets: ON

Settings → Appearance:
├── Base color scheme: Adapt to system (or choose preferred)
├── Translucent window: 85% (optional)
└── Native menus: ON (macOS)

Settings → Hotkeys:
├── Toggle fold on current line: Ctrl/Cmd + Enter
└── Command palette: Ctrl/Cmd + P
```

### Font Recommendations

Mushin works beautifully with these fonts (install separately):

**Primary Text:**
- **Inter** (Recommended) - [Download](https://rsms.me/inter/)
- **Noto Sans** - [Download](https://fonts.google.com/noto/specimen/Noto+Sans)
- **Source Sans Pro** - [Download](https://fonts.google.com/specimen/Source+Sans+Pro)

**Monospace/Code:**
- **JetBrains Mono** (Recommended) - [Download](https://www.jetbrains.com/lp/mono/)
- **Fira Code** - [Download](https://github.com/tonsky/FiraCode)
- **SF Mono** (macOS built-in)

## 🔧 Troubleshooting

### Theme Not Appearing
1. Verify the folder structure: `themes/Mushin/theme.css`
2. Restart Obsidian completely
3. Check file permissions (especially on Linux/macOS)

### Appearance Issues
1. Try switching between light/dark mode
2. Disable other CSS snippets temporarily
3. Check for plugin conflicts

### Performance Issues
1. Update Obsidian to the latest version
2. Disable unnecessary plugins
3. Clear Obsidian cache: `[vault-folder]/.obsidian/workspace`

## 🧘 Advanced Configuration

### Custom CSS Variables

Create a CSS snippet in **Settings** → **Appearance** → **CSS snippets**:

```css
/* Mushin Custom Overrides */
:root {
  /* Adjust accent color */
  --mushin-green: #your-preferred-color;
  
  /* Increase text size */
  --font-text-size: 17px;
  
  /* More line spacing */
  --line-height-normal: 1.8;
  
  /* Adjust sidebar width */
  --file-line-width: 280px;
}
```

### Plugin Compatibility

Mushin has been tested with these popular plugins:

✅ **Fully Compatible:**
- Dataview
- Daily Notes
- Calendar
- Templater
- Advanced Tables
- Excalidraw

⚠️ **Minor Adjustments Needed:**
- Kanban (some styling differences)
- Mind Map (custom colors may override)

❌ **Known Issues:**
- Some custom theme plugins may conflict

## 📱 Mobile Setup

For Obsidian Mobile (iOS/Android):

1. Install Obsidian on your mobile device
2. Sync your vault (including the theme)
3. The theme will automatically apply
4. Adjust text size in mobile settings if needed

## 🔄 Updating the Theme

1. Download the latest release
2. Replace the existing `Mushin` folder
3. Restart Obsidian
4. Your custom settings will be preserved

## 🆘 Getting Help

If you encounter issues:

1. **Check the [FAQ](../../wiki/FAQ)** (when available)
2. **Search [existing issues](../../issues)**
3. **Create a new issue** with:
   - Obsidian version
   - Operating system
   - Steps to reproduce
   - Screenshots (if applicable)

## 🙏 Community

- **Creator**: [@Vlad3Design](https://github.com/Vlad3Design)
- **Portfolio**: [vlad3d.art](https://vlad3d.art)
- **Issues**: [GitHub Issues](../../issues)
- **Discussions**: [GitHub Discussions](../../discussions)

---

*"The journey of a thousand miles begins with a single step."*

Welcome to your zen note-taking journey! 🌸 