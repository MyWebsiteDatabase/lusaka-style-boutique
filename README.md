# Lusaka Style Boutique — SOD203 Team 2

Promotional website for **Lusaka Style Boutique**, a contemporary Zambian fashion boutique created for Northrise University SOD203 Multimedia Publishing.

> **Demonstration Notice**: This project is a front-end student demonstration. It does not process online payments, manage user accounts, or submit live server emails.

---

## What was Upgraded (Stage 4 Enhanced)

- **Luxury Brand Aesthetic**: Editorial color palette featuring obsidian black, ivory cream, crisp white, and champagne gold (`#c5a059`).
- **Real Curated Fashion Photography**: Added real high-resolution images for hero, shirts, trousers, wrap dresses, shoes, accessories, and boutique interior.
- **Footwear Category**: Added shoes & sandals category with tailored loafers and block heel sandals.
- **Contextual WhatsApp Shopping**: Product buttons open pre-formatted WhatsApp orders specifying exact item names and prices in Zambian Kwacha (ZMW).
- **Interactive Multimedia**:
  - HTML5 video player with WebVTT captions (`captions.vtt`) and custom poster (`video-poster.jpg`).
  - HTML5 boutique audio player with visible controls, sample voice track, and full transcript.
  - Automatic graceful fallback cards if media files are missing.
- **Smooth Animations**: Scroll-triggered reveals via `IntersectionObserver`, image hover zoom, header shadow on scroll, animated mobile drawer navigation, and full `@media (prefers-reduced-motion: reduce)` accessibility support.
- **Lightbox Dialog**: Any product or gallery image enlarges into an interactive modal with full keyboard and backdrop dismissal.
- **Client-Side Validation**: Accessible contact form with instant validation alerts.

---

## How to Open the Website

You do **not** need Node, React, or a database.

### Option A — Double-Click (Simplest)
1. Open the folder `sod203-team2`.
2. Double-click `index.html`.
3. It will open directly in Microsoft Edge, Google Chrome, or Mozilla Firefox.

### Option B — VS Code Live Server
1. Open the `sod203-team2` folder in VS Code.
2. Install the **Live Server** extension if not already installed.
3. Right-click `index.html` → **Open with Live Server**.

---

## File Structure

| File / Folder | Purpose |
|---------------|---------|
| `index.html` | Home page (Hero, featured looks, Independence banner, video & audio showcase) |
| `about.html` | Brand story, mission, vision, values, showroom gallery, and audio welcome |
| `products.html` | Complete catalogue with live search, category chips, and WhatsApp order buttons |
| `news.html` | News, student styling specials, pop-up events, and promotional poster |
| `contact.html` | Accessible contact form, WhatsApp ordering setup, boutique hours, and location |
| `css/style.css` | Shared luxury stylesheet (variables, grid/flexbox, animations, media queries) |
| `js/script.js` | Interactive script (nav drawer, WhatsApp builder, search/filter, lightbox, fallbacks) |
| `assets/images/` | High-resolution photography (hero, apparel, footwear, accessories, showroom) |
| `assets/video/` | Promotional MP4 video (`promo-video.mp4`) and WebVTT captions (`captions.vtt`) |
| `assets/audio/` | Spoken audio introduction (`promo-audio.mp3` / `promo-audio.wav`) |
| `assets/graphics/` | Brand logos and vector campaign artwork (`logo.svg`, `promo-poster.svg`) |
| `docs/` | Academic analysis, sitemap, wireframes, testing plan, and report outline |

---

## How to Add Your Own Media Files

### 1. Adding Your WhatsApp Business Number
1. Open `js/script.js` in a text editor.
2. Near the top, find:
   ```javascript
   var CONFIG = {
     whatsappNumber: "", // Enter your number here
   ```
3. Enter your phone number using country code and digits only (no `+` or spaces), for example:
   ```javascript
   whatsappNumber: "260971234567",
   ```
4. Save the file. All product buttons will automatically generate direct WhatsApp order links!

### 2. Replacing Fashion Images
1. Save your photos inside `assets/images/` using standard JPEG (`.jpg`) format:
   - `hero-fashion.jpg` — Home page hero banner
   - `shirt-kafue.jpg` — Kafue Linen Shirt
   - `shirt-cairo.jpg` — Cairo Road Oxford Shirt
   - `trousers-olwende.jpg` — Olwende Chinos
   - `trousers-mutendere.jpg` — Mutendere Wide Trousers
   - `dress-leopards.jpg` — Leopards Hill Wrap Dress
   - `dress-woodlands.jpg` — Woodlands Shirt Dress
   - `shoes-loafers.jpg` — Mosi Leather Loafers
   - `shoes-sandals.jpg` — Kalambo Strap Sandals
   - `accessory-necklace.jpg` — Copperbelt Bead Necklace
   - `accessory-tote.jpg` — Arcades Canvas Tote
   - `about-interior.jpg` — Boutique interior showroom
   - `about-display.jpg` — Clothing rail display
   - `about-fabric.jpg` — Fabric craftsmanship detail
   - `video-poster.jpg` — Video player poster still frame

### 3. Replacing Video & Captions
1. Export your promotional fashion film as an MP4 (H.264 video, AAC audio).
2. Save it as `assets/video/promo-video.mp4`.
3. Open `assets/video/captions.vtt` and replace the sample text and timestamps with your transcript.

### 4. Replacing Audio
1. Record a 20–45 second spoken welcome message.
2. Export as MP3 or WAV and save as `assets/audio/promo-audio.mp3` (or `promo-audio.wav`).
3. If you adjust your speech, update the written transcripts on `index.html` and `about.html`.

---

## Accessibility Compliance

- **Keyboard Navigable**: Visible golden focus outlines on all interactive elements.
- **Semantic Structure**: Proper landmarks (`<header>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<footer>`) and strict heading hierarchy (`<h1>` through `<h3>`).
- **Screen Reader Support**: Descriptive `aria-label`, `aria-expanded`, `aria-current`, and modal dialog semantics.
- **Contrast**: Complies with WCAG AA contrast standards.
- **Reduced Motion**: Respects `prefers-reduced-motion: reduce` by disabling transitions and animations for motion-sensitive users.
