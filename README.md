# Ghostty Configuration

A beautiful and efficient terminal configuration for [Ghostty](https://github.com/mitchellh/ghostty) with optimized appearance, window management, and custom keybindings.

## Overview

This configuration provides a modern terminal setup featuring:
- **Catppuccin Mocha** theme for a cohesive color scheme
- **FiraCode Nerd Font** for enhanced readability and icon support
- Transparent background with blur effect
- Custom split management keybindings
- Green accent color (#a6e3a1) for cursor and dividers

## Installation

1. Clone this repository to your Ghostty configuration directory:
   ```bash
   git clone <repository-url> ~/.config/ghostty
   ```

2. Or copy the `config` file to your Ghostty config location:
   ```bash
   cp config ~/.config/ghostty/config
   ```

## Configuration Breakdown

### Appearance

| Setting | Value | Purpose |
|---------|-------|---------|
| Theme | Catppuccin Mocha | Modern dark color scheme |
| Font Family | FiraCode Nerd Font | Monospace font with ligatures and Nerd Font icons |
| Font Size | 12.0 | Comfortable default size |

### Window

| Setting | Value | Purpose |
|---------|-------|---------|
| Width | 170 columns | Wide terminal for multitasking |
| Height | 45 rows | Tall terminal for vertical content |
| Tab Bar | Hidden | Cleaner appearance |
| Background Blur | Enabled | Visual effect on background |
| Background Opacity | 0.95 (95%) | Transparent background |
| Split Divider Color | #a6e3a1 | Green divider matching accent |

**Note:** `window-save-state = never` ensures the window size resets to these defaults on each launch.

### Cursor

| Setting | Value | Purpose |
|---------|-------|---------|
| Style | Bar | Thin vertical cursor |
| Blinking | Disabled | Static cursor for focus |
| Color | #a6e3a1 | Green accent color |
| Copy on Select | Enabled | Auto-copy selected text |

**Cursor Integration:** `shell-integration-features = no-cursor` disables cursor shape changes from shell integration.

### Keybindings

Custom keybindings provide efficient window and split management:

| Keybind | Action |
|---------|--------|
| `Ctrl+Shift+F` | Toggle fullscreen |
| `Ctrl+Shift+M` | Toggle maximize |
| `Ctrl+Shift+Z` | Toggle split zoom |
| `Ctrl+Shift+Left` | Navigate to left split |
| `Ctrl+Shift+Right` | Navigate to right split |
| `Ctrl+Shift+Up` | Navigate to upper split |
| `Ctrl+Shift+Down` | Navigate to lower split |
| `Ctrl+Shift+Enter` | Create new split (auto-direction) |
| `Ctrl+Shift+D` | Close current split |

## Requirements

- [Ghostty](https://github.com/mitchellh/ghostty) terminal emulator
- [FiraCode Nerd Font](https://www.nerdfonts.com/) installed on your system

## Usage

After installation, Ghostty will automatically load this configuration. All custom keybindings are active by default.

### Split Management Example

```
Ctrl+Shift+Enter    # Create first split
Ctrl+Shift+Right    # Move to right split
Ctrl+Shift+Enter    # Create another split in the new pane
Ctrl+Shift+D        # Close current split when done
```

## Customization

Edit the `config` file to customize:
- **Theme**: Change to any supported Ghostty theme
- **Font**: Modify `font-family` and `font-size`
- **Dimensions**: Adjust `window-width` and `window-height`
- **Colors**: Update cursor and divider colors
- **Keybindings**: Add or modify keybind entries

## References

- [Ghostty Documentation](https://github.com/mitchellh/ghostty)
- [Catppuccin Mocha](https://github.com/catppuccin/catppuccin)
- [FiraCode Font](https://github.com/tonsky/FiraCode)