<div align="center">

# ⚡ CHRONOBOOM 3D
### Chrono-Cards of the Abyss — a neon 3D roguelike deckbuilder & survival game

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/Vanilla_JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=111111)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Three.js](https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=threedotjs&logoColor=white)](https://threejs.org/)
[![Web Audio API](https://img.shields.io/badge/Web_Audio_API-8A2BE2?style=for-the-badge&logo=webaudio&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)
[![Browser Game](https://img.shields.io/badge/PLAYABLE-Browser_Game-00D9FF?style=for-the-badge&logo=googlechrome&logoColor=black)](https://punitpritam788.github.io/chronoboom-3d/)

**🎮 [PLAY CHRONOBOOM 3D](https://punitpritam788.github.io/chronoboom-3d/)** · **[View Source](https://github.com/Punitpritam788/chronoboom-3d)**

*A single-page browser game where every card is a weapon, every wave is a test of your build, and every run brings you closer to the Dreadnought.*

</div>

> **Publishing note:** The Play link above is the intended GitHub Pages URL for the repository `chronoboom-3d`. It becomes live after this repository is created under `Punitpritam788`, the game is uploaded as `index.html` in the repository root, and GitHub Pages is enabled. Until then, the URL may return a 404.

---

## 🌌 The Mission

The Chrono-Cataclysm has torn reality apart and pulled entire worlds into a timeless Singularity. You are **AETHER-MK4**, a Valkyrie Spec-Ops mecha that crash-landed in an abyss of shattered timelines. The mysterious **Chrono-Cards** drifting through the arena turn into reality-warping attacks, defenses, and mobility abilities. Their power awakens the ancient **Dreadnought**—and your survival run becomes a fight to restore the timeline.

CHRONOBOOM 3D combines real-time 3D arena combat with tactical, card-driven choices. Move through incoming threats, manage your energy, experiment with card combinations, collect relics, and upgrade your deck between waves.

## ✨ Key Features

- **Three.js 3D arena** — a neon-lit combat space with a controllable camera, animated combat effects, and a central mecha protagonist.
- **Roguelike deckbuilding** — play a hand of attack, skill, and power cards; then choose a new card reward after clearing a wave.
- **Eight-wave run** — survive escalating enemy pressure and face the Dreadnought boss encounters.
- **Chrono-Card abilities** — combine effects such as meteor strikes, chain lightning, area shockwaves, shields, stasis, and mobility boosts.
- **Relics and upgrades** — earn shards, collect survival relics, and forge upgrades to strengthen cards.
- **Mecha skins and arena themes** — customize the player chassis and visual theme.
- **Story intro cutscene** — four narrative acts introduce AETHER-MK4, the Chrono-Cards, and the Dreadnought.
- **Victory and defeat finales** — separate ending sequences give the run a narrative conclusion.
- **Combat HUD and run summary** — monitor health, shield, mana, XP, wave progress, kills, and cards played.
- **Procedural sound effects** — synthesized in the browser through the Web Audio API; no separate audio files are needed for the built-in sound effects.
- **Desktop and touch controls** — keyboard/mouse support plus an on-screen movement joystick for small screens.
- **Single-file game entry point** — the core game is delivered through `index.html`; no Node.js install or frontend build step is needed.

## 🕹️ Controls

| Action | Control |
|---|---|
| Move | `W`, `A`, `S`, `D` or arrow keys |
| Play a card | Click a playable card or press its displayed number (`1`–`5`) |
| Cycle / overclock the hand | `Space` |
| Orbit the 3D camera | Right-click and drag |
| Move on touch devices | Use the on-screen joystick |
| Story and ending scenes | Use the **Story** and **Endings** buttons in the HUD |
| Customize your mecha | Open **Skins** |
| Inspect your deck and route | Open **Deck** or **Map** |

> **Tip:** Read the card's energy cost and effect before playing it. Use defensive and mobility options to stay alive while setting up stronger attack combinations.

## 🔁 Core Gameplay Loop

1. **Enter the arena.** Follow the origin cutscene or skip directly to combat.
2. **Move and survive.** Dodge enemies while monitoring health, shield, and mana.
3. **Play Chrono-Cards.** Use attacks, defenses, and mobility skills to control the arena.
4. **Clear a wave.** Earn experience, shards, and access to the next tactical choice.
5. **Draft or upgrade.** Add one of the offered cards, take a survival bonus, or forge an upgrade when available.
6. **Build synergies.** Match card effects with relic bonuses and your preferred play style.
7. **Confront the Dreadnought.** Reach the later waves and try to restore the timeline.

## 🛠️ Built With

- **HTML5** for the page and game interface
- **CSS3** for the responsive neon HUD, card presentation, transitions, and cinematic overlays
- **Vanilla JavaScript** for game state, combat systems, wave progression, card/relic logic, UI, and cutscene sequencing
- **Three.js r128** for 3D rendering
- **Tailwind CSS CDN** for utility styling
- **Font Awesome** for interface icons
- **Google Fonts** using Orbitron and Rajdhani for the sci-fi display style
- **Web Audio API** for synthesized sound effects and cinematic tones

The HTML imports some libraries and fonts from CDNs, so an internet connection is required when loading the hosted game.

## 🚀 Run Locally

### Option 1 — Open the file

Download `index.html` and open it in a modern browser. If your browser blocks any functionality when opened as a local file, use the local-server option below.

### Option 2 — Start a lightweight local server

You do not need to install a JavaScript package manager or build the frontend.

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

Make sure `index.html` is in the directory from which you start the server. The game loads its external library dependencies from CDNs.

## 🌐 Publish on GitHub Pages

1. Create a public GitHub repository named **`chronoboom-3d`** under `Punitpritam788`.
2. Upload `index.html`, `README.md`, and the `assets/` folder to the **repository root**.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`, then save.
6. Wait for the Pages deployment to finish. Your expected public URLs are:
   - **Play:** https://punitpritam788.github.io/chronoboom-3d/
   - **Repository:** https://github.com/Punitpritam788/chronoboom-3d

If the Play link does not open immediately, check the Pages deployment status and confirm the entry file is named exactly `index.html` in the repository root.

## 📂 Repository Structure

```text
chronoboom-3d/
├── index.html                  # Complete single-file browser game
└── README.md                   # Project overview and setup guide
```

The separate 50-second gameplay explainer can be attached directly to a LinkedIn post. To keep the Git repository lightweight, the MP4 is not bundled here.

## 🎯 Project Goals

CHRONOBOOM 3D is a personal browser-game project exploring how a single HTML entry point can bring together 3D rendering, tactical deckbuilding, survival progression, responsive interface design, custom sound, and story-driven presentation without a separate build pipeline.

It is an experimental indie game project, not a claim of commercial or AAA production readiness. Feedback on game balance, card synergy, accessibility, performance, and feel is welcome.

## 🧪 Feedback & Contributions

Found a bug, noticed a balancing issue, or have an idea for a new Chrono-Card or relic? Open a GitHub Issue with:

- Your browser and device
- What you were doing when the issue occurred
- What you expected to happen
- What actually happened (screenshots or a short clip help)

Suggestions for cards, enemy patterns, HUD usability, and story presentation are especially welcome.

## 👨‍💻 Creator

Created by **Punit Pritam Mohanty**.

- GitHub: [@Punitpritam788](https://github.com/Punitpritam788)

## 📌 GitHub Topics

Suggested repository topics: `threejs`, `javascript`, `html5-game`, `webgl`, `browser-game`, `roguelike`, `deckbuilder`, `indie-game`, `game-development`, `web-game`, `single-file-html`, `web-audio-api`, `game-design`, `survival-game`, `github-pages`.

## 📄 License

No license file is included in this starter package. Add a `LICENSE` file before describing the project as open source or granting reuse rights. A public repository does not, by itself, grant permission to copy or redistribute the code.

---

<div align="center">

**DRAW YOUR HAND. SURVIVE THE WAVES. BREAK THE TIMELINE.** ⚡

**[▶ PLAY CHRONOBOOM 3D](https://punitpritam788.github.io/chronoboom-3d/)**

</div>
