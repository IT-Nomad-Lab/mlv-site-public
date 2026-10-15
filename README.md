# MLV site

Website of the Movimiento Libertario de Venezuela. Static site built with [Astro](https://astro.build) 7.

## Requirements
Node.js 22.12 or newer and npm.

## Commands
| Command | What it does |
| --- | --- |
| `npm ci` | Install dependencies (run once after cloning). |
| `npm run dev` | Start the dev server at `http://localhost:4321`. |
| `npm run build` | Build the static site into `dist/`. |
| `npm run preview` | Serve the built `dist/` locally. |

## Deploy
Build with `npm run build` and serve the contents of `dist/` from any static host. `public/.htaccess` (Apache) serves `404.html` for missing paths and sends a `noindex` header while the site is a demo; remove that header block at launch. `site` in `astro.config.mjs` is the public URL used for `og:image` links.
