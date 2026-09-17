# Sasha Astiadi — Homepage

Responsive homepage for Sasha Astiadi (sashaastiadi.site) built with semantic HTML and SCSS using BEM methodology. Dark-mode skin matching the live site.

## View the site (no build required)

The compiled stylesheet `dist/main.css` is included in the project, so no build step is needed to view the page. Either:

- Open `src/index.html` directly in a browser, or
- Serve the project folder with any static file server and visit `/src/` (e.g. `npx live-server --open=src/`)

> **Note:** `dist/main.css` must stay in the project — the page links to it directly. Keep it when copying or zipping the project.

## Prerequisites

- [Node.js](https://nodejs.org/) — only needed for rebuilding the SCSS or running the dev script
- [`live-server`](https://www.npmjs.com/package/live-server) — `npm install -g live-server` (only needed for `npm run dev`)

## Install

```bash
npm install
```

## Build

```bash
npm run build
```

Compiles `src/scss/main.scss` to `dist/main.css`. To rebuild automatically while editing SCSS:

```bash
npm run watch
```

## Run locally

```bash
npm run dev
```

Opens http://127.0.0.1:8080/src/ in your browser. The project root is served (not `src/`) because the page references `../dist/main.css`.

## Structure

- `src/index.html` — semantic page markup
- `src/img/` — local image assets
- `src/scss/base/` — resets and foundational styles
- `src/scss/blocks/` — BEM component styles
- `src/scss/utils/` — variables and mixins
- `dist/main.css` — compiled CSS
- `package.json` — build scripts and dependencies (reviewers can run `npm install` if needed)

## Packaging for submission

Zip the project folder as `sasha_astiadi_homepage.zip`. The zip must include `dist/main.css`, `src/` (`index.html`, `img/`, `scss/`), and `package.json`. Exclude `node_modules/` and `project_requirements/`.

Content, imagery, and branding are sourced from https://sashaastiadi.site/.
