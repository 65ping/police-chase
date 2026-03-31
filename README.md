# Police Chase

A top-down 2D police chase game built entirely in the browser with HTML5 Canvas, CSS, and JavaScript. No dependencies, no build step — just open and play.

**[Play Now](https://65ping.github.io/police-chase/)**

## Gameplay

You're a police officer chasing reckless drivers through a neon-lit city at night. Use your siren to pull them over, or bump them to force a stop. Don't let them crash into buildings or traffic — 3 to 7 crashes (depending on difficulty) and it's game over.

## Controls

| Input | Action |
|-------|--------|
| Arrow Keys / WASD | Drive in that direction |
| Space | Activate siren |
| 1-5 | Select difficulty |
| Enter | Start / Restart |

Touch controls are also supported: left side of screen = virtual joystick, right side tap = siren.

## Features

- **Point & Drive controls** — car moves in the direction you press, no tank steering
- **5 difficulty levels** — from Rookie (7 lives, slow enemies) to Chief (3 lives, fast enemies)
- **Combo multiplier** — arrest drivers quickly in succession for x2 to x5 score
- **Speed bonus** — arrest a driver within seconds of their spawn for FAST! or LIGHTNING! bonus points
- **Police rank system** — earn promotions from Cadet to Chief as your score climbs
- **Star rating** — 1 to 5 stars on game over based on performance
- **High score persistence** — best scores saved per difficulty level
- **Edge-of-screen indicators** — arrows point toward off-screen reckless drivers with distance
- **Procedural audio** — siren wail, crash thuds, arrest chimes, rank-up fanfares via Web Audio API
- **Neon noir aesthetic** — dark city, glowing buildings, additive-blend siren lights, particle effects
- **Minimap** — bottom-right corner shows the area around you
- **Mobile/touch support** — virtual joystick + tap siren

## Difficulty Levels

| Level | Name | Lives | Enemy Speed | Siren Range |
|-------|------|-------|-------------|-------------|
| 1 | Rookie | 7 | Slow | Wide |
| 2 | Patrol | 6 | Medium | Standard |
| 3 | Pursuit | 5 | Normal | Normal |
| 4 | SWAT | 4 | Fast | Narrow |
| 5 | Chief | 3 | Very Fast | Tight |

## Tech

- Single `index.html` file, zero dependencies
- HTML5 Canvas 2D rendering with `requestAnimationFrame`
- Procedural city generation using deterministic sin-hash
- Web Audio API for all sound effects
- localStorage for high score persistence
- Google Fonts: Orbitron + JetBrains Mono

## License

MIT
