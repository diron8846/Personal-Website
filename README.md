# Personal Portfolio – `index.html` Overview

This repository contains a single-page portfolio for **Dairon R. MuTuku**.  
The entire site is built in `index.html` using plain HTML, CSS (via a `<style>` block) and vanilla JavaScript.  
It relies on just two external dependencies:

* [Google Fonts](https://fonts.google.com/) – Bebas Neue, Syne, DM Mono  
* [Three.js r128](https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js) – for the animated hero scene  

---
## Hosted on Vercel https://daironrevival.vercel.app/

## 🎨 Visual & UI Highlights

* **Custom CSS variables** for colour palette and font families (`--champ`, `--steel`, `--ff-disp`, etc.).
* **Animated custom cursor** with a trailing ring and hover state.
* **Loader screen** with flickering film frames and percentage counter.
* **Hero section**:
  * Dark, animated gradient background with particle grid.
  * 3‑D Three.js scene: pulsing icosahedron, rings, crystals and particles that respond to mouse.
  * Typographic hero headline with gradient text animation.
  * Magnetic buttons, floating statistic cards, scroll cue.
* **Marquee strip** of skill keywords.
* **About section** with a Rive‑style SVG character that reacts to cursor movement.
* **Skills grid** containing tilt‑interactive skill cards with percentage bars.
* **Project cards** that flip on hover, showing thumbnails and back details/links.
* **Experience timeline**, CV call‑to‑action, contact area with animated button glows.
* **Fixed social dock** (GitHub, LinkedIn, Twitter, Instagram) with 3‑D hover effect.
* **Responsive breakpoints** at 960px and 600px for layouts.

---

## 🧠 JavaScript Features

1. **Loader animation** – pseudo‑random percent updating until page load then fade‑out.
2. **Custom cursor logic** – follows mouse, expands on interactive elements.
3. **Three.js hero scene** – initializes camera, geometry, mouse parallax, animate loop, resize handling and scroll‑fade.
4. **Nav scroll class toggle** – adds `.scrolled` when the page is moved.
5. **Magnetic buttons** – slight mouse‑driven translation inside wrapper.
6. **Smooth scrolling** – anchors and CTA buttons scroll to their targets.
7. **Intersection observers** for reveal animations, stat counters, and timeline/item in‑view triggers.
8. **Animated counters** – projects/years/clients increment when visible.
9. **Skill card 3‑D tilt** on hover.
10. **Contact button cursor glow** – radial light follows cursor inside buttons.
11. **Hero parallax & fade** on scroll.
12. **Rive character interaction** – head follows cursor inside the panel.

---

## 📁 File Structure

```
yt/
├── index.html           # entire site (HTML, CSS, JS all in one)
├── README.md            # this documentation
```

*(Only `index.html` exists in current workspace.)*

---

## ✅ Customization Points

* **Contact info** – email, LinkedIn, GitHub, Instagram links updated inline.
* **Stats** – change `data-target` attributes to adjust projects/years/clients.
* **Text sections** – hero headline, about paragraphs, experience items, etc.
* **Projects list** – duplicate `.project-card` blocks and update content/links.
* **SVG character** – modify or replace the large embedded SVG for a different avatar.

---

## 🚀 How to Run

1. Simply open `index.html` in any modern browser.
2. For local development with file‑access restrictions, you can serve via a simple HTTP server, e.g.:

   ```sh
   python -m http.server 8000
   # or
   npx http-server
   ```

3. Watch the console for any errors (missing assets are unlikely since everything is self‑contained).

---

## 🛠 Notes & Tips

* **Loading issues** – ensure `three.min.js` is reachable (CDN link); the site gracefully degrades if Three.js isn’t available.
* **Editable metrics** – both the visible text and the `data-target` values must be updated together for consistency.
* **Accessibility** – adds `cursor:none` globally, may be undesirable for some users; remove or adjust if needed.
* **Performance** – heavy CSS and inline SVG; test on mobile devices for smoothness, and consider lazy‑loading sections if needed.

---

## 📄 License

This project is released under the [MIT License](LICENSE) – feel free to adapt, share, and build upon it, provided you include the same license in derivative works.

---
😎Dairon

