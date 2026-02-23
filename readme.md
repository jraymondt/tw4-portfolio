# tw4-portfolio

## Quick setup (run at the start of each editing session)

1. Open the project in VS Code.

2. Install dependencies (preferred: pnpm):

```sh
pnpm install
```

### Start the dev server

```sh
pnpm run dev
```

1. Open the site the terminal reports (usually http://localhost:5173).

2. When done, stop the server (Ctrl+C). To verify a production build:

   ```sh
   pnpm run build
   pnpm run preview
   ```

## What this project does (concise)

- The app is a small Vite + Tailwind project that serves the static profile page at [index.html](index.html).
- Layout and content live in [index.html](index.html).
- Styling is in [src/style.css](src/style.css) (imports Tailwind and FontAwesome).
- The JS entry is [src/main.js](src/main.js), which:
  - imports the CSS ([src/style.css](src/style.css)),
  - mounts the UI into `#app`,
  - and wires a simple counter using the exported function [`setupCounter`](src/counter.js).
- The counter logic is implemented in [`setupCounter`](src/counter.js) and increments the button text on click.
- Vite is configured with the Tailwind plugin in [vite.config.ts](vite.config.ts).
- Project scripts are available in [package.json](package.json) (`dev`, `build`, `preview`).

## Important files

- [index.html](index.html)
- [src/main.js](src/main.js)
- [src/counter.js](src/counter.js) — exports [`setupCounter`](src/counter.js)
- [src/style.css](src/style.css)
- [vite.config.ts](vite.config.ts)
- [package.json](package.json)
