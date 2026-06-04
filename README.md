# LIF GTM — Love It Forward

A 14-scene merchant sales deck for **LIF** (Love It Forward) — word-of-mouth infrastructure that turns "you have to try this" into a measurable growth channel.

A single-page HTML slideshow. No build step, no framework, no dependencies.

## Deploy (GitHub Pages) — recommended

1. Push this repo to GitHub.
2. Settings → Pages → deploy from branch → root.
3. Open the Pages URL. It serves `index.html` and loads everything in `img/` and `fonts/` automatically.

This is the intended way to view it — over http everything just works.

## Run locally

Browsers block local `file://` asset loading, so don't just double-click `index.html` — serve it:

```bash
# from this folder
python3 -m http.server 8000
# then open http://localhost:8000
```

## Controls

- **← / →** (or space) — previous / next scene
- **Prev / Next** buttons and the scene counter sit fixed at the bottom
- **Replay** — replays the current scene's entrance animation

## The 14 scenes

| # | Scene |
|----|-------|
| 01 | The wound — "Your best customer just sent you three people." |
| 02 | The problem — you can't measure the introduction |
| 03 | The category — word of mouth becomes a channel you can see |
| 04 | The mechanism — the reveal |
| 05 | The proof — the 2020 experiment |
| 06 | Not this — it's not a referral program |
| 07 | The customer experience |
| 08 | The mechanic — six steps |
| 09 | What success looks like — 90-day metrics |
| 10 | Who LIF is for — best-fit segments |
| 11 | The dashboard — animated count-up |
| 12 | The effort — one integration |
| 13 | The network — the graph becomes the product |
| 14 | The close — run a pilot |

## Structure

```
.
├── index.html      ← the entire deck (markup + CSS + JS)
├── img/            ← background imagery + the LIF mark
├── fonts/          ← Graphik (200/300/600/800) + Romana BT
├── README.md
└── .gitignore
```

## Design system

- **Palette** — Air `#FDFCF8`, Warm `#E8DED4`, Ink `#2F2B2B`, Palm `#0C7A4B`, Sol `#FFAC00`, Blue Jean `#006298` (accent), Poppy `#CA0000` (accent). Never pure black.
- **Type** — Graphik for display/body (heavy 800 or light 200/300, no middle weights for key moments); Romana BT italic for the human moments.
- **Motion** — staggered fade-up entrance per scene; print / PDF / reduced-motion fall back to the fully-revealed state.

## Notes

- The Graphik and Romana BT typefaces in `fonts/` are **licensed** — confirm your license before publishing this repo publicly.
- The background photography/illustration in `img/` is placeholder reference imagery — swap in licensed assets before any public or commercial use.
