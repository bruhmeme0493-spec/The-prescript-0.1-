# The-prescript-v0.1α

# PRESCRYPT v0.1α ❀

A Limbus Company-inspired cyberpunk terminal and electronic badge interface. This is the **v0.1α** stable web prototype, designed to validate the layout, visual identity, and UI behavior before porting to physical hardware.

## 📱 Project Overview
This interface is engineered specifically for low-resolution embedded displays, mimicking an unstable, dystopian corporate terminal that delivers "Prescripts" (commands). 

* **Target Hardware:** ESP32 Microcontroller + 240x320 TFT Display (SPI).
* **Current State:** Fully functional responsive web layout (scaled 2x to 480x640 for development and pixel-hunting on mobile screens).

## 🚀 Key Features Implemented

### 1. Pixel-Perfect SVG Identity
* Integrated the exact text glyph `❀` directly into the SVG rendering pipeline alongside a vector arrow component (`<path>`).
* Avoided standard shape approximations to ensure 100% font-rendering consistency across platforms.
* Applied dual-layer CSS neon drop-shadows (`#5B9BD5` and `#FFD700`) for a high-contrast cyberpunk glow.

### 2. Procedural Interface Glitches
* Implemented a lightweight vanilla JavaScript text destabilizer.
* Randomized character swaps using a custom terminal pool (`0123456789X█▀▄■░▒▓❀⬆`).
* Color-shift alerts that dynamically trigger short styling drops (150ms duration) without breaking the DOM container grid layout.

### 3. Core Mechanics & Grid
* **Binary Stream:** A script-generated background matrix operating at low opacity (0.04) to enhance the technical atmosphere.
* **Autonomous Clock:** A standard 1-second interval loop countdown timer (`14:59`) with an embedded auto-reset sequence on zero-out conditions.
* **Layout Isolation:** Complete use of `flex-shrink: 0` variables to protect header and footer alignment on compact screens.

## 🛠 Tech Stack
* **Frontend:** Semantic HTML5, Vanilla CSS3 (Flexbox architecture).
* **Logic:** Pure Vanilla JavaScript (No heavy frameworks, optimization for future C++ porting).
* **Fonts:** Google Fonts (`Share Tech Mono`).

## 🗺 Roadmap to v0.2
- IDK we'll see what i will do in the future 