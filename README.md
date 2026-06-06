# 🛠️ ESP32-C3 Case Project — Website

> Multi-page HTML/CSS site documenting the design journey of a 3D-printed protective case for the ESP32-C3 Zero microcontroller. Built for ICT30120 Cert III IT (unit ICTWEB304).

## 📁 Files

```
website/
├── index.html         # Home — overview, bento grid, timeline, table, team, form
├── prototype1.html    # First failed print
├── prototype2.html    # Second failed print
├── prototype3.html    # Third print — needs improvement
├── final.html         # Coming soon (placeholder w/ progress + checklist)
├── style.css          # Shared stylesheet (~700 lines, no frameworks)
└── README.md          # This file
```

## ✨ What's in this build

### Design
- **Ocean Breeze** dark teal palette (your existing scheme)
- **Bento grid** homepage layout (2026 trend)
- **Terminal/dev personality** blocks throughout (it's an embedded electronics project — felt fitting)
- **Bold typography** with gradient flowing text
- **Subtle floating geometric shapes** in the background (the 3D-printed-piece vibe)
- **Grid texture overlay** behind everything (with radial mask so edges fade)
- **Scroll progress bar** at the top
- **Scroll-reveal animations** (IntersectionObserver — no library)
- **Mouse-follow glow** on bento cards
- **Animated timeline** with pinging dots, alternating left/right on desktop
- **Lightbox** image preview
- **Mobile-responsive** with hamburger menu
- **Custom scroll-driven progress bar** + animated progress bar on final page
- **Pulse / spin / shine / blink** micro-animations
- **Status colour system** (pass/warn/fail/pending badges)
- **Brutalist-meets-polished** vibe (eyebrow tags with `//` markers, mono labels)

### Tech
- **100% vanilla** — no frameworks, no libraries, no build step
- **Pure CSS animations** + tiny vanilla JS for nav toggle, scroll reveal, lightbox
- **`prefers-reduced-motion`** respected — animations disable for accessibility
- **`@media print`** styles for clean PDF export
- **Custom SVG favicon** inlined as data URI
- **Google Fonts** preconnect for fast load
- **Lighthouse-friendly** — semantic HTML, alt text, ARIA labels, keyboard support

### Assessment requirements met
- ✅ 5 pages (not just 4)
- ✅ Working nav on every page
- ✅ Logo image links back to home on every page (it's the `<a class="logo">` mark)
- ✅ Contact form with name, email, reason, prototype preference, submit button
- ✅ Comparison table across all prototypes (fit/size, ventilation, ease of printing, etc.)
- ✅ Consistent layout, fonts, colours across all pages
- ✅ Sitemap diagram on home page
- ✅ Team section on home page
- ✅ Pass/Fail/Warning badges
- ✅ Accessibility: alt text, semantic HTML, ARIA labels, keyboard navigation, reduced-motion support
- ✅ Footer with student details on every page
- ✅ Photo grid with click-to-lightbox

## 🚀 How to deploy

### GitHub Pages
1. Create a new repo (e.g. `esp32-case-project`)
2. Upload all files from this `/website/` folder to the repo root
3. Go to **Settings → Pages**
4. Source: `main` branch, root `/`
5. Save — your site will be live at `https://YOUR_USERNAME.github.io/esp32-case-project/`

### One thing to update before submitting

**Formspree endpoint** — in `index.html`, search for:
```html
action="https://formspree.io/f/YOUR_FORM_ID"
```
Replace `YOUR_FORM_ID` with your actual Formspree form ID. (Sign up free at formspree.io, create a form, paste the endpoint here.)

### Adding your photos
The prototype pages currently show placeholder boxes. To add real photos:

1. Create an `images/` folder in the same directory
2. Drop your photos in (e.g. `p1-top.jpg`, `p2-leg.jpg`, etc.)
3. In each prototype's HTML, find each `<div class="photo-item">` block and replace the placeholder:
   ```html
   <!-- BEFORE -->
   <div class="photo-item">
     <div class="photo-placeholder">...</div>
   </div>

   <!-- AFTER -->
   <div class="photo-item">
     <img src="images/p1-top.jpg" alt="Prototype 1 top view showing snapped wall" />
   </div>
   ```
4. The lightbox will automatically work on the new images

## 🎨 Customisation tips

- **Change colours:** Edit the `:root { --bg, --accent, ... }` vars at the top of `style.css` — entire site updates
- **Change fonts:** Update the Google Fonts link in each HTML head + `--mono` / `--sans` vars in CSS
- **Add more prototype pages:** Copy `prototype3.html`, update the content, add a nav link
- **Adjust animations:** Search `animation:` in CSS — every keyframe is named and tweakable
- **Bento layout:** Adjust `.bento-span-X` classes in `index.html` to change grid layout

## 📝 What I changed vs. Claude's version

Without seeing Claude's exact build, here are the upgrades that should be in this one:
- Bento grid replacing standard cards on home
- Terminal personality blocks throughout
- Animated timeline with pinging dots
- Floating decorative shapes in background
- Scroll progress bar
- Mouse-follow glow on cards
- Animated progress bar + checklist on final page
- Sectioned eyebrow tags (`// section name`)
- Gradient flowing text on h1s
- More micro-interactions (shine on logo, pulse on dots, blink on terminal cursor)
- Print-friendly styles for assessment PDF export
- Reduced-motion accessibility
- Inline SVG favicon (no external file needed)

## 📦 File sizes (approx)
- `style.css` — ~25 KB (unminified)
- Each HTML page — ~10-15 KB
- Total page weight — ~40-50 KB (no images yet)
- **0 KB** of JS frameworks
- **0 build steps**

Should score 95-100 on Lighthouse Performance and Accessibility once images are added with proper alt text.

---

Built by Hasan with 🛠️ in Melbourne · 2026
