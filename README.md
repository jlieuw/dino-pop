# 🦕 Dino-Pop!

A prehistoric **bubble-shooter** built in a single, dependency-free HTML file. Aim the dino's slingshot, launch colored eggs into the hanging nest, and match **3 or more** of the same color to pop them. Knock eggs loose from the cluster and they drop for bonus points — but don't let the nest reach the bottom, or Mama Bronto stomps the screen!

> Inspired by the classic match-3 bubble-shooter genre (Puzzle Bobble / Bust-a-Move style). This is an original, from-scratch implementation — not affiliated with or endorsed by any existing game or trademark.

## ▶️ Play

Just open `index.html` in any modern browser. No build step, no install, no dependencies.

Or play it locally with any static server, e.g.:

```bash
npx serve .
```

## 🎮 Controls

| Action | Input |
| ------ | ----- |
| Aim    | Move the mouse |
| Launch egg | Click or **Space** |
| Pause  | **P** |
| Toggle sound | 🔊 button (top-right) |

Touch is supported too: drag to aim, lift to fire.

## ✨ Features

- Hexagonal egg grid with proper offset-row neighbor matching
- Bounce-aware aiming trajectory with a ghost target preview
- Flood-fill match detection + falling disconnected clusters
- The nest **descends** over time, ramping up difficulty
- 🦅 **Whirley** the pterodactyl periodically flies past and pushes the nest down
- 💣 Combo **bomb egg** power-up that clears a wide radius
- 🦕 **Mama Bronto** stomp game-over animation
- Levels with more colors and faster descent
- High-score saved in `localStorage`
- WebAudio sound effects, particle bursts, screen shake, score popups

## 🛠️ Tech

Plain HTML5 `<canvas>` + vanilla JavaScript. Everything — rendering, physics, audio, and game logic — lives in `index.html`.

## 📄 License

[MIT](LICENSE)
