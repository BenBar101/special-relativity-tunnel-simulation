# Interactive Special Relativity Simulation

This is a web-based interactive simulation built with vanilla JavaScript and HTML5 Canvas to visualize several special-relativistic effects from the viewpoint of an observer moving through a stationary tunnel.

## Live Demo

**Experience the simulation live here:** [**https://BenBar101.github.io/special-relativity-tunnel-simulation/**](https://BenBar101.github.io/special-relativity-tunnel-simulation/)

## Physics

The simulation distinguishes between quantities that are measured in an inertial frame and what an observer actually receives as light.

### Time dilation

The moving observer's proper time is `dτ`, while Earth-frame coordinate time satisfies

`dt = γ dτ`,

with

`γ = 1 / sqrt(1 - β²)`.

### Length contraction

The displayed contraction value is the standard inertial-frame result for a length parallel to the relative velocity:

`L = L₀ / γ`.

It is intentionally **not** applied as a simple visual shrinking operation. Optical appearance is calculated from the light reaching the observer.

### Aberration and optical appearance

For every rendered point, the simulation solves the past-light-cone condition

`c (t_obs - t_emit) = |r_source - r_observer(t_emit)|`.

The resulting photon direction is then Lorentz-transformed into the observer frame. This is what determines the apparent direction on the canvas. This avoids treating Lorentz contraction as though it were the same thing as visual appearance.

### Relativistic Doppler shift

The photon four-vector transformation gives the frequency factor used by the renderer. With `n` defined as the photon propagation direction in the Earth frame,

`δ = ω' / ω = γ (1 - β n_z)`.

A stationary object in front of an observer moving forward has `n_z < 0`, so it is blueshifted; objects behind are redshifted. The renderer applies a tone-mapped brightness response so the very large physical Doppler factors at high velocity remain visible on an ordinary display.

The color mapping is a visualization of the Doppler factor rather than a literal spectrum renderer.

## Features

- Interactive velocity control from `-0.95c` to `+0.95c`.
- Proper time and Earth-frame coordinate time.
- Lorentz factor and longitudinal length-contraction value.
- Retarded-time/light-cone rendering.
- Relativistic aberration from a Lorentz transformation of photon directions.
- Direction-dependent relativistic Doppler shift.
- Canvas-based perspective rendering with no external libraries.

## Important interpretation

The simulation is intended as an educational optical visualization. The numerical Lorentz transformations and light-cone calculation are physical; the canvas color mapping and tone mapping are deliberately simplified for visualization. In particular, displayed colors should not be interpreted as a full human-vision or detector-spectrum model.

## Running Locally

No special tools are required.

1. Clone the repository:
   ```sh
   git clone https://github.com/BenBar101/special-relativity-tunnel-simulation.git
   ```
2. Navigate to the repository:
   ```sh
   cd special-relativity-tunnel-simulation
   ```
3. Open `index.html` in a modern browser.

## Built With

- HTML5 Canvas
- Vanilla JavaScript
- CSS3

## License

This project is licensed under the MIT License. See `LICENSE` for details.
