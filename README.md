# setup

Personal machine setup files, organized as GNU Stow packages.

## Layout

- `macos/` contains macOS-specific files, including `Brewfile` and Ghostty config.
- `linux-omarchy/` contains Omarchy/Hyprland, Waybar, and Linux Ghostty config.

## Install

From this repository:

```bash
cd ~/Work/setup
```

On Omarchy/Linux:

```bash
stow -t ~ linux-omarchy
```

On macOS:

```bash
stow -t ~ macos
brew bundle --file=~/Brewfile
```

## Notes

- `linux-omarchy/.config/hypr/monitors.conf` is machine-specific and assumes the current laptop plus `DP-4` external display setup.
- `linux-omarchy/.config/hypr/workspaces.conf` and `apps.conf` are kept for reference, but are not currently sourced by `hyprland.conf`.
- If Stow reports conflicts, move the existing target file aside first, then rerun `stow`.
