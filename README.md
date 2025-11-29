# Cyberdream Theme for bat

A dark theme for [bat](https://github.com/sharkdp/bat) based on the [cyberdream.nvim](https://github.com/scottmckendry/cyberdream.nvim) color palette.

## Color Palette

- **Background**: ![#16181a](https://via.placeholder.com/15/16181a/16181a.png) `#16181a`
- **Foreground**: ![#ffffff](https://via.placeholder.com/15/ffffff/ffffff.png) `#ffffff`
- **Blue**: ![#5ea1ff](https://via.placeholder.com/15/5ea1ff/5ea1ff.png) `#5ea1ff` (functions)
- **Green**: ![#5eff6c](https://via.placeholder.com/15/5eff6c/5eff6c.png) `#5eff6c` (strings)
- **Cyan**: ![#5ef1ff](https://via.placeholder.com/15/5ef1ff/5ef1ff.png) `#5ef1ff` (operators, links)
- **Red**: ![#ff6e5e](https://via.placeholder.com/15/ff6e5e/ff6e5e.png) `#ff6e5e` (errors, deletions)
- **Yellow**: ![#f1ff5e](https://via.placeholder.com/15/f1ff5e/f1ff5e.png) `#f1ff5e` (classes, types)
- **Magenta**: ![#ff5ef1](https://via.placeholder.com/15/ff5ef1/ff5ef1.png) `#ff5ef1` (keywords)
- **Pink**: ![#ff5ea0](https://via.placeholder.com/15/ff5ea0/ff5ea0.png) `#ff5ea0` (tags)
- **Orange**: ![#ffbd5e](https://via.placeholder.com/15/ffbd5e/ffbd5e.png) `#ffbd5e` (numbers, constants)
- **Purple**: ![#bd5eff](https://via.placeholder.com/15/bd5eff/bd5eff.png) `#bd5eff` (constants)
- **Grey**: ![#7b8496](https://via.placeholder.com/15/7b8496/7b8496.png) `#7b8496` (comments)

## Installation

### 1. Locate your bat config directory

```sh
bat --config-dir
```

This typically returns:
- **Linux**: `~/.config/bat`
- **macOS**: `~/.config/bat`
- **Windows**: `%APPDATA%\bat`

### 2. Create the themes directory (if it doesn't exist)

```sh
mkdir -p "$(bat --config-dir)/themes"
```

### 3. Copy the theme file

```sh
cp cyberdream.tmTheme "$(bat --config-dir)/themes/"
```

### 4. Rebuild bat's cache

```sh
bat cache --build
```

### 5. Use the theme

You can use the theme in several ways:

**Temporarily (one-time use):**
```sh
bat --theme=Cyberdream yourfile.txt
```

**Set as default:**
Add this to your bat config file (`$(bat --config-dir)/config`):
```sh
--theme="Cyberdream"
```

Or set it via environment variable in your shell profile (`~/.bashrc`, `~/.zshrc`, `~/.config/fish/config.fish` etc.):
```sh
export BAT_THEME="Cyberdream"
```

```fish
set -Ux BAT_THEME Cyberdream
#or, to set it globally
set -gx BAT_THEME Cyberdream
```

## Verification

To see all available themes including Cyberdream:
```sh
bat --list-themes
```

To preview the theme:
```sh
bat --theme=Cyberdream --list-themes
```

## Screenshots

Try viewing different file types to see the theme in action:
```bash
bat --theme=Cyberdream example.py
bat --theme=Cyberdream example.js
bat --theme=Cyberdream example.md
```

## Credits

- Theme based on [cyberdream.nvim](https://github.com/scottmckendry/cyberdream.nvim) by [scottmckendry](https://github.com/scottmckendry)
- Created for [bat](https://github.com/sharkdp/bat) by [sharkdp](https://github.com/sharkdp)
