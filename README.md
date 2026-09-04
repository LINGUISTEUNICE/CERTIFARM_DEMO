# CertiFarm demo — Vercel deployment

This is a single static file (`index.html`) with no build step and no backend.
Data is saved in each visitor's browser via `localStorage`, so it's a good
pitch demo but not a shared multi-user database — that would need a real
backend later.

## Fastest path: Vercel CLI

1. Install the CLI once: `npm i -g vercel`
2. From inside this folder, run: `vercel`
3. Log in when prompted, accept the defaults (framework: **Other**, no
   build command, output directory: `.`)
4. It deploys and prints a live URL. Run `vercel --prod` to promote it to
   your production domain.

## No terminal? Drag-and-drop

1. Go to https://vercel.com/new
2. Drag this folder onto the page
3. Deploy — same result, no CLI needed

## Prefer GitHub

1. Push this folder to a new GitHub repo
2. On vercel.com, "Add New… → Project" → import that repo
3. Framework preset: **Other**. Leave build command blank, output
   directory `.`
4. Deploy

Any of these works — the file is 100% static, so there's nothing to
configure beyond pointing Vercel at it.
