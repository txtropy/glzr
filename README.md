# GlazeWM User Guide (my setup)

## 1. Mental model

- **Workspaces are roles, not apps.** Named by role, with a number where you need several.
- **Workspaces follow focus.** They are not pinned to a monitor (monitor indexes are unreliable). A workspace you jump to appears on the monitor you are on. If it is on the wrong screen, move it by direction.
- **One chord reaches any workspace:** `alt+g`, then a letter, then (for numbered groups) a number.

## 2. Workspaces and their keys

Each name is shown in the bar with the key letter underlined, like a Windows menu (for example `c̲ode1̲` means press `c`, then `1`).

| Workspace | After `alt+g` press | What lives there |
|---|---|---|
| `code1`-`code3` | **c**, then 1 / 2 / 3 | One VS Code project each, plus an optional terminal |
| `web1`-`web2` | **w**, then 1 / 2 | Browsers (e.g. one for the large screen, one for the small) |
| `tools1` - `tools3` | **t**, then 1 / 2 / 3 | Dev tools and applications (db, api, azure tools, etc.) |
| `chat` | c**h**at → `h` | Team chat, meeting app |
| `utils` | **u** | OS utilities: File Explorer, Task Manager |
| `notes` | **n** | Note-taking |
| `media` | **m** | Music |
| `other` | **o** | Miscellaneous |
| `0`-`9` | the digit | Scratch workspaces for things you have not named yet |

## 3. Key cheat sheet

### Workspaces

| Keys | Action |
|---|---|
| `alt+g`, then the keys above | Go to that workspace |
| `alt+shift+g`, then the same keys | Send focused window there and follow it |
| `Esc` (inside any chord) | Cancel |
| `alt+z` | Jump back to the previous workspace |
| `alt+a` / `alt+s` | Previous / next active workspace |

Examples: `alt+g`, `c`, `2` goes to `code2`. `alt+g`, `h` goes to `chat`. `alt+shift+g`, `w`, `1` sends the focused window to `web1`.

### Windows

| Keys | Action |
|---|---|
| `alt+h/j/k/l` | Focus left/down/up/right |
| `win+shift+h/j/k/l` | Move window in that direction |
| `alt+u/i/o/p` | Resize (narrower / shorter / taller / wider) |
| `alt+r` | Resize mode (h/j/k/l or arrows, Enter/Esc to leave) |
| `alt+f` | Fullscreen toggle |
| `alt+t` | Toggle tiling |
| `alt+shift+space` | Toggle floating (centered) |
| `alt+space` | Cycle focus: tiling, floating, fullscreen |
| `alt+v` | Change tiling direction for next window |
| `alt+m` | Minimize |
| `alt+shift+q` | Close window |
| `alt+enter` | Open Windows Terminal |

### Monitors

| Keys | Action |
|---|---|
| `alt+shift+a` / `f` / `d` / `s` | Move focused workspace to the monitor on the left / right / up / down |

### Recovery

| Keys | Action |
|---|---|
| `alt+shift+p` | Pause GlazeWM (all bindings off until pressed again) |
| `alt+shift+w` | Redraw all windows |
| `alt+shift+r` | Reload config |
| `ctrl+alt+shift+e` | Exit GlazeWM |

## 4. Zebar Styling (minimal)

**Zebar bar.** The bar is a separate widget pack, so its colors are not set by `config.yaml`. The pack lives in its own folder and is selected in Zebar's `settings.json`.

How to set up:
> Copy and paste these two files: html template `.\zebar\nord-bar\with-glazewm.html` & stylesheet `.\zebar\nord-bar\nord.css` to the following path `%APPDATA%\zebar\downloads\glzr-io.starter@0.0.0` or wherever your zebar widget pack lives.