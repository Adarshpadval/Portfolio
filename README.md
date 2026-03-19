# Adarsh Padval — Portfolio

Welcome to the source code for my portfolio. This is a single-page application built without heavy front-end frameworks, demonstrating high-performance, modern UI/UX design, and complex interactivity using core web technologies (HTML, CSS, JavaScript).

## 🚀 Live Demo
You can view the live portfolio at: [https://adarshpadval.github.io/portfolio/](https://adarshpadval.github.io/portfolio/)

## ⚡ Core Features

- **Blazing Fast Performance**: Zero-dependency architecture. A standalone HTML file containing optimized embedded CSS, SVG strings, and modular Vanilla JS loops, keeping the payload incredibly light (~160KB total).
- **Physics-Based Interaction**: Custom interactive force-directed graph (Skill Constellation) built using the HTML5 `<canvas>` API, customized with repulsion and attraction physics.
- **Command Palette (`Cmd+K` or `/`)**: MacOS Spotlight-style navigation modal providing fast context-switching and keyboard-centric access.
- **Micro-Animations & Visuals**: Modern glassmorphism UI rules, custom interactive cursor engine, CSS-animated parallax avatars, and typing effects.
- **Magnetic Buttons & Live Clock**: Premium interaction states simulating natural physical weight (magnetism) and a dynamic system status clock.
- **Technical SEO**: Fully implemented structured schema (`application/ld+json`), semantic tags, and Open Graph directives.

## 💻 Tech Stack
- Vanilla HTML5 / Semantic DOM
- Pure CSS3 (`var()` theming, flexbox/grid, 3D transforms, custom properties)
- Modular ES6+ JavaScript (IIFEs, RequestAnimationFrame wrappers, IntersectionObserver)

## 🏗 Setup & Modifying Projects
Because this is a zero-dependency build, no build steps (`npm`, `webpack`) are strictly required.

1. **Serve the file locally:**
   We recommend using Live Server (VSCode) or simple HTTP server to avoid CORS issues with canvasses and modules.
   ```bash
   npx serve .
   ```

2. **Add or modify projects:**
   Navigate to the bottom of the Javascript section inside `index.html`. You will find the data array `PROJS`. Add new entries following this structure:
   ```javascript
   { 
     t: 'Project Name', 
     c: 'biz', // 'biz' or 'saas'
     hs: ['#primaryColor', '#secondaryColor'], // Hero gradients
     d: 'Description here', 
     s: ['Tech 1', 'Tech 2'], 
     u: 'https://link-to-live-site.com' 
   }
   ```

## 🎨 Modifying Appearance
Most theme configuration is driven by CSS variables located in the `:root` scope at the top of the stylesheet.
```css
:root {
  --c0: #020812;   /* Main Background */
  --c1: #050d18;   /* Section Striping */
  --cyan: #00d4ff; /* Primary Highlight */
  --green: #00ff9d;/* Success Accent */
}
```

## 📜 License
&copy; 2025 Adarsh Padval. All rights reserved. 
