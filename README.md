# ✦ Sakura Mehndi Artistry — Luxury Website

<div align="center">

![Version](https://img.shields.io/badge/version-1.0.0-C9A84C?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=three.js&logoColor=white)
![GSAP](https://img.shields.io/badge/GSAP-88CE02?style=for-the-badge&logo=greensock&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-7B0D1E?style=for-the-badge)

**A cinematic, luxury-grade, fully responsive website for a premium Bridal Mehndi Designer brand.**

[Live Preview](#) · [Report Bug](#) · [Request Feature](#)

</div>

---

## 📖 Table of Contents

- [Overview](#-overview)
- [Screenshots](#-screenshots)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [File Structure](#-file-structure)
- [Getting Started](#-getting-started)
- [Customization Guide](#-customization-guide)
- [Sections Breakdown](#-sections-breakdown)
- [Performance](#-performance)
- [Browser Support](#-browser-support)
- [Roadmap](#-roadmap)
- [License](#-license)

---

## 🌟 Overview

**Sakura Mehndi Artistry** is a single-file, production-ready luxury website designed for a premium bridal mehndi artist brand. It delivers a cinematic digital experience — immersive 3D visuals, smooth GSAP animations, glassmorphism UI, and a complete booking workflow — all targeting high-end wedding clients.

The entire site is contained in **one self-sufficient HTML file** with zero build tools required. Just open in a browser.

> **Design Philosophy:** Royal Indian wedding aesthetic fused with modern minimalism. Every pixel intentional. Every interaction meaningful.

---

## 📸 Screenshots

> *(Replace with actual screenshots after deployment)*

| Section | Description |
|---|---|
| 🎬 Hero | Fullscreen Three.js particle mandala + animated headline |
| 🌸 About | Split layout with ornamental frame, stats counter, timeline |
| 💎 Services | 3D tilt glassmorphism cards with modal detail popups |
| 🖼️ Gallery | Masonry grid with hover tilt and overlay animations |
| 💬 Testimonials | Auto-playing carousel with coverflow-style active card |
| 📅 Booking | 3-step animated form → WhatsApp deep-link |
| 📸 Instagram | 12-tile hover grid social proof section |
| 🦶 Footer | 4-column elegant footer with animated social icons |

---

## ✨ Features

### 🎨 Design & Visual
- **Royal color palette** — Deep Maroon, Gold, Ivory, Blush as CSS custom properties
- **Glassmorphism** cards with backdrop-filter blur and gold border accents
- **Ornamental UI elements** — corner frames, diamond dividers, spoke lines
- **Elegant typography** — `Cormorant Garamond` (serif display) + `Jost` (clean sans-serif)
- **Dark / Light mode** toggle with smooth CSS variable transition

### 🌐 3D & Animation
- **Three.js Hero Scene** — 600-particle gold shimmer system + animated mandala torus rings
- **Mouse parallax** — mandala follows cursor movement in real-time
- **SVG Preloader** — mehndi mandala drawn via `stroke-dashoffset` animation (~3.2s)
- **GSAP ScrollTrigger** — reveal animations, parallax, stagger effects on every section
- **VanillaTilt** — 3D perspective tilt with glare on all service cards
- **Testimonial carousel** — smooth GSAP `x` transform with auto-play

### 🖱️ Micro-interactions
- **Custom cursor** — gold dot + ring follower + canvas particle trail
- **Hover states** — glow follow, underline reveals, scale transforms, border transitions
- **Button shimmer** — sliding gold fill on CTA hover
- **Gallery** — scale + overlay reveal on hover
- **Social icons** — lift-up translateY on hover

### 📱 UX & Accessibility
- **Mobile-first responsive** — tested at 480px / 768px / 1024px
- **Hamburger drawer nav** — smooth slide-in with overlay backdrop
- **Smooth anchor scrolling** — GSAP `ScrollToPlugin` with offset compensation
- **Scroll progress bar** — gradient indicator at the very top of the viewport
- **Floating CTA** — persistent WhatsApp + Book Now buttons
- **ESC key** closes modals
- **`aria-label`** on all icon-only buttons

### 🔊 Extra Delights
- **Ambient music toggle** — Web Audio API layered sine/triangle harmonics (C major chord)
- **Animated counter** — stats count up when scrolled into view
- **Service modals** — detailed package info with smooth scale-in transition
- **WhatsApp deep-link** — booking form auto-generates a pre-filled WhatsApp message

---

## 🛠 Tech Stack

| Library | Version | Purpose |
|---|---|---|
| [Three.js](https://threejs.org/) | r128 | 3D hero scene — particles, geometry, renderer |
| [GSAP](https://greensock.com/gsap/) | 3.12.2 | All animations — scroll, timeline, transitions |
| [GSAP ScrollTrigger](https://greensock.com/scrolltrigger/) | 3.12.2 | Scroll-driven animation engine |
| [GSAP ScrollToPlugin](https://greensock.com/scrolltoplugin/) | 3.12.2 | Smooth anchor navigation |
| [VanillaTilt.js](https://micku7zu.github.io/vanilla-tilt.js/) | 1.8.1 | 3D card tilt + glare |
| [Google Fonts](https://fonts.google.com/) | — | Cormorant Garamond + Jost + Dancing Script |
| Web Audio API | Native | Ambient background music |
| CSS Custom Properties | Native | Theming system (dark/light mode) |

> All libraries are loaded from **cdnjs.cloudflare.com CDN** — no npm, no build step.

---

## 📁 File Structure

```
mehndi-luxury-website/
│
├── mehndi-luxury-website.html    # ← The entire website (single file)
└── README.md                     # ← This documentation
```

### Inside the HTML file — Modular Comment Blocks

```
<!-- SECTION 1:  CSS Variables & Theme System  -->
<!-- SECTION 2:  Custom Cursor Styles          -->
<!-- SECTION 3:  Preloader Animation           -->
<!-- SECTION 4:  Navigation Bar                -->
<!-- SECTION 5:  Hero (Three.js Canvas)        -->
<!-- SECTION 6:  About                         -->
<!-- SECTION 7:  Services + Modal              -->
<!-- SECTION 8:  Gallery                       -->
<!-- SECTION 9:  Testimonials Carousel         -->
<!-- SECTION 10: Booking Form (3-step)         -->
<!-- SECTION 11: Instagram / Social Grid       -->
<!-- SECTION 12: Floating CTA                  -->
<!-- SECTION 13: Footer                        -->

// JS Block 1:  Preloader fade-out
// JS Block 2:  Custom cursor + trail canvas
// JS Block 3:  Three.js hero scene setup
// JS Block 4:  Hero GSAP timeline (post-preloader)
// JS Block 5:  GSAP ScrollTrigger animations
// JS Block 6:  Mobile nav drawer
// JS Block 7:  Dark / Light theme toggle
// JS Block 8:  Ambient Web Audio music
// JS Block 9:  Service card glow follow
// JS Block 10: Service modal open / close
// JS Block 11: Testimonials carousel
// JS Block 12: Booking form steps + WhatsApp
// JS Block 13: VanillaTilt init
// JS Block 14: Nav + Float CTA entrance
```

---

## 🚀 Getting Started

### Option A — Open directly (simplest)
```bash
# Just double-click the file, or:
open mehndi-luxury-website.html
```

### Option B — Local dev server (recommended for full feature support)
```bash
# Using Python 3
python -m http.server 8080

# Using Node.js (npx)
npx serve .

# Using VS Code
# Install "Live Server" extension → Right-click → Open with Live Server
```

Then visit `http://localhost:8080` in your browser.

> ⚠️ **Note:** The Web Audio API ambient music requires a local server or HTTPS in some browsers due to autoplay policies. Opening directly via `file://` will mute this feature — all other features work fine.

---

## 🎨 Customization Guide

### 1. Brand Name & Identity
Find and replace `Zara` / `Zara Mehndi Artistry` / `zaramehndiartistry` throughout the file.

```html
<!-- Line ~420 -->
<a href="#hero" class="nav-logo">✦ Zara <span>Artistry</span></a>

<!-- Line ~470 -->
<h1 class="hero-title">Luxury Mehndi Art for Your <em>Special</em> Moments</h1>
```

---

### 2. Color Palette
All colors are CSS custom properties at the top of the `<style>` block:

```css
:root {
  --maroon:      #7B0D1E;   /* Primary brand color    */
  --gold:        #C9A84C;   /* Accent / highlight      */
  --ivory:       #F7F2E8;   /* Light text / backgrounds */
  --blush:       #F0D4CF;   /* Soft accent             */
  --bg-dark:     #0E0608;   /* Dark background base    */
}
```

> Change these 5 variables and the entire site recolors instantly.

---

### 3. Adding Real Photography
Replace the SVG placeholder blocks with `<img>` tags:

```html
<!-- Find the about-image-placeholder div and replace with: -->
<div class="about-image-placeholder">
  <img src="your-artist-photo.jpg" alt="Sakura — Master Mehndi Artist"
       style="width:100%;height:100%;object-fit:cover;" />
</div>
```

For gallery items, replace `.gallery-svg` divs:
```html
<div class="gallery-item-inner">
  <img src="gallery/bridal-01.jpg" alt="Bridal Mehndi Design"
       style="width:100%;height:100%;object-fit:cover;" />
  <div class="gallery-overlay">...</div>
</div>
```

---

### 4. WhatsApp Number
Two locations to update:

```html
<!-- Floating CTA button (~line 590) -->
<a href="https://wa.me/91 XXXXXXXXXX?text=...">

<!-- Booking form JS (~line 700) -->
const link = 'https://wa.me/91 XXXXXXXXXX?text=' + ...
```

Replace `91 XXXXXXXXXX` with your number (country code + number, no `+` or spaces).

---

### 5. Pricing & Services
Service prices and details are in the `serviceData` JavaScript object:

```javascript
const serviceData = {
  bridal: {
    name: 'Royal Bridal Mehndi',
    price: '₹18,000',
    duration: '4 – 6 hours',
    includes: ['Full hands & arms', '...'],
    note: 'Travel charges extra...'
  },
  // arabic, indowestern, festival ...
};
```

Card prices in the HTML:
```html
<div class="service-price">₹18,000 <span>/ session</span></div>
```

---

### 6. Contact Information
In the footer section:
```html
<span>Jamshedpur, Jharkhand & Pan-India Travel</span>
<span>+91 98765 43210</span>
<span>hello@zaramehndiartistry.com</span>
```

---

### 7. Social Media Links
Footer social icons:
```html
<a href="https://instagram.com/yourhandle" class="social-icon">📸</a>
<a href="https://pinterest.com/yourhandle" class="social-icon">📌</a>
```

Instagram handle in social section:
```html
<p>@zaramehndiartistry · 180k followers</p>
<a href="https://instagram.com/yourhandle">Follow @zaramehndiartistry →</a>
```

---

### 8. SEO Meta Tags
At the top of `<head>`:
```html
<meta name="description" content="Your custom description here..." />
<meta name="keywords" content="your, keywords, here" />
<title>Your Brand Name | Tagline</title>
```

Add Open Graph tags for social sharing:
```html
<meta property="og:title" content="Zara Mehndi Artistry" />
<meta property="og:description" content="Luxury Bridal Henna..." />
<meta property="og:image" content="https://yourdomain.com/og-image.jpg" />
<meta property="og:url" content="https://yourdomain.com" />
```

---

### 9. Preloader Timing
Adjust preloader display duration (default: 3200ms):
```javascript
// Around line 620
setTimeout(() => { /* fade out preloader */ }, 3200);
```

SVG drawing speed (CSS):
```css
.preloader-path {
  animation: drawMehndi 3s ease forwards 0.3s; /* adjust 3s */
}
```

---

### 10. Particle Count (Performance)
Reduce particles on lower-end devices:
```javascript
const particleCount = 600; // reduce to 300 for better performance
```

---

## 📋 Sections Breakdown

| # | Section | Key Elements |
|---|---|---|
| 1 | **Hero** | Three.js canvas, 600 gold particles, mandala rings, mouse parallax, GSAP headline reveal |
| 2 | **About** | Split grid, ornamental photo frame, animated stat counters, GSAP timeline items |
| 3 | **Services** | 4 glassmorphism cards, VanillaTilt 3D, glow cursor follow, detail modals |
| 4 | **Gallery** | 8-item masonry grid, CSS column layout, hover scale + overlay reveal |
| 5 | **Testimonials** | 4-card GSAP carousel, auto-play, dot navigation, active card highlight |
| 6 | **Booking** | 3-step form, package radio select, WhatsApp deep-link pre-fill |
| 7 | **Social** | 12-tile Instagram-style grid, hover opacity reveal |
| 8 | **Footer** | 4-column grid, contact info, policy links, social icons |

---

## ⚡ Performance

- **Single HTTP request** for the HTML file itself
- **CDN-loaded libraries** — cached by browsers across sites
- **Google Fonts** — preconnected via `<link rel="preconnect">`
- **Three.js pixel ratio capped** at `2` to prevent GPU overload on retina screens
- **Particle count** configurable (default 600 — runs at 60fps on modern hardware)
- **CSS animations** use `transform` and `opacity` exclusively — no layout thrashing
- **ScrollTrigger** uses `IntersectionObserver` under the hood — efficient scroll detection
- Recommend adding `loading="lazy"` to `<img>` tags when adding real photos

### Lighthouse Estimates *(with real images optimized)*
| Metric | Target |
|---|---|
| Performance | 85–92 |
| Accessibility | 90+ |
| Best Practices | 95+ |
| SEO | 95+ |

---

## 🌐 Browser Support

| Browser | Support |
|---|---|
| Chrome 90+ | ✅ Full |
| Firefox 88+ | ✅ Full |
| Safari 14+ | ✅ Full |
| Edge 90+ | ✅ Full |
| Opera 76+ | ✅ Full |
| Samsung Internet | ✅ Full |
| IE 11 | ❌ Not supported |

> CSS custom properties, `backdrop-filter`, and Web Audio API require modern browsers. All features degrade gracefully on older environments.

---

## 🗺 Roadmap

Future enhancements to consider:

- [ ] **Real image gallery** — integrate Cloudinary for optimized delivery
- [ ] **Lightbox** — full-screen image viewer with cinematic transition
- [ ] **360° hand preview** — Three.js interactive hand model with mehndi texture
- [ ] **Backend booking** — connect form to Firebase / Supabase for lead capture
- [ ] **CMS integration** — Contentful or Sanity for non-technical content updates
- [ ] **Live Instagram feed** — Instagram Basic Display API integration
- [ ] **Multi-language** — Hindi / Urdu / Arabic toggle
- [ ] **PWA** — service worker + manifest for installable app experience
- [ ] **Video hero** — optional background video fallback for the 3D scene

---

## 👩‍💻 Developer Notes

### CSS Architecture
All styles live in a single `<style>` block organized into clearly commented sections. CSS custom properties (variables) handle the entire theming system — adding a third theme requires only a new `[data-theme="xyz"]` block.

### JavaScript Architecture
All JS is in a single `<script>` block at the bottom, organized into 14 numbered comment blocks. No framework dependencies — pure vanilla JS + library APIs.

### Animation Philosophy
- **Page load:** GSAP timeline (sequential, orchestrated)
- **Scroll:** GSAP ScrollTrigger (efficient, scrub-capable)
- **Hover:** CSS transitions (GPU-composited, no JS overhead)
- **3D:** Three.js rAF loop (decoupled from scroll/GSAP)

### Adding a New Section
1. Add HTML after the relevant existing section
2. Add CSS in the `<style>` block with a clear comment header
3. Add a `.reveal` class to elements you want scroll-animated
4. ScrollTrigger picks up `.reveal` elements automatically

---

## 📄 License

```
MIT License

Copyright (c) 2025 Zara Mehndi Artistry

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND.
```

---

<div align="center">

**Made with ✦ and tradition**

*Crafted for brides who deserve nothing less than extraordinary*

[⬆ Back to Top](#-zara-mehndi-artistry--luxury-website)

</div>
