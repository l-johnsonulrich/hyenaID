# Hyena ID

A phone/tablet replacement for the ID binders. Left photo on top, right photo on bottom,
text overlay you type yourself. Works with no signal once installed.

## Files

| File | What it is |
|---|---|
| `index.html` | The whole app |
| `manifest.json`, `sw.js`, `icon-*.png` | Makes it installable and work offline |
| `LING-sample.json` | LING, KCM North subadult, both photos — for testing import |

## Put it online

1. New GitHub repo, e.g. `mara-hyena-project/hyena-id`.
2. Drag all six files into it (web browser is fine, no git needed).
3. Settings → Pages → Deploy from branch → `main` / root.
4. Wait a minute, then open `https://<org>.github.io/hyena-id/` on a phone.

**Install to the home screen.** iPhone: Share → Add to Home Screen. Android: menu → Install app.
It must be added to the home screen to run full screen and to hold its photos reliably.

## Using it

**Browse** — pick a clan, pick an age–sex class, then:

- swipe **up / down** — next or previous hyena
- swipe **left / right** — alternate photos of the same hyena, different angle or light
- **tap the photo** — hide the text, tap again to bring it back
- arrow keys and space do the same on a laptop

**Add a hyena** — from the class list, hit `+`. Type whatever you want overlaid on the photo.
None of it is checked or connected to anything. Add left photos, add right photos.
Photos shrink to 1600px on the phone before they are saved, so a full-size camera JPEG is fine to hand it.

**Set the default photo** — in the edit screen, tap any photo to move it to first position.
First is what you see when you land on the hyena; the rest are the sideways swipes.

**Move a hyena between folders** — edit it, change the Clan or Class dropdown, save. Photos follow.

**Test import** — Library (gear icon) → Import library file → pick `LING-sample.json`.
LING appears under KCM North → Subadults.

## Sharing between devices

Right now each device holds its own copy.

- Library → **Export library file** writes one file with every hyena and photo.
- On the other device, Library → **Import library file**.
- Same name in the same folder gets replaced; everything else is added.

Over camp WiFi this is AirDrop or a shared folder. It is manual, and two people editing the
same hyena the same day will clobber each other. Fine for a season, not fine forever.

## Known limits

- Storage is per device and per browser. Erasing site data erases the library. Export
  after any big session, and keep that file somewhere that gets backed up.
- iOS can evict data from a site that has not been opened in a few weeks. Adding it to
  the home screen makes this much less likely, but keep the export.
- High-ISO photos compress badly. LING's right photo came out 660 KB against 259 KB for
  the left, purely from grain. Budget roughly 300–700 KB per photo.
