# My Suckless Setup

A custom suckless build for Arch Linux with personal patches and configurations.

## Components

- **dwm** - Dynamic Window Manager
- **st** - Simple Terminal
- **dmenu** - Application launcher
- **dwmblocks-async** - Modular async status bar

## Patches Applied

### dwm
- statuscmd (clickable status bar)
- XF86 media keys (volume, brightness)

## Keybindings

| Key | Action |
|-----|--------|
| Mod + Enter | Open terminal (st) |
| Mod + d | dmenu launcher |
| Mod + w | LibreWolf browser |
| Mod + q | Kill window |
| Mod + Shift + q | Quit DWM |
| Mod + 1-9 | Switch tags |
| Print | Full screenshot (scrot) |
| Mod + Print | Area screenshot |
| F2 | Volume down |
| F3 | Volume up |
| F4 | Brightness down |
| F5 | Brightness up |

## Status Bar Blocks

- WiFi + download speed
- Memory usage
- Battery status
- Volume
- Brightness
- Date & Time

## Dependencies

```bash
sudo pacman -S brightnessctl pactl scrot playerctl terminus-font
```

## Installation

```bash
git clone https://github.com/ruvindalakmal/suckless.git
cd suckless/dwm && sudo make clean install
cd ../st && sudo make clean install
cd ../dmenu && sudo make clean install
cd ../dwmblocks-async && sudo make clean install
```
