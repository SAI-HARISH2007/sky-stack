# Sky Stack — a tap-timing stacker HTML5 playable

**Play it:** https://sai-harish2007.github.io/sky-stack/

A one-tap tower stacker in a single HTML file. No libraries, no build step, HTML5 Canvas only.

1. **The 3-second hook** — "TAP to drop!" over a slow first block; the mechanic teaches itself.
2. **One mechanic** — a block slides back and forth; tap to drop it on the tower. The
   overhang is sliced off and tumbles away, so sloppy taps shrink the tower until a miss
   ends the run.
3. **Pressure** — blocks speed up every floor; perfect drops (within 7px) keep the full
   width, flash a ring, and chain into combos.
4. **The end card** — floor count, a pulsing CTA ("PLAY FREE"), and a replay option.

## Details

- Slice-and-fall physics: overlap interval math decides keep vs. cut; cut pieces fall
  with rotation. Camera eases down as the tower grows; screen shake on sloppy drops.
- Procedural art: hue-cycling buildings with lit windows, drifting parallax clouds, a
  sky gradient that brightens with altitude. Mouse, touch, and spacebar input.
- QA hook for headless testing: `#place=0,-14,10,…` drops blocks at those offsets
  synchronously — used to screenshot-verify stacking, slicing, and the game-over path
  in headless Chromium.
- One `index.html`, zero asset dependencies.

Built in one evening with Claude Code, by Sai Haresh Anand S. Companion to
[Gem Grove](https://github.com/SAI-HARISH2007/gem-grove) (match-3) and
[Pin Rescue](https://github.com/SAI-HARISH2007/pin-rescue) (pull-the-pin).
