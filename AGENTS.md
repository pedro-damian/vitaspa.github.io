# AGENTS.md

## What this is

Static single-page website for VitaSpa (spa in Lima, Peru). No build system, no package manager, no tests, no CI.

## Structure

- `index.html` — the entire site (HTML + inline CSS + inline JS + Tailwind CDN)
- `js/css/estilos.css` — empty, unused
- `assets/` — empty, unused

## Architecture

- SPA-style navigation via `showPage(id)` — toggles `div.page` elements by showing/hiding `.active` class
- `showServiceDetail(serviceId)` is an alias for `showPage()`
- All styling is Tailwind CSS via CDN + inline `<style>` block
- All JS is inline `<script>` at bottom of `index.html`
- Language is Spanish (es), currency is Peruvian Soles (S/)

## Working on this repo

- Edit `index.html` for any changes — it's the only file that matters
- Open `index.html` in a browser to preview (no dev server needed)
- Images are loaded from Unsplash CDN — no local image assets exist
- Contact form submission is faked with `alert()` — no backend
