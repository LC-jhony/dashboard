# AGENTS.md

## Project

Simple Vite + Tailwind CSS v4 dashboard. No framework, no JavaScript logic — static HTML with Tailwind utility classes.

## Stack

- Vite 8.2
- Tailwind CSS 4.3 (via `@tailwindcss/vite` plugin)
- Alpine.js (loaded via CDN in `index.html`)

## Commands

```bash
npm run dev      # dev server
npm run build    # production build → dist/
npm run preview  # preview production build
```

## Structure

- `index.html` — main entrypoint, contains all markup and inline Alpine.js logic
- `src/input.css` — single CSS file, just `@import "tailwindcss"`
- `vite.config.mjs` — minimal config with Tailwind plugin
- `dist/` — build output

## Conventions

- Tailwind v4: config-free, no `tailwind.config.js`. Customize via `@theme` in CSS if needed.
- Responsive breakpoints: `sm:` (640px), `md:` (768px), `lg:` (1024px)
- Alpine.js for interactivity (dropdowns, toggles). No build step for JS.
- No linting, no tests, no TypeScript configured.
