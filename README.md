# MidnightCookie — BetterDiscord Theme

![BetterDiscord](https://img.shields.io/badge/BetterDiscord-theme-7289DA.svg)
![CSS3](https://img.shields.io/badge/CSS3-powered-blue.svg)
![Status](https://img.shields.io/badge/status-draft-yellow.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)

<p align="center">
  <img src="https://raw.githubusercontent.com/JDaxmaut/midnight-cookie/main/eef877db84c911f0b84f02e3ec60f4f4_1.png" alt="MidnightCookie" width="120">
</p>

A sophisticated dark theme with warm cookie-inspired accents and midnight blue tones.

## Features

- Warm brown accent colors (hsl 28°, 80%, 60%)
- Deep midnight blue backgrounds
- Smooth animations and transitions
- Custom scrollbar styling
- Hover effects on messages, channels, and buttons
- Adaptive design for mobile
- Dark/light mode support
- High contrast accessibility
- **Chat background image support** — works with Discord's native background feature

## Installation

1. Download `MidnightCookie.theme.css`
2. Move it to your BetterDiscord themes folder:
   - Windows: `%appdata%/BetterDiscord/themes/`
   - macOS: `~/Library/Application Support/BetterDiscord/themes/`
   - Linux: `~/.config/BetterDiscord/themes/`
3. Enable the theme in BetterDiscord settings

## Files

| File | Description |
|---|---|
| `MidnightCookie.theme.css` | Ready-to-use theme file for BetterDiscord |
| `midnight-source.css` | Source file with full styles (for development) |

## Chat Background

The theme supports Discord's native chat background feature. To use it:
1. Go to Discord Settings → Chat Background
2. Upload any image
3. The theme keeps messages readable with `backdrop-filter: blur(3px)`

## Development

The theme is built with CSS custom properties for easy customization:

```css
--accent-hue: 28;          /* Warm orange */
--accent-saturation: 80%;
--accent-lightness: 60%;
--midnight-primary: hsl(220, 15%, 12%);
--midnight-accent: hsl(28, 80%, 60%);
```