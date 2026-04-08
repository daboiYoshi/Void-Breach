# VOID BREACH 🚀

**A 3D-style space shooter built entirely with vanilla HTML, CSS & JavaScript — no server required.**

---

## How to Play

1. Open `index.html` in any modern browser (Chrome, Firefox, Edge, Safari).
2. Click **ENGAGE** to start.
3. Survive all 10 waves of enemies.

---

## Controls

| Input | Action |
|-------|--------|
| **WASD** / Arrow Keys | Move ship |
| **Mouse** | Aim / steer toward cursor |
| **Left Click** / **Space** | Fire |
| **1** | Switch to Plasma Cannon (laser) |
| **2** | Switch to Seeker Missile (homing) |
| **3** | Switch to Scatter Burst (spread shot) |
| **P** / **Esc** | Pause |

---

## Enemy Types

| Enemy | Description |
|-------|-------------|
| 🔴 **Fighter** | Fast, dives at you with sinusoidal weave |
| 🟠 **Bomber** | Slow, tanky, fires heavy rounds |
| 🟡 **Scout** | Tiny and erratic — fast strafing |
| 🟣 **Capital Ship** | Massive boss-class ship, multi-shot spread |

---

## Power-ups

| Icon | Type | Effect |
|------|------|--------|
| ❤️ | Health | +30 HP |
| 🛡️ | Shield | +50 Shields |
| ⚡ | Energy | +60 Energy |
| 🔥 | Rapid Fire | 2.5× fire rate (8s) |
| ✨ | Triple Shot | 3× laser streams (6s) |
| ⭐ | Invincible | Full invincibility (5s) |

---

## Upgrade System

Between waves, spend **credits** (earned from kills) to upgrade:
- Hull Plating (max HP)
- Shield Capacitor (max shields)
- Engine Boost (speed)
- Cannon Overcharge (laser damage)
- Energy Cell (max energy)
- Shield Regen Module (faster shield recovery)

---

## File Structure

```
space-shooter/
├── index.html          — Main entry point
├── README.md           — This file
├── css/
│   ├── style.css       — Main styles, screens, HUD
│   └── hud.css         — HUD animations, combos, effects
├── js/
│   ├── renderer.js     — Canvas 2D rendering engine
│   ├── audio.js        — Web Audio API procedural SFX + music
│   ├── game.js         — Core game engine (entities, physics, AI)
│   ├── hud.js          — DOM-based HUD/UI manager
│   └── main.js         — Boot & glue code
└── data/
    ├── config.json     — Game config, enemy/weapon stats, wave data
    └── upgrades.json   — Upgrade tree & achievements
```

---

## Technical Notes

- **No localhost required** — uses `fetch()` for JSON, which works fine with `file://` in most browsers.
  - If Chrome blocks local file fetch, run with: `chrome --allow-file-access-from-files`
  - Or use any browser's "Open File" feature.
- Pure **Canvas 2D** renderer with perspective projection for a 3D feel.
- Procedural audio via **Web Audio API** — all SFX synthesized in code.
- Fully **offline** — no CDN dependencies, no external assets.

Made by Snake Arcade. and daboiYoshi 2026. Contact info@daboiyoshi.com
