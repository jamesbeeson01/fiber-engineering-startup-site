# Fiber Design Automation — website

Static, single-page site for showing prospective clients. Plain HTML + CSS, no build step.

## Preview

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

## Edit

| What | Where |
|---|---|
| Team photos | `assets/team/` (see README there) |
| Credential badges / logos | `assets/credentials/` (see README there) |
| Bios, credentials, contact details, location | `index.html` — every placeholder has `class="todo"` and shows **highlighted yellow** on the page |
| Company name | search for `Fiber Design Automation` |
| Colors / fonts | top of `styles.css` |

Before showing the site to anyone, search `index.html` for `todo`, `EDIT`, `REVIEW` and `CONFIRM`. Nothing highlighted yellow should remain.

## Deploy

Any static host works. Simplest: GitHub Pages (Settings → Pages → deploy from branch, root folder).

## Next step

See [`HANDOFF.md`](HANDOFF.md): what was deliberately left out of the site, and how to run the `grill-me` review in Claude Code.
