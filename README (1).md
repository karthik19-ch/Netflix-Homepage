# StreamFlix — Netflix Homepage UI Clone

A front-end clone of the Netflix homepage built with plain **HTML, CSS, and JavaScript** — no frameworks, no build tools, single file.

> ⚠️ This is a UI/UX demo for educational purposes only. It is **not affiliated with Netflix**. All branding, titles, and artwork are original/placeholder content (gradient thumbnails, fictional show names).

---

## Features

- **Sticky navbar** — transitions from transparent to solid black on scroll, with nav links and profile avatar
- **Hero banner** — full-width gradient backdrop with title, genre tags, description, and "Play" / "More Info" buttons
- **Horizontal content rows** — multiple scrollable carousels (Trending Now, Top 10 Today, New Releases, etc.)
  - Hover-to-zoom card effect, just like Netflix
  - "Top 10" row displays large rank numbers
  - Left/right arrow buttons appear on hover to scroll each row
- **Interactive demo actions** — clicking a card or hero button shows a "Now Playing" alert
- **Responsive layout** — adapts nav, hero text, footer grid, and card sizes for mobile screens

---

## Tech Stack

| Layer | Tech |
|-------|------|
| Structure | HTML5 |
| Styling | CSS3 (Flexbox, CSS variables, gradients, transitions) |
| Behavior | Vanilla JavaScript (DOM generation, scroll events, click handlers) |

No external libraries, frameworks, or build steps required.

---

## Project Structure

```
.
├── index.html   # Full app — HTML, CSS, and JS in a single file
└── README.md    # This file
```

---

## How to Run

1. Download `index.html`.
2. Open it directly in any modern web browser (Chrome, Firefox, Edge, Safari).

That's it — no server, no dependencies, no build process needed.

### Optional: Run via local server
If you prefer serving it locally (e.g. to avoid any browser file:// restrictions):

```bash
# Python 3
python -m http.server 8000

# then open
http://localhost:8000
```

---

## Customization

- **Rows & titles** — edit the `titles` and `rowDefs` arrays in the `<script>` section to change carousel content.
- **Thumbnail colors** — edit the `palettes` array (CSS gradients used as placeholder posters).
- **Hero content** — edit the text inside `.hero-content` in the HTML.
- **Branding** — change `.logo` text/color and the `--red` CSS variable for a different accent color.

---

## Possible Enhancements

- Search overlay / modal
- Hover preview modals with "more info" details
- Mobile hamburger menu for nav links
- Real image thumbnails via an API (e.g. TMDB)
- "My List" persistence using localStorage

---

## License

This project is provided for educational/demo purposes. Not affiliated with, endorsed by, or connected to Netflix in any way.
