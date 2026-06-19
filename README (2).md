# StreamFlix 🎬

A Netflix-inspired streaming platform UI clone built with pure HTML, CSS, and JavaScript — no frameworks, no dependencies.

---

## 📌 Overview

StreamFlix is a pixel-faithful recreation of Netflix's core browsing interface. It replicates the visual design language, layout structure, and interactive behaviors of a modern streaming platform using only vanilla web technologies.

---

## ✨ Features

- **Fixed Navbar** with scroll-triggered background transition
- **Hero Section** with gradient backdrop, metadata tags, and action buttons
- **Dynamic Content Rows** generated via JavaScript from a data array
- **Horizontal Scroll** with smooth arrow navigation (‹ ›)
- **Card Hover Effects** — scale + lift animation on mouse-over
- **Top 10 Row** with oversized rank numbers overlay
- **Responsive Design** — adapts to mobile and desktop viewports
- **Footer** with multi-column link grid

---

## 🛠️ Tech Stack

| Technology | Usage |
|------------|-------|
| HTML5 | Page structure and semantics |
| CSS3 | Styling, animations, responsive layout |
| Vanilla JavaScript | DOM generation, scroll effects, interactions |

> No libraries. No frameworks. No build tools.

---

## 📁 Project Structure

```
streamflix/
└── index.html       # Single-file app (HTML + CSS + JS)
```

---

## 🚀 Getting Started

### Run Locally

1. Clone or download the repository
2. Open `index.html` in any modern browser

```bash
git clone https://github.com/your-username/streamflix.git
cd streamflix
open index.html
```

No installation or server required.

---

## 🎨 UI Components

### Navbar
- Fixed positioning with `z-index` layering
- Transparent by default → solid black (`#000`) on scroll via JS scroll listener
- Logo, nav links (Home, TV Shows, Movies, New & Popular, My List), search, bell, and profile avatar

### Hero Section
- Full-viewport gradient background using layered CSS `linear-gradient` and `radial-gradient`
- Metadata tags (genre, year, category)
- Play and More Info buttons with active press animation

### Content Rows
Rows are generated dynamically from `rowDefs` array:

```js
const rowDefs = [
  { title: "Trending Now",                          ranked: false },
  { title: "Top 10 Today",                          ranked: true  },
  { title: "New Releases",                          ranked: false },
  { title: "Critically Acclaimed Dramas",           ranked: false },
  { title: "Because You Watched Midnight Frequencies", ranked: false }
];
```

- Each row renders 16 cards with gradient backgrounds
- `ranked: true` rows add oversized rank numbers (1–10)
- Arrow buttons scroll the track by 600px per click

### Cards
- Gradient thumbnail placeholders (10 unique palettes)
- Title label with bottom gradient overlay
- Hover: `scale(1.12) translateY(-10px)` with elevated shadow
- Click: alert with title name (demo behavior)

---

## 📱 Responsive Behavior

| Breakpoint | Changes |
|------------|---------|
| `≤ 760px` | Nav links hidden |
| `≤ 600px` | Hero font size reduced, cards shrink to 160×90px, footer grid switches to 2 columns |

---

## 🎨 Color Palette

| Variable | Hex | Usage |
|----------|-----|-------|
| `--red` | `#e50914` | Logo, accent |
| `--black` | `#141414` | Page background |
| `--dark` | `#000000` | Scrolled navbar |
| `--gray` | `#808080` | Footer text, muted UI |
| `--white` | `#ffffff` | Primary text |

---

## 🔮 Possible Enhancements

- [ ] Modal popup with trailer preview on card click
- [ ] Search bar with live filter across card titles
- [ ] "My List" toggle (add/remove from list)
- [ ] Dark/Light mode toggle
- [ ] Skeleton loading animation for cards
- [ ] Persistent state via `localStorage`

---

## 📄 License

This project is built for **educational and portfolio purposes only**.  
StreamFlix is not affiliated with or endorsed by Netflix, Inc.

---

## 👨‍💻 Author

**Karthik**  
B.Tech CSE — The Apollo University, Chittoor  
Frontend Development Intern — Alfido Tech

> *Part of the Alfido Tech Internship Task Series*
