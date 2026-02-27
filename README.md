# Nalgonda Biggest Rang – Holi Fest 2026

This is a clean, responsive, single-page landing site for the Holi festival.

## Tech stack
- HTML5, CSS3, JavaScript
- **Tailwind CSS** (installed locally via npm/PostCSS)
- No backend; purely static

> **Note:** earlier versions used the CDN for Tailwind. For production or build environments, Tailwind is compiled as a PostCSS plugin using the CLI. The CDN is not suitable for production.

## Setup & build
1. Open a terminal at the project root.
2. Install dependencies:
   ```bash
   npm install
   ```
3. Build the CSS once or watch for changes:
   ```bash
   npm run build:css      # one‑time production build (minified)
   npm run watch:css      # development mode with auto-rebuild
   ```
   The generated stylesheet will be written to `styles.css`.

4. Open `index.html` in your browser or serve via a simple HTTP server:
   ```bash
   npx http-server .
   # or python -m http.server 8000
   ```

## Folder structure
```
holi website/
├─ index.html             # single-page markup
├─ styles.css             # generated output (don't edit directly)
├─ package.json           # npm config & scripts
├─ tailwind.config.js     # specifies files to scan for class usage
├─ postcss.config.js      # PostCSS plugins config
├─ src/
│  └─ styles.css          # Tailwind directives + custom CSS (source)
└─ README.md
```

## Customisation
- Update the booking URL in `index.html` to the District link (e.g. `https://link.district.in/DSTRKT/nb9gcdto`).
- Add real images to the gallery grid by replacing the `.gallery-item` placeholders with `img` elements or background images.
- Customize the `#schedule` section with the actual event timings and details.
- The site now features a fixed, translucent navigation bar with smooth scrolling, responsive hamburger menu for mobile, and new Gallery & Schedule sections.
- Hero section has a full‑screen background image with overlay, dual CTAs, and decorative wave.
- Highlight cards include icons, headings use gradient text, and gallery shows real photos from Unsplash.
- Schedule entries display icons and the overall layout has improved spacing and visual hierarchy.
- The hero section now has animated color splashes, gradient backgrounds, and custom typography for a festive appearance.
- Highlight cards include accent bars and soft shadows.
- Buttons use a vibrant gradient;&nbsp;modify colors easily in `src/styles.css`.
- Feel free to tweak fonts, spacing, or add additional decorative elements by editing `src/styles.css` or adjusting the Tailwind config.

## Deployment
Since this is a static site, you can deploy the directory to any static hosting provider (GitHub Pages, Netlify, Vercel, etc.). Ensure you run the CSS build step before deployment so `styles.css` is up to date.

---
Happy Holi! 🎨