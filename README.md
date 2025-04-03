# Qtile Configuration

This repository contains a customized configuration file for Qtile, a dynamic tiling window manager written in Python. This configuration includes key bindings, layouts, widgets, and other settings tailored for an efficient and productive workflow.

## Features
- **Custom Key Bindings:**
  - Window navigation and management.
  - Launching applications such as terminals and browsers.
  - Layout switching and resizing windows.
  - System actions (shutdown, restart, reload config).
- **Multiple Layouts:**
  - Columns, Max, and more (commented out options available).
- **Autostart Script:**
  - Runs a script located at `~/.config/qtile/autostart.sh` on startup.
- **Floating Window Rules:**
  - Specific applications (like GPG pinentry and SSH prompts) open as floating windows.
- **Wayland Support:**
  - Virtual Terminal (VT) switching is configured for Wayland.

## Key Bindings

| Key Combination        | Action |
|------------------------|--------|
| `Mod + Return`        | Open terminal |
| `Mod + h/l/j/k`      | Move focus left/right/down/up |
| `Mod + Shift + h/l/j/k` | Move windows |
| `Mod + Control + h/l/j/k` | Resize windows |
| `Mod + w`            | Kill focused window |
| `Mod + Tab`         | Switch layouts |
| `Mod + f`           | Toggle fullscreen |
| `Mod + t`           | Toggle floating |
| `Mod + Control + r` | Reload configuration |
| `Mod + Control + q` | Quit Qtile |
| `Mod + Space`       | Switch to the next window |
| `Mod + Shift + Return` | Toggle split layout |
| `Mod + F2`          | Launch Floorp Browser |
| `Mod + F3`          | Launch qutebrowser |

For more key bindings, refer to the `keys` section in `config.py`.

## Layouts
- **Columns** (Default, supports resizing and stacking)
- **Max** (Full-screen layout for focused window)
- Additional layouts like MonadTall, Bsp, Matrix, and Tile are available (commented out in config).

## Installation
1. Ensure Qtile is installed on your system.
2. Copy the configuration file to `~/.config/qtile/config.py`:
   ```bash
   mkdir -p ~/.config/qtile
   cp config.py ~/.config/qtile/
   ```
3. (Optional) Create an autostart script at `~/.config/qtile/autostart.sh` and make it executable:
   ```bash
   touch ~/.config/qtile/autostart.sh
   chmod +x ~/.config/qtile/autostart.sh
   ```
4. Restart Qtile to apply changes:
   ```bash
   qtile restart
   ```

## Customization
- Modify key bindings to fit your workflow.
- Adjust layouts and widget settings as needed.
- Edit the autostart script to include applications you want to start with Qtile.



