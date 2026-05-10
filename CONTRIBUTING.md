# Contributing to fuzz-wall

Thanks for taking the time to contribute!!

## Ways to contribute
- Report bugs via [Issues](https://github.com/youngcoder45/fuzz-wall/issues)
- Suggest new wallpaper setters or WM support
- Submit pull requests

## Guidelines
- Keep it POSIX sh (no bash-specific syntax)
- Test on at least one Wayland and one X11 WM before submitting
- One feature/fix per PR
- Update README if you add a new wallpaper setter

## Adding a new wallpaper setter
In the `set_wallpaper()` function, add a new case:
```sh
yournewsetter)
    yournewsetter --some-flag "$WALL" ;;
```
And add it to `detect_setter()` in the right block (Wayland or X11).

## Commit style
```
fix: handle missing wallpaper directory gracefully
feat: add swww transition support
docs: update README with nitrogen example
```
