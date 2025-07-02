# 🎨 Mushin Theme - Advanced Customization Guide

> *"Adapt what is useful, reject what is useless, and add what is specifically your own."* - Bruce Lee

This guide will help you customize the Mushin theme to perfectly align with your personal zen practice and aesthetic preferences.

## 🎋 CSS Variable System

The Mushin theme is built on a comprehensive CSS variable system that allows for easy customization without breaking the core design philosophy.

### Core Color Variables

```css
/* In your obsidian.css file, override these variables: */

:root {
  /* Primary Colors */
  --mushin-green: #6b7d6b;     /* Main accent color */
  --mushin-beige: #c9b896;     /* Secondary accent */
  --mushin-stone: #a8a8a8;     /* Neutral element */
  --mushin-paper: #fafafa;     /* Background base */
  --mushin-ink: #2c2c2c;       /* Primary text */
  --mushin-shadow: rgba(0, 0, 0, 0.08); /* Shadows */
}

/* Dark theme overrides */
.theme-dark {
  --mushin-green: #8fa68f;
  --mushin-beige: #d4c096;
  --mushin-paper: #1a1a1a;
  --mushin-ink: #e8e8e8;
  --mushin-shadow: rgba(0, 0, 0, 0.4);
}
```

### Typography Customization

```css
:root {
  /* Font Families */
  --font-text: "Your Preferred Font", "Inter", sans-serif;
  --font-interface: "Your Interface Font", "Inter", sans-serif;
  --font-monospace: "Your Code Font", "JetBrains Mono", monospace;
  
  /* Font Sizes */
  --font-text-size: 16px;      /* Base text size */
  --font-ui-small: 13px;       /* UI elements */
  --font-ui-medium: 14px;      /* Buttons, tabs */
  --font-ui-large: 16px;       /* Headers */
  
  /* Line Heights */
  --line-height-normal: 1.6;   /* Body text */
  --line-height-tight: 1.3;    /* Headings */
  --line-height-loose: 1.8;    /* Reading mode */
}
```

### Spacing and Layout

```css
:root {
  /* Custom spacing scale */
  --space-zen-xs: 4px;
  --space-zen-s: 8px;
  --space-zen-m: 16px;
  --space-zen-l: 24px;
  --space-zen-xl: 32px;
  --space-zen-xxl: 48px;
  
  /* Border radius customization */
  --radius-zen-small: 4px;
  --radius-zen-medium: 8px;
  --radius-zen-large: 12px;
  --radius-zen-xl: 16px;
  
  /* Reading width */
  --content-max-width: 800px;  /* Default optimal reading width */
  --sidebar-width: 300px;      /* Sidebar width */
}
```

## 🌸 Color Scheme Variations

### Seasonal Color Palettes

#### Spring Zen (Cherry Blossom)
```css
:root {
  --mushin-green: #7d8471;     /* Soft sage */
  --mushin-beige: #f4d1ae;     /* Warm cream */
  --mushin-accent: #d4a574;    /* Gentle peach */
  --background-primary: #fdf9f5; /* Warm white */
}
```

#### Summer Zen (Bamboo Grove)
```css
:root {
  --mushin-green: #6b8e6b;     /* Fresh bamboo */
  --mushin-beige: #d9e5d6;     /* Pale bamboo */
  --mushin-accent: #9fc49f;    /* Living green */
  --background-primary: #f8fdf8; /* Fresh white */
}
```

#### Autumn Zen (Maple Leaves)
```css
:root {
  --mushin-green: #8b7355;     /* Warm brown */
  --mushin-beige: #e6d2a6;     /* Golden beige */
  --mushin-accent: #cc9966;    /* Maple gold */
  --background-primary: #fdf8f2; /* Warm paper */
}
```

#### Winter Zen (Misty Mountains)
```css
:root {
  --mushin-green: #6b7a7a;     /* Stone gray */
  --mushin-beige: #d6d9d6;     /* Soft mist */
  --mushin-accent: #9bb3b3;    /* Cool sage */
  --background-primary: #fafcfc; /* Cool white */
}
```

## 🖋️ Typography Enhancements

### Serif Aesthetic
```css
:root {
  --font-text: "Crimson Text", "Georgia", serif;
  --font-interface: "Source Sans Pro", sans-serif;
}

/* Enhanced readability for serif */
.markdown-source-view,
.markdown-preview-view {
  line-height: 1.7;
  font-size: 17px;
}
```

### Monospace Minimalism
```css
:root {
  --font-text: "SF Mono", "Monaco", monospace;
  --font-interface: "SF Mono", "Monaco", monospace;
}

/* Monospace adjustments */
body {
  letter-spacing: 0.02em;
}
```

### Japanese Typography
```css
:root {
  --font-text: "Noto Sans CJK JP", "Yu Gothic", sans-serif;
  --font-interface: "Noto Sans CJK JP", "Yu Gothic", sans-serif;
}

/* Support for vertical writing */
.japanese-vertical {
  writing-mode: vertical-rl;
  text-orientation: upright;
}
```

## 🎭 Layout Customizations

### Wide Screen Optimization
```css
/* For ultrawide monitors */
.workspace-leaf-content {
  max-width: 1200px;
  margin: 0 auto;
}

.markdown-source-view,
.markdown-preview-view {
  max-width: 900px;
}
```

