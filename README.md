# 🐍 Snake Game

A sleek, neon-styled Snake game built with pure HTML, CSS, and JavaScript — no frameworks, no dependencies.

![HTML](https://img.shields.io/badge/HTML-100%25-orange?style=flat-square&logo=html5)
![No Dependencies](https://img.shields.io/badge/dependencies-none-brightgreen?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)

---

## 🎮 Play It

Just open `index.html` in any modern browser — that's it.

> **[▶ Live Demo](https://asadullahx4.github.io/snake-game/)** *(enable GitHub Pages to activate this link)*

---

## ✨ Features

- **Neon cyberpunk aesthetic** — animated grid background, scanlines, glowing snake and food
- **Progressive difficulty** — speed and score multiplier increase every 5 food eaten (Level system)
- **Persistent best score** — saved to `localStorage` across sessions
- **Keyboard controls** — Arrow keys or WASD to move, `P` to pause, `R` to restart
- **Mobile D-pad** — on-screen directional buttons appear on small screens
- **Swipe support** — swipe on the canvas to change direction on touch devices
- **Pause / Resume** — mid-game pause with a clean overlay
- **Animated food** — pulsing glow effect on the food item
- **Snake eyes** — the head renders eyes that face the current direction

---

## 🕹️ Controls

| Action | Keyboard | Mobile |
|--------|----------|--------|
| Move Up | `↑` or `W` | D-pad ↑ / Swipe up |
| Move Down | `↓` or `S` | D-pad ↓ / Swipe down |
| Move Left | `←` or `A` | D-pad ← / Swipe left |
| Move Right | `→` or `D` | D-pad → / Swipe right |
| Pause / Resume | `P` | — |
| Restart | `R` | — |

---

## 📁 Project Structure

```
snake-game/
└── index.html   # Everything in one file — HTML, CSS, and JS
```

---

## 🚀 Getting Started

```bash
git clone https://github.com/Asadullahx4/snake-game.git
cd snake-game
open index.html   # or just double-click the file
```

No build step. No npm install. No server required.

---

## 🧠 How It Works

- Rendered on an HTML5 `<canvas>` element using the 2D Context API
- Game loop runs via `setInterval`, with the interval shrinking as the level increases
- Speed formula: `max(50ms, baseInterval - (level - 1) × 12ms)`
- Score per food: `10 × current level`
- Best score is stored in `localStorage` under the key `snakeBest`

---

## 📱 Responsive Design

The canvas and layout adapt to screen size. On screens narrower than 520px, the keyboard hint is hidden and the D-pad controls appear automatically.

---

## 📄 License

MIT — free to use, modify, and distribute.

---

*Made by [Asadullahx4](https://github.com/Asadullahx4)*
