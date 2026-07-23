# 🚀 Vector Siege

**A neon arcade survival shooter — pilot a hero rocket, dodge terrifying dragons, and fight your way through progressively harder levels.**

**[▶ Play it live](https://briangaini.github.io/vector-siege/)**

---

## About

Vector Siege is a browser-based arcade shooter built entirely with React and the HTML5 Canvas API — no game engine, no external assets. Every visual (the hero rocket, enemy ships, dragon bosses, particle effects) is drawn procedurally in code, and every sound effect and voice line is synthesized live with the Web Audio API and Speech Synthesis API.

Survive waves of enemy rockets, collect power-ups, and fill the level meter to summon one of five distinct dragon bosses — each with its own look and its own escalating attack pattern, from a simple opening breath attack to full bullet-hell spirals and charge attacks at higher levels.

## Features

- **Progressive difficulty** — 5 unique dragon boss designs that cycle and intensify as you climb levels, each with attack patterns that unlock over time (aimed shots → ring bursts → spirals → charge attacks → minion summons)
- **9 power-ups** — Shield, Rapid Fire, Spread Shot, Homing Missiles, Piercing Laser, Freeze, Nuke, Heal, and 2x Score
- **Upgrade shop** — pick a permanent perk after every boss kill (more lives, faster fire rate, heavier damage, quicker dash, longer shields)
- **Dash/dodge move** with its own cooldown for skilled players
- **Boss weak points** — hit the eyes for critical damage
- **Environmental hazards** — asteroid fields to dodge from level 2 onward
- **Fully synthesized audio** — no sound files; every effect and the "Monster incoming" / "Monster defeated" voice lines are generated in real time
- **Difficulty select** (Casual / Normal / Brutal) and an accessibility toggle to reduce screen-shake and flash effects
- **Persistent high score**, saved locally in your browser
- **Mobile-friendly** — drag to move, tap to dash, fully playable one-handed

## Tech Stack

- **React 18** (loaded via ESM CDN, no build tooling required to run it)
- **HTML5 Canvas** for all rendering
- **Web Audio API** for procedural sound design
- **Web Speech API** for boss voice lines
- **Tailwind CSS** for UI chrome
- Pre-compiled to plain JavaScript (no runtime JSX transform) for fast, reliable loading

## Run it locally

No installation needed — it's just static files. Clone the repo and open `index.html` in a browser, or serve it:

```bash
git clone https://github.com/briangaini/vector-siege.git
cd vector-siege
python3 -m http.server 8000
# visit http://localhost:8000
```

## Controls

| Action | Desktop | Mobile |
|---|---|---|
| Move | WASD / Arrow keys, or mouse | Drag anywhere |
| Fire | Automatic (targets nearest enemy) | Automatic |
| Dash | Spacebar | Dash button (bottom-right) |

## Project Structure

```
vector-siege/
├── index.html   # entry point, loads React + game.js
├── game.js      # the full game (compiled from JSX)
└── README.md
```

## License

MIT — see [LICENSE.md](LICENSE.md).

---

Built by [Brian Gaini](https://github.com/briangaini).
