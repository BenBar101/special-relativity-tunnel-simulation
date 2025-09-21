# Interactive Special Relativity Simulation

![Special Relativity Simulation GIF](https://raw.githubusercontent.com/Vibe-design/special-relativity-simulation/main/special-relativity.gif)

This is a web-based, interactive simulation built with vanilla JavaScript and HTML5 Canvas to visualize the counter-intuitive effects of traveling near the speed of light, as described by Einstein's theory of special relativity.

## Live Demo

**Experience the simulation live here:** [**https://BenBar101.github.io/special-relativity-tunnel-simulation/**](https://BenBar101.github.io/special-relativity-tunnel-simulation/)

---

## Introduction

What would you actually *see* if you could travel at 95% the speed of light? This simulation aims to answer that question by providing a first-person view of a "tunnel" environment, allowing you to control your velocity and observe the strange, mind-bending consequences of special relativity in real-time.

The physics implemented are based on the core equations of the theory, demonstrating that what you see is not a bug or an artistic effect, but a faithful representation of reality at extreme speeds.

## Features: The Physics in Action

This simulation showcases several key principles of special relativity:

#### 🚀 Time Dilation
- **What to look for:** Observe the two clocks in the info panel.
- **The Physics:** The "**Your Time (Moving)**" clock runs slower than the "**Earth Time (Stationary)**" clock. The closer you get to the speed of light, the more dramatic this difference becomes. This is a direct consequence of the principle that moving clocks tick slower.

#### 📏 Length Contraction
- **What to look for:** Pay attention to the green rulers along the top and bottom of the tunnel.
- **The Physics:** These horizontal rulers, aligned with your direction of motion, appear shorter as your speed increases. Notice that the vertical rulers on the side walls **do not** contract, as length contraction only affects the dimension parallel to the velocity.

#### 🎨 Relativistic Doppler Effect & Beaming
- **What to look for:** The colors and brightness of the objects in the tunnel.
- **The Physics:**
  - **Blueshift:** When moving forward, the light from objects in front of you is compressed, shifting its color towards the blue end of the spectrum and making it appear intensely bright.
  - **Redshift:** When moving backward, the light from objects is stretched, shifting its color towards the red end of the spectrum and making it appear much dimmer.

####  warping Relativistic Aberration (The "Tunnel Vision" Effect)
- **What to look for:** The geometry of the tunnel itself.
- **The Physics:** This is perhaps the most dramatic visual effect.
  - **Moving Forward:** The visual field is compressed into a "tunnel" in front of you. Light from your periphery appears bent towards your direction of travel. This is why the scene appears to "blur" or warp into a focused point.
  - **Moving Backward:** The visual field expands radially outwards. Objects appear to fly away from the center towards the edges of your view, creating the perception of even faster motion.

---

## How to Use

- **Velocity Slider:** Use the slider at the top left to control your velocity as a percentage of the speed of light (`c`).
  - Move the slider to the **right** to travel forward.
  - Move the slider to the **left** to travel backward.
- **Info Panels:** The panels at the bottom display real-time data on your proper time, stationary time, the Lorentz factor (γ), and the current percentage of length contraction.

## Built With

- **HTML5 Canvas:** For rendering the 2D projection of the 3D scene.
- **Vanilla JavaScript:** All physics, logic, and rendering are handled with plain JavaScript, with no external libraries or frameworks. This ensures the simulation is lightweight and performant.
- **CSS3:** For styling the user interface.

## Running Locally

No special tools are required to run this project.

1.  Clone the repository:
    ```sh
    git clone https://github.com/BenBar101/special-relativity-tunnel-simulation.git
    ```
2.  Navigate to the directory:
    ```sh
    cd special-relativity-tunnel-simulation 
    ```
3.  Open the `index.html` file in any modern web browser.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
