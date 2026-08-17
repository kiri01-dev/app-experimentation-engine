# App Experimentation Engine

Live page: https://kiri01-dev.github.io/app-experimentation-engine/

This is a GitHub Pages site published from a git repo that lives inside a larger
working folder (`synthetic data strategy & skills`). Only the files listed below
are tracked — everything else in the folder is ignored via `.gitignore` and never
gets pushed.

## Files tracked in this repo

- `app-experimentation-engine.html` — the actual page content
- `index.html` — a redirect stub so the root URL lands on the page above
- `.gitignore` — restricts git to just these files
- `README.md` — this file

## How to update the published page

1. Edit `app-experimentation-engine.html` in place (e.g. regenerate it from
   `app-experimentation-engine.md` however you normally do).
2. From this folder, run:

   ```bash
   git add app-experimentation-engine.html
   git commit -m "update: <what changed>"
   git push
   ```

3. GitHub Pages rebuilds automatically, usually live within ~1 minute.
   Check build status with:

   ```bash
   gh api repos/kiri01-dev/app-experimentation-engine/pages/builds/latest --jq .status
   ```

## Notes

- The repo is public (required for GitHub Pages on a free plan).
- If you ever want to track another file in this folder (e.g. the diagrams),
  add an explicit `!filename` line to `.gitignore` first, or `git add` will
  silently skip it.
- Remote: `https://github.com/kiri01-dev/app-experimentation-engine` (branch `main`).
