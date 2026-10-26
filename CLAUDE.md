# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Status

StockyApp is currently the unmodified `create-vue` starter (Vue 3 + Vite, plain JavaScript, no router/store/tests/linter). `src/components/` (HelloWorld, TheWelcome, WelcomeItem, icons) is still scaffold demo code; there is no app-specific logic yet.

## Commands

Requires Node `^22.18.0 || >=24.12.0`.

- `npm install` — install dependencies
- `npm run dev` — Vite dev server with HMR (includes `vite-plugin-vue-devtools`)
- `npm run build` — production build to `dist/`
- `npm run preview` — serve the production build
- `npm run format` — Prettier over `src/` (no semicolons, single quotes, 100-col width)

There is no test runner or linter configured.

## Structure

- Entry: `index.html` → `src/main.js` (mounts `App.vue` on `#app`, imports `src/assets/main.css`).
- `@` is aliased to `src/` in both `vite.config.js` and `jsconfig.json`; keep the two in sync if changed.
