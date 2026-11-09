# PlayGround

<!-- omgithub:readme:start -->
## 🚀 Build, play, and remix with OMGithub

**Created using [OMGithub.com](https://go.ondev.store/).**

[![OMGithub](https://img.shields.io/badge/OMGithub-Open%20project-orange?style=for-the-badge)](https://go.ondev.store/crunchyrollpremium497-glitch/PlayGround)
[![GitHub](https://img.shields.io/badge/GitHub-Source-181717?logo=github&style=for-the-badge)](https://github.com/crunchyrollpremium497-glitch/PlayGround)

- 🎮 [Open the project](https://go.ondev.store/crunchyrollpremium497-glitch/PlayGround).
- ✨ [Remix this project](https://go.ondev.store/crunchyrollpremium497-glitch/PlayGround?remix=1).
- 💻 [Explore the source](https://github.com/crunchyrollpremium497-glitch/PlayGround).
- 🛠️ [Check build runs](https://github.com/crunchyrollpremium497-glitch/PlayGround/actions).
- 🐛 [Report an issue](https://github.com/crunchyrollpremium497-glitch/PlayGround/issues).
- 👤 [Explore the creator's projects](https://go.ondev.store/crunchyrollpremium497-glitch).
- 🌍 [Create with OMGithub](https://go.ondev.store/).
<!-- omgithub:readme:end -->

# CHITTAGONG LIFE — City Stories

A small, playable **Three.js browser prototype** set in Chattogram, Bangladesh. The current vertical slice starts in Muradpur and focuses on a neighborhood café, light free-roam exploration, and an optional delivery.

## Run locally

Serve this folder over HTTP (ES modules and the Three.js CDN import do not work reliably from `file://`), then open the local address in a modern browser. For example:

```bash
python3 -m http.server 3000
```

Open <http://localhost:3000>. An internet connection is needed to load Three.js and the web fonts from their CDNs.

## Controls

- **WASD / arrow keys:** move; **Shift:** run; **Space:** hop
- **E:** interact; **M:** open or close the full map
- **Drag the world:** orbit the camera; **mouse wheel:** adjust camera distance
- On narrow/mobile layouts, use the on-screen joystick, **RUN**, and interaction buttons.

## Implemented in this prototype

- Five named neighborhood destinations, a compact city guide, current-district indicator, and full-map district navigation.
- Third-person walking, running, camera orbit, simple pedestrians and traffic, and enter/exit interactions for nearby vehicles.
- A purchasable, enterable Muradpur café with stock, staffing, upgrades, customer satisfaction, and time-based income and expenses.
- An optional delivery activity with a destination marker, completion reward, and completion count.
- A cycling weather display with a lightweight rain effect and ambient audio toggle.
- Local-device save/load via `localStorage`, including wallet, café/economy, clock, active delivery, and player position. This is not cloud or account-backed storage.
- Responsive touch-control layout. The 390×844 mobile viewport was checked for visible controls and horizontal overflow.

## Prototype status and limitations

This is an incremental browser vertical slice, **not a finished open-world game and not an Unreal Engine 5 production build**. The map and districts are compact representations; interactions and vehicle behavior are intentionally simple. The game does not yet include a deep quest/story system, combat, full-scale city simulation, robust driving physics, online multiplayer, cloud saves, or production-ready authored assets and audio. These systems should be treated as future work, not as existing features.

## Validation notes

The current browser check covered café entry/exit and business/delivery flows, explicit save/load and reload persistence, map opening/closing and district selection, keyboard movement, and the mobile layout. `node --check game.js` passes. Save data is stored in the browser under `chittagong-life-save`; clearing site storage removes it.
