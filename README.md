# Glowinn — Made for Modern Elegance

A full-viewport video hero landing page: floating pill navbar, centred hero over a
looping forest-floor video, and moss-tinted glass cards along the bottom of the frame.

React + Vite (JSX). Dependencies: `react`, `react-dom`, `@vitejs/plugin-react`, `vite`.

## Setup

Requires Node.js 20.19+ (or 22.12+) for Vite 7.

```
npm install
npm run dev
```

## The hero video

The page expects `public/hero.mp4`. It is intentionally **not** hotlinked from the
template library's storage — that URL appears nowhere in this project. Download the
asset once and serve it from your own hosting like any other asset you own:

```
curl -L -o public/hero.mp4 "<hero video URL from the build prompt>"
```

Until the file exists, the hero falls back to its radial forest-green gradient and
everything else renders normally.

## Structure

```
index.html
vite.config.js
public/favicon.svg
public/hero.mp4              <- download this
src/main.jsx
src/App.jsx
src/styles/globals.css       tokens, reset, .shell, .sr-only, .btn + pearl/ink variants
src/components/Navbar.jsx + Navbar.css
src/components/Hero.jsx  + Hero.css
src/components/icons.jsx
```
