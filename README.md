 <div align="center">

# 🐍 Doodle Snakes & Ladders 🪜
### A classic board game, reimagined as a playful, hand-drawn 3D browser experience.

[![Play the Game](https://img.shields.io/badge/PLAY_THE_GAME-GitHub_Pages-ff7a6b?style=for-the-badge)](https://punitpritam788.github.io/doodle-snakes-and-ladders/)
[![GitHub Stars](https://img.shields.io/github/stars/Punitpritam788/doodle-snakes-and-ladders?style=for-the-badge&logo=github&color=ffd43b)](https://github.com/Punitpritam788/doodle-snakes-and-ladders/stargazers)
[![GitHub Issues](https://img.shields.io/github/issues/Punitpritam788/doodle-snakes-and-ladders?style=for-the-badge&logo=github)](https://github.com/Punitpritam788/doodle-snakes-and-ladders/issues)
[![Last Commit](https://img.shields.io/github/last-commit/Punitpritam788/doodle-snakes-and-ladders?style=for-the-badge)](https://github.com/Punitpritam788/doodle-snakes-and-ladders/commits/main)

[![HTML5](https://img.shields.io/badge/HTML5-Single_File-E34F26?style=flat-square&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-Custom_UI-1572B6?style=flat-square&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla-F7DF1E?style=flat-square&logo=javascript&logoColor=222)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Three.js](https://img.shields.io/badge/3D-Three.js-black?style=flat-square&logo=threedotjs&logoColor=white)](https://threejs.org/)
[![No Build Step](https://img.shields.io/badge/Build-No_Build_Step-4c956c?style=flat-square)](#-run-locally)

**One notebook-inspired board. Eight character designs. Snakes, ladders, silly surprises, and a little browser magic.**

[🎮 Play the game](https://punitpritam788.github.io/doodle-snakes-and-ladders/) · [💻 Source repository](https://github.com/Punitpritam788/doodle-snakes-and-ladders) · [🐛 Report a bug](https://github.com/Punitpritam788/doodle-snakes-and-ladders/issues)

</div>

---

## ✨ The idea

What if a familiar board game looked as though somebody had sketched it in the margins of a notebook?

**Doodle Snakes & Ladders** turns the classic race from square 1 to square 100 into a browser-based game with a hand-drawn visual identity. The board uses imperfect outlines, notebook-inspired panels, colourful illustrated characters, and small animated details. Underneath that playful style is a Three.js scene with moving pawns, a 3D dice roll, turn logic, sound effects, and a local record system.

The project is intentionally lightweight: the game is delivered as one HTML file, with CSS and JavaScript included rather than a separate front-end build pipeline. It is a creative-coding experiment in making a small game feel expressive without requiring a large asset bundle or framework-heavy setup.

> **Play link:** The badge above points to the expected GitHub Pages URL. For the demo to work, commit the game source as `index.html` and enable GitHub Pages for the repository. Check the link in a private/incognito window before promoting it.

## 🧩 At a glance

| | Details |
|---|---|
| **Genre** | Casual, turn-based board game |
| **Board** | 100 squares with snakes and ladders |
| **Players** | 2–4 seats per match; seats can be human-controlled or bot-controlled |
| **Character selection** | 8 illustrated pawn designs |
| **Rendering** | Three.js scene with Canvas-generated textures and artwork |
| **Sound** | Procedurally generated effects using the Web Audio API |
| **Persistence** | Browser `localStorage` for local settings, records, and scores |
| **Runtime** | Modern browser with WebGL support |
| **Build tools** | No npm install or bundling step required |
| **External resources** | Three.js r128 and Google Fonts are loaded from CDNs |

## 🎮 Features

### ✏️ A hand-drawn visual language

- Sketchbook-inspired colours, paper textures, rough outlines, and doodled UI elements.
- A board whose numbers, snakes, ladders, and character details are drawn through Canvas routines.
- An animated opening sequence that reveals the board, numbers, snakes, ladders, and decorative doodles.
- Small ambient illustrations—such as a butterfly, bird, plane, fish, snail, and twinkling star—that help the scene feel alive.
- Animated transitions and playful text feedback when turns change, a snake catches a pawn, a ladder helps a player, or someone wins.

### 🧊 A Three.js board scene

Three.js handles the 3D presentation, including the game board, pawns, dice, movement, and scene effects. Canvas-generated textures give the objects their illustrated look, keeping the art style consistent without relying on a directory full of imported image files.

### 🎲 Classic rules with a small twist

- Roll a virtual dice and move along the numbered path.
- Land at the foot of a ladder to climb forward.
- Land on a snake to slide backward.
- Rolling a six grants another roll.
- An exact roll is required to finish on square 100; an overshoot does not move the pawn.
- Turn indicators make it easier to see whose move is next.

### 👥 Flexible player setup

Set up a match with 2, 3, or 4 player seats. Each seat can be configured as a human or a computer-controlled opponent. Human players can enter a short display name, and each seat can choose from the available illustrated pawn designs.

### 🖍️ Eight pawn designs

Players can choose from eight distinctive character illustrations. The selected pawns appear in the 3D scene as sticker-like pieces, with name labels to make a multi-player game easier to follow.

### 🌪️ Optional harder board mode

The setup includes a **Random snakes & ladders (harder)** option. It changes the board configuration for a less predictable run, offering a different challenge from the standard layout.

### 🔊 Generated sound effects

The game creates short tones through the browser's Web Audio API rather than depending on a folder of prerecorded audio. Use the sound toggle to mute or enable effects. Browsers generally require a user interaction before audio can begin.

### 🏆 Results, stats, and local leaderboards

The game records local statistics such as games played, wins, best winning turn count, snakes encountered, and ladders climbed. A local leaderboard interface can show saved results for the current browser/device and distinguish classic and random-board runs.

Local records are stored in `localStorage`. They are not automatically synchronised between browsers or devices, and clearing browser data may remove them.

### 🧪 Online-play and global-score integration status

The source contains an online-room interface with room-code, ready-state, and random-match flows, as well as hooks for global scoring. However, the supplied standalone HTML does **not** include a fully configured network/lobby provider. These flows should be treated as integration scaffolding until a compatible provider is wired in and end-to-end tests have confirmed that they work in the deployed environment. Local turn-based play does not depend on that integration.

The GitHub-score flow also opens an issue form for a result and expects a compatible repository/workflow setup; it is not a fully automated global leaderboard out of the box.

## 🕹️ How to play

1. Open the deployed game or run it locally using the instructions below.
2. Choose the number of player seats: 2, 3, or 4.
3. For each seat, select **Human** or **Bot**, provide a name when applicable, and pick a pawn.
4. Optionally switch on **Random snakes & ladders (harder)**.
5. Start the match and press **Roll!** on your turn. During active gameplay, the interface also supports keyboard and pointer/tap interaction to trigger a roll.
6. Watch your pawn hop between squares. Ladders move you forward; snakes send you back.
7. Try to reach square 100 with an exact roll. A six earns an extra roll.
8. After the game, review the result and local statistics, then start another round.

### Default board connections

These are the board connections defined in the supplied source for the standard setup.

| Type | Start | Destination |
|---|---:|---:|
| 🪜 Ladder | 1 | 38 |
| 🪜 Ladder | 4 | 14 |
| 🪜 Ladder | 8 | 30 |
| 🪜 Ladder | 21 | 42 |
| 🪜 Ladder | 28 | 76 |
| 🪜 Ladder | 50 | 67 |
| 🪜 Ladder | 71 | 92 |
| 🪜 Ladder | 80 | 99 |
| 🐍 Snake | 98 | 78 |
| 🐍 Snake | 95 | 56 |
| 🐍 Snake | 87 | 36 |
| 🐍 Snake | 62 | 18 |
| 🐍 Snake | 48 | 26 |
| 🐍 Snake | 32 | 10 |

## 🧰 Technology and implementation

| Technology | Role in the project |
|---|---|
| **HTML5** | Game shell, overlay panels, buttons, player setup, results, and leaderboard UI |
| **CSS3** | Sketchbook styling, responsive layout, transitions, animated labels, and visual hierarchy |
| **Vanilla JavaScript** | Game state, turn progression, rules, CPU turns, UI updates, save/load, and event handling |
| **Three.js r128** | 3D scene, board, dice, pawns, camera, and animation loop |
| **Canvas 2D API** | Procedural board artwork, number lettering, pawn textures, doodles, and texture generation |
| **Web Audio API** | Short synthesised sound effects for rolls, movement, and win/lose feedback |
| **`localStorage`** | Local preferences, nickname/player configuration, and game records |

### How the game is organised

The single HTML document contains three broad layers:

1. **Interface layer:** HTML elements and CSS overlays handle player setup, sound controls, turn indicators, messages, results, and leaderboard panels.
2. **Rendering layer:** Three.js renders the scene. Canvas helpers draw visual textures and character art for use in the 3D world.
3. **Game-state layer:** JavaScript tracks player positions, turns, dice results, snakes, ladders, bot turns, winning conditions, and local persistence.

Keeping these layers together in one file reduces setup friction for a small browser experiment. It also means the project would benefit from modularisation if it grows significantly.

## 🚀 Run locally

There is no package installation or front-end build command. The supplied game HTML can be run directly in a modern browser, or served locally for a more realistic website workflow.

### Option A — Open the file

1. Download the game HTML from the project package.
2. Rename it to `index.html` if necessary.
3. Open it in a current browser such as Chrome, Edge, Firefox, or Safari with WebGL enabled.
4. Allow an internet connection for the CDN-hosted Three.js library and Google Fonts.

### Option B — Use a local static server

With Python installed, put `index.html` in a folder and run:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

On some systems, the command may be `python3 -m http.server 8000`.

### Option C — Publish with GitHub Pages

1. Commit the supplied game file to the root of this repository with the exact name `index.html`.
2. Commit this README as `README.md`.
3. Open the repository's **Settings → Pages**.
4. Under the build/deployment source, choose **Deploy from a branch**.
5. Select the `main` branch and `/ (root)` folder, then save.
6. Wait for the deployment to complete in the Pages panel.
7. Open `https://punitpritam788.github.io/doodle-snakes-and-ladders/` in a private/incognito window and verify that the game loads, that the dice can roll, and that sound can be muted.

If you already deploy from another branch or workflow, retain that setup and update the instructions to match it.

## 📂 Repository layout

The game itself is designed to remain a single-file browser experience:

```text
doodle-snakes-and-ladders/
├── index.html     # Complete browser game (HTML, CSS, JavaScript)
└── README.md      # Project overview, setup, rules, and contribution guide
```

The social post, article, and publishing guide delivered with this package are optional authoring documents; they do not need to be committed to the game repository.

## 🧭 Known limitations and honest status

- **The game source must be committed:** GitHub Pages needs the actual HTML entry point in the repository. A README alone cannot publish the game experience.
- **Online mode needs a provider:** Room and matchmaking interface code exists, but the standalone file does not configure the lobby/network service by itself.
- **Global leaderboards are not standalone by default:** the global score hooks rely on host-provided integration, while local/device records work through browser storage.
- **External CDN dependency:** Three.js and Google Fonts are fetched over the internet. A network restriction may prevent those resources from loading.
- **Local progress is browser-specific:** stats and settings live in `localStorage` and do not automatically sync between devices.
- **No automated test suite is included:** gameplay should be manually tested in the browsers and screen sizes you intend to support.
- **No license file is supplied in the current repository:** add a license before inviting people to reuse or redistribute the code.

## 🔧 Troubleshooting

| Problem | Things to check |
|---|---|
| The page is blank or the 3D scene does not appear | Confirm WebGL is enabled, your browser is up to date, and the Three.js CDN is reachable. Open DevTools → Console for runtime errors. |
| Fonts look different | Google Fonts may be blocked or unavailable; the CSS includes fallback fonts. |
| No sound plays | Interact with the page first, check that the mute button is not enabled, and check system/browser volume. Some browsers gate audio until a gesture occurs. |
| The Play link does not load | Confirm `index.html` is in the repository root, GitHub Pages is enabled, and the latest deployment succeeded. |
| Local stats disappeared | Browser data may have been cleared, private browsing may discard storage, or you may have opened the page under another origin/device. |
| Online room or global leaderboard fails | Treat it as unconfigured until the corresponding lobby/database provider is connected and verified. Local play should remain the first debugging target. |

## 🛣️ Roadmap ideas

These are possible follow-up improvements rather than claims about features already shipped:

- [ ] Add authentic gameplay screenshots or a short GIF to the repository.
- [ ] Wire up and document a supported, secure online-lobby provider; test joining, leaving, disconnects, and turn synchronisation.
- [ ] Decide on a reliable global leaderboard storage model and document abuse prevention and data handling.
- [ ] Add automated tests for movement, exact-roll-to-100, extra rolls, snake/ladder transitions, and win conditions.
- [ ] Review keyboard accessibility, visible focus states, reduced-motion preferences, and contrast.
- [ ] Test mobile layouts and performance on real devices.
- [ ] Add a LICENSE file and release/changelog notes.
- [ ] Consider splitting rendering, game rules, and UI into modules if the project grows.

## 🤝 Contributing

Feedback and focused contributions are welcome.

1. Open an [issue](https://github.com/Punitpritam788/doodle-snakes-and-ladders/issues) with reproduction steps or a clear feature request.
2. Fork the repository and create a branch for your change.
3. Keep changes focused and preserve the hand-drawn visual identity unless a redesign is intentional.
4. Test the gameplay path manually: start a match, roll, trigger a snake and ladder, verify turn progression, and finish a game.
5. Include before/after screenshots or a short clip for visual changes.
6. Open a pull request explaining what changed, why it matters, and how you tested it.

## 📸 Screenshots and gameplay clips

A real screenshot or short gameplay recording would make this README even more compelling. Capture the actual game after publishing `index.html`, then add the files under an `assets/` directory and embed them here. Suggested captures:

- **Main menu:** player count, pawn choices, and random-board option.
- **Mid-game:** the 3D board, player markers, and dice.
- **Movement moment:** a snake slide or ladder climb.
- **Results screen:** winning animation and local stats.

Use compressed images or a short GIF so the README remains quick to load. Do not use concept art that does not match the build.

## 👨‍💻 Creator

Created by **Punit Pritam Mohanty**.

- GitHub profile: [@Punitpritam788](https://github.com/Punitpritam788)
- Project repository: [doodle-snakes-and-ladders](https://github.com/Punitpritam788/doodle-snakes-and-ladders)
- Issues and feedback: [Open a GitHub issue](https://github.com/Punitpritam788/doodle-snakes-and-ladders/issues)

If you try it, I would love feedback on the visual direction, game feel, and which feature deserves the next improvement. A ⭐ on the repository is appreciated if you find the experiment interesting.

---

<div align="center">

**Roll the dice. Follow the doodles. Try not to get bitten.** 🐍🎲

*Made with ✏️, JavaScript, and a little browser magic.*

</div>
