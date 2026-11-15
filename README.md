# Matiqsson SpaceXplorer AB

**A playable 3D Solar System you can fly through, right in your browser.**

The Sun, all eight planets, major moons, a flyable asteroid belt, and checkpoint rings to thread through. Everything is generated procedurally by code—no external images, 3D models, or sound files. The entire experience fits in **one 118 KB HTML file**.

## Try it

1. Download **`index.html`**: open [`index.html`](index.html) and click **Download raw file** (top-right on GitHub), or right-click → *Save Link As...* on [`raw index.html`](index.html?raw=true).
2. Double-click the downloaded `index.html` to open it in **Chrome**, **Edge**, **Firefox**, or **Safari**.
3. Click anywhere in space (or use the touch controls) to take the helm and start flying.

Nothing to install, no server needed, and works completely offline in any browser with **WebGL 2**.

## What's out there

- **The full Sol System:** The Sun, Mercury, Venus, Earth & Luna, Mars, the Asteroid Belt, Jupiter (with Io & Europa), Saturn (with rings & Titan), Uranus, and Neptune.
- **Ring Challenge & Free Flight:** Fly through all **13 checkpoint rings** to complete the tour—or toggle rings off anytime with `G` for pure scenic exploration.
- **Discovery Scanner & Auto-Orbit:** Approach any world and hold `X` to log science data, engage **Auto-Orbit (`O`)** to circle a planet, or fire **Warp (`F`)** to cruise across the system.
- **Arcade 6DoF Spaceship Flight:** Smooth, weighty steering where holding **Boost** (`Shift` or the on-screen Boost pad) drives you forward while letting you steer cleanly into your target.
- **Procedural Audio:** Real-time thruster rumble, boost roar, and scanner chimes synthesized live with the Web Audio API.

## Controls

| Action | Keyboard & Mouse |
|---|---|
| Steer pitch / yaw | Click space & move mouse (or `Arrow Keys`) |
| Fly / strafe | `W` `A` `S` `D` |
| Move up / down | `Space` / `C` (or `R` / `Ctrl`) |
| Roll left / right | `Q` / `E` |
| Turbo Boost (steer while holding) | Hold `Shift` |
| Cycle target planet / moon | `Tab` / `Shift+Tab` |
| Warp to target | `F` |
| Auto-Orbit target | `O` |
| Scan nearby body | Hold `X` |
| Toggle checkpoint rings | `G` |
| Planets & moons list | `L` |
| Hide / show HUD | `H` |

**On touchscreens:** Use the left virtual stick to fly/strafe, slide across the open screen to look around, and hold the large right **BOOST** pad to thrust while dragging your thumb to steer.

## How it works

- Built directly with **WebGL 2** and custom GLSL procedural planet, atmosphere, ring, and starfield shaders—no 3D engine or external libraries.
- Uses 64-bit (`Float64`) floating-origin camera-relative math with a logarithmic depth buffer to keep planetary scales crisp without jitter or z-fighting.
- Quaternion 6DoF flight physics with zero gimbal lock and live Web Audio synthesis.
