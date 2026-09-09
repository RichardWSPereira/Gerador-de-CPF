# Copilot Instructions

## Project Overview

This is a small Portuguese-language CPF generator built with vanilla JavaScript and Webpack.

## Structure

- `src/main.js`: browser entry point and UI event handling.
- `src/modules/geraCPF.js`: CPF generation logic, including state suffix selection.
- `src/modules/validaCPF.js`: CPF check-digit calculation.
- `src/assets/css/style.css`: application styles.
- `public/index.html`: static page served by the browser.
- `public/assets/js/bundle.js`: generated Webpack output; regenerate it after source changes.

## Development

- Install dependencies with `npm install`.
- Regenerate the bundle with `npx webpack --mode development`.
- Use `npm run dev` for Webpack watch mode.

## Conventions

- Keep user-facing text in Brazilian Portuguese.
- Prefer small, focused changes that preserve the existing vanilla JavaScript and Webpack setup.
- Keep CPF calculation logic in `src/modules/` and DOM interaction in `src/main.js`.
- Do not edit generated bundle output manually; regenerate it from `src/` instead.
- Preserve unrelated working-tree changes.
