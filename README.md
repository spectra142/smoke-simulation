# Smoke Simulation

A real-time, interactive 2D fluid simulation running entirely in a single HTML file. It uses a 256×256 grid-based Navier-Stokes solver with semi-Lagrangian advection, pressure projection, and vorticity confinement to produce smooth, swirling smoke-like motion.

## Features

- **Grid-based fluid solver** — 256×256 stable Navier-Stokes on `Float32Arrays`
- **Semi-Lagrangian advection** — keeps the simulation stable even at high velocities
- **Pressure projection** — enforces incompressibility so the fluid preserves volume
- **Vorticity confinement** — preserves realistic eddies and turbulence
- **Procedural rendering** — no external images or libraries; everything is generated in code
- **Mouse and touch support** — works on desktop and mobile browsers
- **Interactive controls** — adjust viscosity, diffusion, and fade rate in real time

## Quick Start

1. Clone or download this repository.
2. Open `smoke_simulation.html` in any modern web browser (Chrome, Firefox, Edge, Safari).
3. Click and drag to push the smoke around.

No build step, no server, and no dependencies are required.

## Controls

| Action | Result |
|--------|--------|
| Left-click + drag | Push smoke in the direction of movement |
| Right-click + drag | Clear / remove smoke |
| Shift + left-click + drag | Also clears smoke |
| **Viscosity** slider | Controls how quickly velocity diffuses |
| **Diffusion** slider | Controls how quickly smoke density spreads |
| **Fade rate** slider | Controls how fast smoke dissipates over time |

## Browser Requirements

Any modern browser with Canvas 2D support. For smooth 60 FPS performance, a recent desktop or mobile GPU/CPU is recommended.

## License

This project is released under the MIT License. See `LICENSE` for details.