### Compact Mode
```css
/* For smaller screens or minimal setups */
:root {
  --space-zen-s: 6px;
  --space-zen-m: 12px;
  --space-zen-l: 18px;
  --font-text-size: 14px;
}

.workspace-tab-container {
  padding: var(--space-zen-s);
}
```

### Distraction-Free Mode
```css
/* Hide all UI elements except content */
.hide-zen-ui .workspace-sidebar,
.hide-zen-ui .status-bar,
.hide-zen-ui .titlebar {
  display: none;
}

.hide-zen-ui .workspace-leaf-content {
  border: none;
  box-shadow: none;
}
```

## 🌊 Animation Customizations

### Gentle Animations
```css
/* Slower, more meditative transitions */
* {
  transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
}

/* Breathing effect for focused elements */
.workspace-leaf-content:focus-within {
  transform: scale(1.002);
  box-shadow: 0 4px 16px var(--mushin-shadow);
}
```

### Minimal Motion
```css
/* For users who prefer reduced motion */
@media (prefers-reduced-motion: reduce) {
  * {
    transition: none !important;
    animation: none !important;
  }
}
```

### Zen Hover Effects
```css
/* Subtle elevation on hover */
.nav-file-title:hover,
.nav-folder-title:hover {
  transform: translateX(2px);
  border-left: 2px solid var(--mushin-green);
}

/* Gentle glow for interactive elements */
.clickable-icon:hover {
  box-shadow: 0 0 8px rgba(107, 125, 107, 0.3);
}
```

## 🔧 Plugin-Specific Customizations

### Calendar Plugin
```css
/* Mushin styling for calendar */
.calendar-container {
  background: var(--background-primary);
  border-radius: var(--radius-zen-medium);
}

.calendar-day {
  border-radius: var(--radius-zen-small);
}

.calendar-day.has-note {
  background: var(--mushin-beige);
  color: var(--mushin-ink);
}
```

### Kanban Plugin
```css
/* Zen kanban boards */
.kanban-plugin__board {
  background: transparent;
}

.kanban-plugin__item {
  background: var(--background-modifier-form-field);
  border: 1px solid var(--background-modifier-border);
  border-radius: var(--radius-zen-medium);
  box-shadow: var(--mushin-shadow);
}
```

### Graph View
```css
/* Harmonious graph colors */
.graph-view.color-fill {
  color: var(--mushin-green);
}

.graph-view.color-line {
  color: var(--mushin-beige);
}
```

## 🎨 Advanced Theming Techniques

### Custom Properties for Sections
```css
/* Different zones with different energy */
.workspace-sidebar {
  --zone-energy: calm;
  filter: saturate(0.9);
}

.workspace-leaf-content {
  --zone-energy: focus;
  filter: saturate(1.1);
}
```

### Contextual Color Adjustments
```css
/* Time-based theming */
@media (prefers-color-scheme: dark) {
  :root {
    --time-of-day: night;
    filter: contrast(0.95) brightness(0.95);
  }
}
```

### Breathing Space Variations
```css
/* Different breathing patterns */
.breathing-minimal {
  --breathing-multiplier: 0.5;
}

.breathing-generous {
  --breathing-multiplier: 1.5;
}

.breathing-meditative {
  --breathing-multiplier: 2;
}

/* Apply to spacing */
* {
  padding: calc(var(--base-padding) * var(--breathing-multiplier, 1));
}
```

## 🧘‍♀️ Accessibility Enhancements

### High Contrast Mode
```css
@media (prefers-contrast: high) {
  :root {
    --text-normal: #000000;
    --background-primary: #ffffff;
    --text-accent: #006600;
    --background-modifier-border: #333333;
  }
}
```

### Large Text Support
```css
@media (min-resolution: 120dpi) {
  :root {
    --font-text-size: 18px;
    --space-zen-m: 20px;
  }
}
```

### Motion Sensitivity
```css
.motion-sensitive {
  transition: none;
  animation: none;
}

.motion-sensitive * {
  transition: none;
  animation: none;
}
```

## 🌟 Creating Your Personal Zen

### Custom CSS Snippets Location
Place your custom modifications in:
```
YourVault/.obsidian/snippets/mushin-personal.css
```

### Template for Personal Customization
```css
/* My Personal Mushin Modifications */
/* Created: [Date] */
/* Purpose: [Your intention] */

:root {
  /* My color preferences */
  --my-accent: #your-color;
  --my-background: #your-background;
  
  /* My typography choices */
  --my-font: "Your Font", sans-serif;
  --my-size: 16px;
  
  /* My spacing preferences */
  --my-breathing: 1.2; /* Multiplier for spacing */
}

/* Apply my preferences */
.my-zen-space {
  color: var(--my-accent);
  font-family: var(--my-font);
  font-size: var(--my-size);
}
```

## 🎯 Best Practices

1. **Start Small**: Make one change at a time and observe how it affects your workflow
2. **Document Changes**: Keep notes about what you modified and why
3. **Test Both Modes**: Ensure your changes work in both light and dark themes
4. **Respect the Philosophy**: Maintain the zen principles of simplicity and clarity
5. **Share Mindfully**: If you create something beautiful, consider sharing with the community

## 🔄 Reverting Changes

To reset to default Mushin theme:
1. Remove or comment out your custom CSS
2. Restart Obsidian
3. The original zen will return

---

*"The master in the art of living makes little distinction between his work and his play, his labor and his leisure, his mind and his body, his information and his recreation, his love and his religion."* - James A. Michener

May your customizations deepen your practice and enhance your path to digital enlightenment. 