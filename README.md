# Tournament Arena 🎮

An original, single-file **UT99-style arena deathmatch** that runs entirely in your browser. A fan-made homage to the classic 1999 arena shooters — all code, art, sounds, and the map are procedural and original. No game assets, no installs: one HTML file.

**Play:** just open `index.html` in any modern desktop browser (needs internet on first load to fetch three.js from a CDN). Wired and **Bluetooth controllers are fully supported**, including menu navigation and rumble — and pads with unusual layouts (like the Amazon Luna Controller) get a guided calibration wizard.

## Features

- **Map "ARENA-99"** — a symmetric arena with a central deck, twin side platforms, two towers, jump pads, bridges, and lava pits
- **5 weapons** — Impact Hammer, Enforcer, Shock Rifle (beam + ball + the classic **shock combo**: hit your own ball with the beam), Rocket Launcher, Flak Cannon (bouncing shards)
- **Movement** — WASD, jump, double jump, and double-tap-direction dodge
- **Bots** — 1–6 opponents across three skill tiers (Novice / Adept / Masterful) with A* pathfinding, item hunting, and range-appropriate weapon choice
- **Items** — health vials, kegs, armor (absorbs 60%), damage amp, weapons, and ammo, all on respawn timers
- **HUD** — kill feed, streak announcer (FIRST BLOOD… MONSTER KILL), scoreboard (Tab)
- **Gamepad** — pair a Bluetooth pad, press any button on it, and go: full menu navigation, sticks move/look, triggers fire, dual-rumble feedback (toggleable)
- **Controller calibration** — pads that report a non-standard button/axis layout are flagged on the title screen; a guided 16-step wizard (buttons, triggers, d-pad, sticks) learns the physical layout, saves it per controller in your browser, and applies it automatically every session. An INVERT LOOK Y toggle is right next to the CALIBRATE button. A live input monitor shows exactly what the game sees from your pad.

## Controls

| Action | Keyboard | Gamepad |
| --- | --- | --- |
| Move | WASD | Left stick |
| Look | Mouse | Right stick |
| Fire / Alt-fire | LMB / RMB | RT / LT |
| Jump (double jump mid-air) | Space | A |
| Dodge | Double-tap A/D/W/S | Y |
| Cycle weapons | 1–5 / wheel | LB/RB or B/X |
| Scoreboard | Tab | — |
| Pause / menus | Esc | D-pad + A, Start |

## Tech

One self-contained HTML file (~138 KB) using [three.js](https://threejs.org/) loaded from a CDN. Procedural canvas textures, WebAudio-synthesized weapons and announcer stingers, an auto-generated navigation graph for the bots, and a 90-assertion Node test harness (world/pathfinding, physics, combat math, gamepad lifecycle, non-standard-pad calibration, and a full bot match simulation).

## Legal

Original fan-made homage. Not affiliated with, endorsed by, or derived from Epic Games' Unreal Tournament franchise; no Epic assets are used.
