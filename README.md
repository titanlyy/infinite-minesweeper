# 🧨 Infinite Minesweeper

A fully browser-based, procedurally generated Minesweeper game with an infinite scrolling board, sound effects, scoring, leaderboards, and multiplayer rooms (coming soon).

## Play
Open `index.html` in any modern browser, or deploy via [Vercel](https://vercel.com) / [Cloudflare Pages](https://pages.cloudflare.com).

## Features
- ♾️ Infinite procedural board via deterministic seed hashing
- 🎮 Pan, zoom, reveal, flag, and chord mechanics
- 💾 Cloud-ready session save/restore
- 🔊 Sound effects and haptic feedback
- 🌗 Dark, Light, Neon, and High Contrast themes
- 📱 Mobile-first touch controls
- 🏆 Score, streaks, sector bonuses, and leaderboard (Phase 2)
- 🧑‍🤝‍🧑 Private rooms and multiplayer (Phase 3)

## Stack
- Vanilla JS + HTML5 Canvas (no framework dependencies for core game)
- CSS custom properties for design tokens and theming
- Node.js + Express backend (Phase 2)
- WebSockets for multiplayer (Phase 3)

## Project Structure
```
infinite-minesweeper/
├── index.html          # App shell
├── styles/
│   ├── tokens.css      # Design system tokens
│   ├── base.css        # Reset and global styles
│   ├── hud.css         # HUD components
│   ├── modals.css      # Modals and overlays
│   └── themes.css      # Theme variants
├── src/
│   ├── main.js         # App entry point
│   ├── game/
│   │   ├── board.js    # Board generator and chunk manager
│   │   ├── hash.js     # Deterministic mine hashing
│   │   ├── reveal.js   # Reveal, flag, chord, flood-fill
│   │   └── score.js    # Score, streaks, sector bonuses
│   ├── render/
│   │   ├── renderer.js # Canvas renderer
│   │   ├── camera.js   # Pan and zoom
│   │   └── minimap.js  # Mini-map overlay
│   ├── ui/
│   │   ├── hud.js      # HUD updates
│   │   ├── settings.js # Settings drawer
│   │   ├── modals.js   # Tutorial, results, room modals
│   │   └── theme.js    # Theme switcher
│   ├── audio/
│   │   └── sound.js    # Web Audio API sound manager
│   └── utils/
│       ├── storage.js  # LocalStorage / cloud save helpers
│       └── events.js   # Input event handlers
└── assets/
    └── icons/          # SVG icons
```

## Development (browser-based)
1. Open in [GitHub Codespaces](https://github.com/codespaces) or [StackBlitz](https://stackblitz.com)
2. No install needed — pure HTML/CSS/JS for Phase 1
3. Preview by opening `index.html`

## Roadmap
- [x] Phase 1: Core infinite game engine
- [ ] Phase 2: Accounts, leaderboard, daily challenge
- [ ] Phase 3: Multiplayer rooms
- [ ] Phase 4: Cosmetics, daily events
