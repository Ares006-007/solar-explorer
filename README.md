# Solar System Explorer

**Glide through the cosmos—explore an interactive 3D Solar System with stunning visuals, planetary facts, and mythological insights.**

---

## Live Demo

Check out the live experience here: https://ares006-007.github.io/solar-explorer/

---

## About the Project

**Solar System Explorer** is an interactive web application that takes you on a journey through our Solar System. Navigate smoothly between Mercury, Venus, Earth, Mars, Jupiter, Saturn, Uranus, Neptune, and Pluto while discovering fascinating facts about each celestial body.

The application features:
- **3D planet visualization** with realistic textures
- **Interactive planet selection** via an intuitive sidebar menu
- **Orbital mechanics display** showing each planet's distance from the Sun in Astronomical Units (AU)
- **Smooth animations** creating an immersive "gliding" experience between planets
- **Detailed information panels** with scientific facts, myths, and unique characteristics for each world
- **Moon orbital systems** showing known satellites for each planet
- **Responsive design** optimized for desktop viewing

This project is perfect for astronomy enthusiasts, educators, and anyone curious about our place in the cosmos.

---

## Key Features

- **Planet Selector** — Click on any planet in the left sidebar to smoothly transition to it
- **AU Distance Display** — See the orbital distance from the Sun in Astronomical Units for each planet
- **3D Animations** — CSS-driven 3D transforms create a stunning parallax effect as you navigate
- **Interactive Moon Systems** — Visual representation of satellites orbiting planets (Earth's Moon, Mars' Moons, Jupiter's Galilean Moons, etc.)
- **Detail Panels** — Expandable information cards with fascinating planetary facts and mythology
- **Texture-Mapped Planets** — Real NASA textures and quality images for authentic planet appearance
- **Smooth Transitions** — Cubic-bezier animations for fluid navigation between planets
- **Fullscreen Experience** — Immersive viewport optimized for exploration

---

## Tech Stack

- **HTML5** — Semantic structure and form controls (radio inputs for planet selection)
- **CSS3** — Advanced features including:
  - 3D transforms (translateZ, rotateX, perspective)
  - Keyframe animations
  - CSS transitions and cubic-bezier timing functions
  - Responsive positioning and viewport geometry
- **Vanilla JavaScript** — None required; pure CSS-based interactivity using radio button state management
- **External Resources** — Font Awesome icons and Google Fonts (Montserrat)

---

## File Structure

```
solar-explorer/
├── index.html          # Main HTML file with planet structure and info panels
├── style.css           # Comprehensive styling and animations
└── README.md           # Project documentation (this file)
```

---

## Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- No build tools, npm, or dependencies required!

### Installation & Running Locally

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Ares006-007/solar-explorer.git
   cd solar-explorer
   ```

2. **Open in your browser:**
   - **Option A:** Double-click index.html
   - **Option B:** Use a local server (recommended for best results)
     ```bash
     # Using Python 3
     python -m http.server 8000
     
     # Using Python 2
     python -m SimpleHTTPServer 8000
     
     # Using Node.js (if installed)
     npx http-server
     ```
   
   Then navigate to http://localhost:8000 in your browser.

3. **Start exploring!** Click on any planet in the left sidebar to glide to it.

---

## How It Works

### UI Logic

**Planet Selection:**
- Each planet is associated with a hidden input type="radio" element
- Clicking a planet's label in the sidebar triggers the corresponding radio button
- CSS :checked pseudo-selectors manage all visual state changes

**Navigation Flow:**
1. User clicks a planet label
2. Radio input becomes checked
3. CSS selectors like input[type=radio].planet1:checked + label + div .solar_systm:nth-of-type(1) apply transforms
4. 3D perspective shifts planets into view
5. Animations cascade with staggered timing for smooth entry

**3D Transformations:**
- Each planet container uses translateZ() to position it in 3D space
- perspective property creates the depth effect
- rotateX(-20deg) tilts the solar system for visual interest
- Planets are repositioned based on which radio is checked

**Information Panels:**
- Secondary radio inputs manage panel visibility
- Clicking "Read More" on a planet shows a detailed information card with:
  - Historical mythology
  - Scientific facts and statistics
  - High-quality representative images
  - Key characteristics (rotation, orbit, notable features)

**Moon Systems:**
- Orbital trajectories drawn with border: dashed
- Moon elements positioned absolutely with CSS transforms
- Each moon orbits its parent planet in a circular pattern

---

## Screenshots

<!-- Add screenshots here -->

---

## Author

@code.ares — Crafted with curiosity and CSS magic

---

## License

This project is licensed under the MIT License — feel free to use, modify, and distribute as you wish.

---

## Fun Facts from the Explorer

- **Mercury**: 88-day year, fastest planet
- **Venus**: Rotates backward! Days are longer than years
- **Earth**: The only known planet with life
- **Mars**: Home to Olympus Mons, the solar system's tallest mountain
- **Jupiter**: The largest planet; has 4 Galilean moons
- **Saturn**: Famous for its stunning ring system
- **Uranus**: Rotates on its side with a 84-year orbit
- **Neptune**: Fastest winds in the solar system
- **Pluto**: Reclassified as a dwarf planet in 2006

---

Enjoy your journey through space!