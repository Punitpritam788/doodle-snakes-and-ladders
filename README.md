<div align="center">

# 🐍 Doodle Snakes & Ladders 🪜

### The classic race to 100 — hand-drawn on a napkin, rendered in 3D, played in one HTML file.

[![Play](https://img.shields.io/badge/▶_PLAY_NOW-live_demo-ff7a6b?style=for-the-badge&labelColor=2b2a33)](#-quick-start)
[![Single File](https://img.shields.io/badge/single-HTML_file-ffd93d?style=for-the-badge&labelColor=2b2a33)](#-quick-start)
[![Three.js](https://img.shields.io/badge/Three.js-r128-000000?style=for-the-badge&logo=threedotjs&logoColor=white)](https://threejs.org)

![Zero build](https://img.shields.io/badge/build_step-none-brightgreen?style=flat-square)
![Dependencies](https://img.shields.io/badge/dependencies-1-blue?style=flat-square)
![Players](https://img.shields.io/badge/players-1--4-orange?style=flat-square)
![Platform](https://img.shields.io/badge/platform-any_modern_browser-8a63d2?style=flat-square&logo=googlechrome&logoColor=white)
![WebGL](https://img.shields.io/badge/WebGL-powered-990000?style=flat-square&logo=webgl&logoColor=white)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-ff69b4?style=flat-square)
![Made with love](https://img.shields.io/badge/made_with-♥_and_crayons-d62839?style=flat-square)

<br/>

<!-- 🎬 Drop your promo here: drag doodle-snakes-ladders.mp4 into a GitHub issue/PR comment, copy the generated URL, paste it on its own line below -->
<!-- https://github.com/user-attachments/assets/YOUR-VIDEO-ID -->

</div>

---

## ✨ What is this?

**Doodle Snakes & Ladders** turns a childhood classic into a living doodle. The board **draws itself** — grid, coloured tiles, numbers, wriggling snakes and ladders "falling from the sky" — on a crumpled napkin covered in sketches of suns, snails, cats and kites. Pick a pawn, roll the dice, and race to **100**.

No installs. No bundler. No framework. **Just open the file.**

## 🎮 Features

| | |
|---|---|
| 👥 **1–4 players** | Hot-seat with friends, or add 🤖 bots |
| 🐾 **8 doodle pals** | Cactus, sunflower, fox, bee, frog, bunny, bear, penguin |
| 🎲 **Random boards** | Toggle *Random snakes & ladders (harder)* for a fresh layout every game |
| 🏆 **Leaderboards** | Saved in your browser — fewest turns wins |
| 🖍️ **Hand-drawn 3D** | Three.js scene with sketchy, crayon-style textures |
| 🔊 **Sound** | Generated with the Web Audio API — no audio files |
| 🌐 **Online rooms** | Room-based multiplayer when hosted where the room service is available (see note below) |

## 🚀 Quick Start

```bash
git clone https://github.com/<your-username>/doodle-snakes-ladders.git
cd doodle-snakes-ladders
open index.html        # macOS  (Linux: xdg-open · Windows: start)
```

That's it. Or serve it locally:

```bash
npx serve .
```

> **Note:** the game loads Three.js (r128) and Google Fonts from a CDN, so you need an internet connection on first load.

## 🕹️ How to Play

1. Choose **2–4 players** and set each as 🙂 Human or 🤖 Bot.
2. Pick a pawn for everyone.
3. Hit **Let's play!** and press **Roll**.
4. 🪜 Land on a ladder's foot → **climb up**. 🐍 Land on a snake's head → **slide down**.
5. First pawn to square **100** wins. 🎉

## 🛠️ Tech

- **Three.js r128** — 3D board, pawns, dice and camera
- **Vanilla JS + CSS** — all UI and game logic in a single file
- **Web Audio API** — procedural sound effects
- **localStorage** — nickname and leaderboards

## 🎬 Promo Video

A 45-second promo was produced with [claude-code-video-toolkit](https://github.com/digitalsamba/claude-code-video-toolkit) (Remotion) using footage recorded straight from the game.

## 🌐 About online play

Online rooms rely on a room service that is available when the page is opened inside **claude.ai** as a signed-in user. Elsewhere, the *Play online* button stays hidden and the game works fully offline-style with local players and bots.

## 🤝 Contributing

Ideas welcome — new pawns, board themes, dice skins, a mobile touch pass, or a self-hosted multiplayer backend. Fork, branch, PR. 🖍️

## 📄 License

MIT — doodle freely.

<div align="center">

**If this made you smile, drop a ⭐ — it feeds the snakes.** 🐍

</div>
