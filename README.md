# BV Portal — Incoming Call Routing Prototype

Interactive single-file HTML prototype of the Incoming Call Routing page for the BV Portal, covering Schedulers, DIDs, Location Holidays, and Away Mode.

## Preview

Open `index.html` in any modern browser — no build step, no install.

All dependencies (React 18, ReactDOM, Babel Standalone, Tailwind CSS) are loaded from CDNs at runtime.

## GitHub Pages

To publish this prototype as a live URL:

1. Push this repository to GitHub.
2. Go to **Settings → Pages**.
3. Under **Source**, select the `main` branch and the `/ (root)` folder.
4. Save. Your prototype will be available at `https://<your-username>.github.io/<repo-name>/` within a minute or two.

## Files

- `index.html` — the full prototype (React + Tailwind, single file, ~300KB)
- `README.md` — this file
- `.gitignore` — standard ignores

## Development

Edit `index.html` directly. The script block uses `type="text/babel"` so JSX is transpiled in the browser via Babel Standalone. Reload the page to see changes.

For a faster local preview with live reload, you can run any static server, e.g.:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Tabs

- **Schedulers** — create, edit, duplicate, and delete schedulers with time slots (list and calendar views), custom holidays, and DID assignments.
- **DIDs** — table of incoming numbers and their assigned schedulers, with search and inline re-assignment.
- **Location Holidays** — reusable holidays that can be linked to any scheduler.
- **Away Mode** — one-tap forwarding rules for after-hours or out-of-office scenarios.
