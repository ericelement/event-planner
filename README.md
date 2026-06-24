# Event Designer — MTF Biologics booth

A glassCanopy planning + pitch toolkit for the MTF Biologics trade-show booth ("Touch the Difference"). Three self-contained HTML files plus the booth artwork.

## What's here

| File | What it is |
|---|---|
| [`mtf-event-canvas.html`](mtf-event-canvas.html) | **The event builder.** A liquid-node canvas of the campaign on a Past → Present → Future timeline. Splat a phase open to burst its tactics out; click any glob to bring it into focus (presentation), then the ✎ icon to edit it in place. Drag tray tactics in to add them, or drag a placed glob between phases to move it. Carries the campaign theme, per-tactic **timing**, **target lists**, and **conversation/messaging** tracks, plus a **Plan** view (schedule + roll-ups). Saves to `localStorage`. |
| [`renuva-booth-pitch-deck.html`](renuva-booth-pitch-deck.html) | **The pitch deck.** A 14-slide walkthrough of the booth concept, each slide anchored on a booth image. Arrow keys / swipe to navigate. |
| [`gc-live-events-philosophy.html`](gc-live-events-philosophy.html) | **The philosophy deck.** glassCanopy's point of view on live events — the "how we think" companion to the booth pitch. |
| [`mtf-booth-concept-and-prompts.md`](mtf-booth-concept-and-prompts.md) | The written concept, multi-angle booth description, and image-generation prompts. |
| `assets/` | The 10 booth illustrations (clean filenames) used by the apps and deck. |
| `Booth images/` · `editorial cartoons for MTF booth preso/` | Original source artwork. |

## Running it

The HTML files reference local images, so browsers block them on `file://`. Serve the folder over HTTP:

```bash
cd "Event Designer"
python3 -m http.server 8000
# then open http://localhost:8000/mtf-event-canvas.html
```

The decks (`renuva-booth-pitch-deck.html`, `gc-live-events-philosophy.html`) also work opened directly, but the booth images only load when served.

## Brand

glassCanopy enterprise-light system — cool glass-white (`#F6F9FA`), teal (`#2EAABB`), deep navy (`#05162A`), DM Sans. Booth artwork is editorial-cartoon with a teal + warm-wood palette and one warm-orange focal object per frame.
