# 🛠️ ESP32-C3 Zero — Protective Case Project

> A multi-page website documenting the full design-and-build journey of a 3D-printed protective case for the **ESP32-C3 Zero** microcontroller — from three failed prototypes to a working, tested final design.

**Student:** Hasan Kandemir · **ID:** 100376427
**Course:** ICT30120 Certificate III in Information Technology
**Unit:** ICTWEB304 — Build simple web pages
**Project type:** Team design project (BSBXTW301 — Work in a team)

---

## 📖 About the project

The goal was to design and 3D-print a protective case for the ESP32-C3 Zero so the board is safe to handle and use in a classroom environment. The case had to:

- Fit the ESP32-C3 Zero correctly
- Protect the board during normal classroom use
- Allow access to the **USB-C port, GPIO pins and buttons**
- Include **ventilation holes** for airflow and cooling
- Be strong enough for everyday handling and printable on classroom equipment

The project was completed iteratively across **four versions**, each one fixing the problems found in the last. The final design — selected as the team's combined solution — passed all testing criteria.

---

## 🧭 The design journey

| Version | Date | Print Time | Material | Cost | Result |
|---------|------|-----------|----------|------|--------|
| Prototype 1 | 26/05/2026 | 12m 57s | 3.02 g | $0.09 | ❌ Fail |
| Prototype 2 | 01/06/2026 | 20m 1s | 4.25 g | $0.13 | ❌ Fail |
| Prototype 3 | 02/06/2026 | 28m 49s | 6.19 g | $0.19 | ⚠️ Needs Improvement |
| **Final Design** | **09/06/2026** | **34m 21s** | **9.03 g** | **$0.23** | ✅ **Pass** |
| **Totals** | — | **1h 36m 8s** | **22.49 g** | **$0.64** | — |

**Key fixes along the way:** corrected internal dimensions and tolerances, thicker walls, correct print orientation, larger GPIO pin slots, added ventilation, and a redesigned snap-fit lid. The final design adds wall-mounting, a removable lid for easy chip access and controller-style buttons.

---

## 📁 Project structure

```
.
├── index.html         # Home — overview, stats, prototype timeline, comparison table, team
├── prototype1.html    # Prototype 1 — first failed print
├── prototype2.html    # Prototype 2 — second failed print
├── prototype3.html    # Prototype 3 — fits and clips, one fix needed
├── final.html         # Final design — selected, printed, tested and passed
├── style.css          # Shared stylesheet (no frameworks)
├── images/            # Prototype + final design photos (p1_*, p2_*, p3_*, f1_*)
└── README.md          # This file
```

---

## ✨ Website features

- **5 linked pages** with consistent navigation, fonts and colours
- **Comparison table** across all prototypes (fit, ventilation, lid system, port access, cost, result)
- **Photo galleries** with click-to-enlarge lightbox on every prototype and the final design
- **Pass / Fail / Needs-Improvement status badges** throughout
- **Improvement log** and **product requirements checklist** on the final page
- **Responsive design** — works on desktop and mobile (hamburger menu)
- **Accessibility** — semantic HTML, alt text on all images, ARIA labels, keyboard support and reduced-motion handling
- **Footer with student details** on every page

---

## 🧰 Built with

- **HTML5 + CSS3** — no frameworks, no libraries, no build step
- A small amount of **vanilla JavaScript** for the navigation menu, scroll-reveal animations and lightbox
- **Google Fonts** (Syne + Space Mono)

---

## 🚀 Viewing the site

**Locally:** download the repository and open `index.html` in any web browser.

**Live (GitHub Pages):** Settings → Pages → deploy from this branch (root `/`).

---

Built by Hasan Kandemir · Melbourne, Australia 🇦🇺 · 2026
Submitted under ICTWEB304.
