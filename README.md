# ⚡ CHAOSOS — A WebOS for the Restless

A single-file, browser-based operating system with draggable windows, a working synth music player, a spray paint app, a terminal, and zero passwords. Built for the WebOS 1 mission.


---

##  Getting Started

No install, no build step, no dependencies.

1. Download `webos.html`
2. Open it in any modern browser (Chrome, Firefox, Edge, Safari)
3. That's it. You're in.

>  Click anywhere once before hitting play on the music player — browsers block audio until you interact with the page.

---

## 🖥️ Apps

| App | Icon | What it does |
|---|---|---|
| **Notepad** | ✏️ | A scratchpad textarea with a terminal-green monospace look. Nothing fancy, just write. |
| **Terminal** | 💀 | A tiny shell with real commands: `help`, `hello`, `date`, `joke`, `matrix`, `graffiti`, `clear`. |
| **Spray Paint** | 🎨 | A real drawing canvas — pick a neon color, set brush size, and tag the canvas. Has a clear button. |
| **Music Player** | 🎵 | A working synth player. Generates 4 original distorted punk/chiptune tracks live using the Web Audio API — no audio files. Includes a real-time frequency EQ visualizer. |
| **Devlog** | 📓 | Shows the project's dev history (3+ entries) and lets you add your own logs on the fly. |
| **About** | 💥 | System info, version, and feature tags. |

---

## 🎮 Controls & Behavior

- **Drag** any window by its titlebar
- **Resize** from the bottom-right corner handle
- **Minimize / Maximize / Close** with the colored dots (top-left of each window — yes, that's the joke)
- **Taskbar** at the bottom shows all open windows — click to refocus or restore
- **Start menu** (`▤ APPS` button, bottom-left) launches any app from one place
- **Double-click** desktop icons to open apps
- **Clock** in the taskbar runs live
- Boot-time notifications pop in from the bottom-right

---

##  Mission Requirements Checklist

| # | Requirement | Status |
|---|---|---|
| 1 | Working webpage with multiple draggable windows |  All 6 apps open in independent draggable/resizable windows |
| 2 | Looks like your own, not a copy of the guide |  Custom graffiti/punk theme, neon palette, animated wallpaper |
| 3 | At least 3 devlogs showing progress |  See the 📓 Devlog app — 3 built-in entries, expandable |
| 4 | At least 1 new feature not in the guide |  Live synth **Music Player** with Web Audio-generated tracks + EQ visualizer, plus a custom **Terminal** and **Spray Paint** app |
| 5 | No password — anyone can test it |  Opens straight to the desktop, no login screen |

---

##  Tech Stack

- **HTML / CSS / vanilla JavaScript** — single file, no frameworks
- **Web Audio API** — real-time synthesized audio (oscillators, distortion via wave-shaping, bandpass filters, analyser node for the EQ)
- **Canvas API** — animated graffiti wallpaper + spray paint app
- **Google Fonts** — Permanent Marker, Space Grotesk, Share Tech Mono

---

##  Project Structure

```
webos.html   ← everything. one file. that's the whole project.
```

---

##  Known Quirks

- Audio requires a user click first (browser autoplay policy — not a bug, just how browsers work)
- Devlog entries reset on page refresh (no backend/storage — by design, keeps it a static file)
- Maximize toggles full-screen-ish; minimize hides the window until you click it in the taskbar

---

##  Devlog Highlights

- **Initial commit** — basic window dragging up and running
- **Spray paint feature** — neon brush canvas added
- **Music player + polish** — synth audio engine wired up, glitch animations added

(Full logs live inside the app itself — open 📓 Devlog to read and add more.)

---

