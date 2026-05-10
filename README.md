# fuzz-wall

A minimal fuzzel-based wallpaper picker that works across Wayland and X11.

## Features
- Works on Wayland and X11
- Auto-detects installed wallpaper setter
- Custom wallpaper directory via env var
- No config files needed

## Dependencies
- `fuzzel`
- One of: `swaybg`, `swww`, `feh`, `nitrogen`, `xwallpaper`
- Optional: `libnotify` for error notifications

## Supported WMs
| WM | Session | Setter |
|---|---|---|
| Sway | Wayland | swaybg |
| Hyprland | Wayland | swww / swaybg |
| river | Wayland | swaybg |
| i3 | X11 | feh |
| bspwm | X11 | feh / nitrogen |
| openbox | X11 | nitrogen |

## Install

### AUR
```bash
paru -S fuzz-wall
# or
yay -S fuzz-wall
```

### Manual
```bash
git clone https://github.com/youngcoder45/fuzz-wall
cd fuzz-wall
chmod +x fuzz-wall
cp fuzz-wall ~/.local/bin/
```

## Usage
```bash
fuzz-wall

# Custom wallpaper directory
FUZZ_WALL_DIR=~/Pictures/walls fuzz-wall
```

## License
MIT © Aditya
