# Trailside Tales — Tour 1 (draft site)

**Local draft only.** Nothing here is published. Do not push or go live until Dave says so.

## What this is

A mobile-first static page for **Trailside Tales, Tour 1: Where the Trail Meets the Lake** — Harrison trailhead (mile 15.3) south ~7–7.5 miles to Chatcolet Bridge / Heyburn State Park.

- Written by Dave (Harrison, Idaho)
- Narrated by a computer voice (Chatterbox) — disclosed on the page
- Tap-to-play HTML5 audio (no auto GPS in this draft)
- Approximate OpenStreetMap map with two pins (trailhead + bridge only)

## Preview locally

From this folder:

```bash
cd /workspace/trailside-tales/site
python3 -m http.server 8080
```

Then open `http://localhost:8080/` in a browser.

Or open `index.html` directly (some browsers restrict local audio/`file://`; the tiny server above is more reliable).

## Files

```
site/
  index.html          # the tour page
  README.md           # this file
  audio/
    00-intro.mp3
    01-stop1.mp3 … 10-stop10.mp3
    11-outro.mp3
```

All paths are relative so the folder works as a static site.

## Publish later to GitHub Pages (steps only — do not do this yet)

1. Create a new empty public GitHub repo (e.g. `trailside-tales-tour1`) when Dave approves.
2. Copy the contents of this `site/` folder into the repo root (or a `/docs` folder).
3. Commit and push.
4. In the repo: **Settings → Pages → Source**: Deploy from branch `main` (root or `/docs`).
5. Wait a minute; open the `*.github.io` URL Dave gets.
6. Keep `noindex` until reviews are done and Dave wants it findable; then remove the robots meta if desired.

**$0 stack:** GitHub Pages is free for public repos. Leaflet + OSM tiles are free. No paid APIs, no sign-ups required for riders.

## Before going live

Dave still needs to approve:

- Publishing (repo + Pages on)
- Pending reviews: Crane Historical Society (stops 3–6) and Coeur d’Alene Tribe cultural staff (stops 7, 8, 10, and Schitsu'umsh pronunciation)

## Map pin sources (approximate)

| Pin | Approx. coords | Source |
|---|---|---|
| Harrison trailhead | 47.4547, −116.7868 | Public trail place listing near mile 15.3 |
| Chatcolet Bridge | 47.3782, −116.7536 | HistoricBridges.org Bridge Locator |

Mid-route stops use text landmarks only — no invented GPS pins.
