# 🎮 GPU RUSH — The Indie Dev's Nightmare

A retro arcade browser game where you play as a scrappy indie developer scrambling to collect GPUs while dodging Big Tech corporate agents, firewalls, paywalls, and TOS violations.

Built as a single self-contained HTML file — no frameworks, no build step, no dependencies.

## Gameplay

- **Collect GPUs** to hit each level's quota and advance.
- **Dodge hazards** — firewalls, paywalls, and TOS traps slow you down or steal your progress.
- **Evade corporate agents** — CEO-style sprites that chase you and steal collected GPUs.
- **Fight bosses** — take on NVIDIA, Amazoom, Megasoft, and a final boss. Extra GPUs beyond the quota deal damage.
- **Breaking News events** — mid-game modifiers that shake up spawn rates, speed, or shrink the playfield.
- **Sell-out offers** — take the deal for 2× score (but your run ends) or stay indie and keep going.

## Controls

| Input | Action |
|-------|--------|
| Arrow keys / WASD | Move |
| Touch drag | Move (mobile) |
| Enter / Tap | Advance through title, news, dialogs |
| Y / N | Accept or decline sell-out offers |
| ? button | In-game help |

## Running the Game

Open `index.html` in any modern browser. That's it.

For stricter browser environments (font loading, audio policies), serve the folder with any static server:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Tech Stack

| Layer | Technology |
|-------|------------|
| Rendering | Canvas 2D (320×180 internal, scaled to 960×540 display) |
| Audio | Web Audio API (procedural synthesized sounds) |
| UI | HTML + CSS with CRT-style shell and pixel-art sprites |
| Fonts | Press Start 2P, VT323 (Google Fonts) |
| Persistence | `localStorage` for high score |
| Logic | Vanilla JavaScript, single IIFE |
