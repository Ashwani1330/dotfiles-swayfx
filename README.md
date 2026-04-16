# Dotfiles (SwayFX)

Minimalist configuration for SwayFX (Wayland).

## Preview
<img width="1600" height="900" alt="Desktop Preview" src="https://github.com/user-attachments/assets/c59d7526-c87b-42d6-b585-a51255bc480a" />

## Components

| Component | Application | Notes |
| :--- | :--- | :--- |
| **Window Manager** | [SwayFX](https://github.com/WillPower3309/swayfx) | Blur & Radius enabled |
| **Bar** | [Waybar](https://github.com/Alexays/Waybar) | Custom CSS, MPRIS, & Pomodoro |
| **Terminal** | [Kitty](https://sw.kovidgoyal.net/kitty/) | Catppuccin Mocha Theme |
| **Launcher** | [Rofi](https://github.com/davatorium/rofi) | Run / Drun / Window modes |
| **Lock Screen** | [Swaylock](https://github.com/swaywm/swaylock) | Custom ring colors |
| **Notifications** | [SwayNC](https://github.com/ErikReider/SwayNotificationCenter) | Feature-rich notification center |
| **Compositor** | Native | SwayFX handles composition |

## Theming

  * **Palette:** Catppuccin Mocha
  * **Bar Font:** SF Pro Text, Inter, NotoSans Nerd Font
  * **Terminal Font:** FiraCode Nerd Font Mono
  * **Icons:** Papirus
  * **Wallpaper:** Managed via Sway config

## Key Bindings

<details>
<summary><b>Click to view full keybindings list</b></summary>

| Keybind | Action | Command |
| :--- | :--- | :--- |
| **Applications** | | |
| `Mod` + `Enter` | Open Terminal | `$term` (Kitty) |
| `Mod` + `n` | Open File Manager | `thunar` |
| `Mod` + `d` | App Launcher | `rofi -show drun` |
| `Mod` + `Shift` + `d` | Run Command | `rofi -show run` |
| `Mod` + `.` | Emoji Picker | `rofi -show emoji` |
| `Mod` + `c` | Clipboard Manager | `cliphist` |
| **Navigation & Workspaces** | | |
| `Alt` + `Tab` | MRU Window Swap | `swayr` |
| `Mod` + `Tab` | Visual Window List | `swayr switch-window` |
| `Mod` + `Ctrl` + `Arrows` | Move Workspace | `move workspace to output` |
| **System** | | |
| `Mod` + `Shift` + `q` | Kill Focused Window | `kill` |
| `Mod` + `Shift` + `x` | Lock Screen | `swaylock` |
| `Mod` + `Shift` + `c` | Reload Configuration | `reload` |
| `Mod` + `Shift` + `e` | Exit Sway | `swaynag` |
| **Screenshots** | | |
| `Mod` + `Shift` + `s` | Region Screenshot | `grim` + `slurp` |
| `Print` | Full Screenshot | `grim` |
| **Window Management** | | |
| `Mod` + `f` | Toggle Fullscreen | `fullscreen` |
| `Mod` + `Shift` + `Space` | Toggle Floating | `floating toggle` |
| `Mod` + `b` | Split Horizontal | `splith` |
| `Mod` + `v` | Split Vertical | `splitv` |
| `Mod` + `s` | Stacking Layout | `layout stacking` |
| `Mod` + `w` | Tabbed Layout | `layout tabbed` |
| `Mod` + `e` | Toggle Split | `layout toggle split` |
| `Mod` + `Minus` | Scratchpad (Show) | `scratchpad show` |
| `Mod` + `Shift` + `Minus` | Scratchpad (Move) | `move scratchpad` |
| **Hardware / Media** | | |
| `Vol Up/Down/Mute` | Audio Control | `pactl` |
| `Bright Up/Down` | Brightness Control | `brightnessctl` |
| `Play/Next/Prev` | Media Control | `playerctl` |

</details>

## Utilities Setup

  * **Screenshot:** `grim` + `slurp` (Copies to clipboard)
  * **Clipboard:** `cliphist` with Rofi integration
  * **Audio:** PipeWire with `qpwgraph` for patchbay control
  * **Gestures:** Native 3-finger (workspaces) and 4-finger (window list) swipes
  * **Tiling:** `autotiling` script
  * **Auth Agent:** `polkit-gnome`

---

### Sources
* **Waybar Config Base:** [Prateek7071/dotfiles](https://github.com/Prateek7071/dotfiles)
* **Wallpapers:** [dharmx/walls](https://github.com/dharmx/walls)
