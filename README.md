<div align="center">

# 🐍 Doodle Snakes & Ladders 🪜
### A classic board game, reimagined as a hand-drawn 3D doodle.

[![Live Demo](https://img.shields.io/badge/🎮_Play_the_Game-Live_Demo-ff7a6b?style=for-the-badge)](https://punitpritam788.github.io/doodle-snakes-and-ladders/)
[![GitHub Repo](https://img.shields.io/badge/GitHub-Source_Code-24292f?style=for-the-badge&logo=github)](https://github.com/Punitpritam788/doodle-snakes-and-ladders)
[![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla-F7DF1E?style=for-the-badge&logo=javascript&logoColor=222)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Three.js](https://img.shields.io/badge/3D-Three.js-000000?style=for-the-badge&logo=threedotjs&logoColor=white)](https://threejs.org/)
[![HTML5](https://img.shields.io/badge/HTML5-Single_File-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-Custom_UI-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)

**📄 One HTML file. ✏️ A paper-and-pencil personality. 🎲 Plenty of chaotic climbs and slides.**

[▶ Play Now](https://punitpritam788.github.io/doodle-snakes-and-ladders/) · [Explore the Code](https://github.com/Punitpritam788/doodle-snakes-and-ladders) · [Report a Bug](https://github.com/Punitpritam788/doodle-snakes-and-ladders/issues)

</div>

---

## ✨ What is Doodle Snakes & Ladders?

Remember doodling a board game in the margins of a notebook? **Doodle Snakes & Ladders** brings that sketchbook energy to the browser. It takes the familiar race from square 1 to square 100 and dresses it in a hand-drawn visual style, a Three.js-powered 3D scene, expressive characters, animated feedback, and a playful interface.

The goal is simple: make a familiar game feel like a tiny world someone lovingly drew into existence.

## 🎮 Features

| Feature | What you get |
| --- | --- |
| ✏️ **Sketchbook art direction** | Wobbly outlines, notebook-paper styling, playful colours, and doodle-inspired UI elements. |
| 🧊 **3D board scene** | Browser-rendered 3D presentation powered by Three.js. |
| 🎲 **Classic 100-square race** | Roll, move, climb ladders, dodge snakes, and try to reach the finish. |
| 👥 **1–4 player setup** | Configure a small group game or include computer-controlled opponents. |
| 🧸 **Illustrated pawns** | Sticker-like character designs give the board its own personality. |
| 🔊 **Sound controls** | Toggle generated game sounds on or off. |
| 🏆 **Results and local records** | Results UI and browser-saved statistics for games, wins, best turns, snakes encountered, and ladders climbed. |
| 📊 **Leaderboard interface** | Dedicated leaderboard screens and categories are included in the interface. |
| 📱 **Responsive UI** | Layout adjustments and touch-friendly interaction for smaller screens. |
| ⚡ **Lightweight setup** | The game source is designed around a single HTML document—no frontend build step. |

> **Online-play note:** The interface includes an online-play flow. Verify the networking path in the published build before advertising live multiplayer as fully operational.

## 🕹️ How to Play

1. Open the [live game](https://punitpritam788.github.io/doodle-snakes-and-ladders/).
2. Choose the number of players and configure the available player options.
3. Start the game.
4. Roll when it is your turn. Follow the on-screen prompts for supported tap or keyboard interactions.
5. Land on a ladder to climb ahead—or on a snake to slide backwards.
6. Race toward square **100** and celebrate the winner!

A lead can disappear after one particularly unfortunate snake encounter. That's part of the fun. 🐍

## 🧰 Built With

- **HTML5** — structure and single-file delivery.
- **CSS3** — responsive layout, the hand-drawn visual language, transitions, and animations.
- **Vanilla JavaScript** — game state, turn flow, board logic, drawing, local records, and sound generation.
- **Three.js (r128)** — 3D rendering in the browser.
- **Canvas 2D API** — procedural board details and character artwork/textures.
- **Web Audio API** — lightweight synthesized sound effects.
- **localStorage** — remembers local preferences and game statistics in the same browser.

### 🧩 How it is put together

The core experience is intentionally lightweight: markup, styles, and JavaScript are packaged in one HTML document. Canvas routines generate the sketch-like board and character textures; Three.js renders the board scene and game pieces; browser storage preserves local statistics and the sound preference.

## 🚀 Run Locally

No package installation or build command is needed for the single-file game.

### Option 1 — Open the HTML file

1. Download the game HTML file from the project files.
2. Open it in a modern browser.
3. Keep an internet connection available if the page needs to load the externally hosted Three.js library or Google Fonts.

### Option 2 — Clone with Git

```bash
git clone https://github.com/Punitpritam788/doodle-snakes-and-ladders.git
cd doodle-snakes-and-ladders
```

Open the main HTML file in a browser. You can also serve the folder using any simple static web server.

## 📁 Repository Layout

The public repository currently contains the README only. The game source is available as a separate HTML file in the project workflow; add/commit that file to the repository so visitors can clone and run the complete game.

Recommended layout:

```text
doodle-snakes-and-ladders/
├── index.html       # Complete single-file game
└── README.md        # Project overview and instructions
```

Once `index.html` is committed, the published GitHub Pages link can serve as the direct playable build.

## 🌱 Ideas for Future Improvements

- Add real screenshots or a short gameplay GIF near the top of this README.
- Verify and document the online multiplayer flow end to end.
- Add an accessibility pass for keyboard navigation, contrast, and reduced-motion preferences.
- Add smoke tests for core turns, snake/ladder movement, and the win condition.
- Publish tagged releases and keep a changelog for notable updates.

## 🤝 Contributing

Ideas, bug reports, and improvements are welcome.

1. Open an [issue](https://github.com/Punitpritam788/doodle-snakes-and-ladders/issues) describing the idea or problem.
2. Fork the repository and create a focused branch.
3. Make your changes and test the game in a browser.
4. Open a pull request with a clear summary and screenshots or a short clip for visual changes.

## 📸 Help the README stand out

A real gameplay capture would make this page even more compelling. Add a compressed GIF, screenshot, or short demo clip taken from the actual game, then embed it here. Avoid stock artwork so people see the real project they are about to play.

## 👨‍💻 Creator

Created by **Punit Pritam Mohanty**.

- GitHub: [@Punitpritam788](https://github.com/Punitpritam788)
- Repository: [doodle-snakes-and-ladders](https://github.com/Punitpritam788/doodle-snakes-and-ladders)

If the project made you smile, consider ⭐ starring the repository and sharing feedback!

---

<div align="center">

**Roll the dice. Follow the doodles. Try not to get bitten.** 🐍🎲

Made with ✏️ and a little browser magic.

</div>
