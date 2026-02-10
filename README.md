# Norton Commander Classic Skin for Midnight Commander

A classic Norton Commander color scheme for Midnight Commander, optimized for modern terminals like Warp.

## Features

- **Classic Blue Background**: Traditional DOS/Norton Commander dark blue (`color21`)
- **Warp Terminal Optimized**: Uses 256-color palette to prevent color overrides
- **High Visibility Marked Files**: Bright yellow (`color226`) and bold for files marked with Insert key
- **Clear Selection**: Yellow text on black background for cursor selection
- **Traditional Layout**:
  - Black background for status bar and button bar
  - Cyan buttons (Help, Menu, View, etc.)
  - White function key numbers on black
  - Classic line-drawing characters

## Installation

### macOS / Linux

```bash
# Create skins directory if it doesn't exist
mkdir -p ~/.local/share/mc/skins

# Download the skin
curl -o ~/.local/share/mc/skins/norton-classic.ini https://raw.githubusercontent.com/nicoonee/mc-norton-classic-skin/main/norton-classic.ini

# Edit your MC configuration
# Add this line to ~/.config/mc/ini under [Midnight-Commander] section:
# skin=norton-classic
```

Or manually add to `~/.config/mc/ini`:

```ini
[Midnight-Commander]
skin=norton-classic
```

### Quick Test

Test the skin without permanently changing your configuration:

```bash
mc -S ~/.local/share/mc/skins/norton-classic.ini
```

## Why This Skin?

This skin was specifically created to solve color visibility issues in Warp terminal, where:

- Standard named colors (like `blue`, `cyan`, `yellow`) get overridden by Warp's theme
- Marked files were hard to distinguish from unmarked files
- The classic MC look was lost due to terminal color substitution

### Solution

This skin uses **256-color palette codes** (`color21` for blue, `color226` for yellow) which Warp cannot override, ensuring consistent appearance regardless of terminal theme.

## Color Scheme

- **Main Background**: `color21` (classic blue)
- **Selection Cursor**: `color226` (bright yellow) on black
- **Marked Files**: `color226` (bright yellow) bold on blue
- **Status/Button Bar**: White/cyan on black
- **Dialogs**: Standard gray with cyan focus
- **Menus**: White/yellow on cyan

## Screenshots

*Coming soon*

## Compatibility

- ✅ Midnight Commander 4.8+
- ✅ Warp Terminal
- ✅ iTerm2
- ✅ Terminal.app
- ✅ Most 256-color terminals

## Contributing

Feel free to open issues or submit pull requests if you have suggestions for improvements!

## License

MIT License - Feel free to use and modify as needed.

## Acknowledgments

Inspired by the classic Norton Commander and DOS-era file managers.
