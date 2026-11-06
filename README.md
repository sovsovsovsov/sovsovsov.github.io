# Four Lane Rush

A 4-key (A S K L) rhythm game in the style of osu!mania. One file (`index.html`), no dependencies, no audio assets: the song is synthesized live with the Web Audio API.

## Play

- Keys: **A S K L** (or tap the lanes on a touch screen)
- Hold notes: keep the key down until the tail reaches the line, then release
- **Esc** pauses
- Menu settings: scroll speed, audio offset (nudge if hits feel early or late), volume

## Charts

Three charts for the same song ("Neon Static", 140 BPM, ~1:45):

| Chart  | What to expect |
|--------|----------------|
| Easy   | Beat-aligned taps, occasional holds and jumps |
| Normal | Eighth-note rhythms, chords, longer holds |
| Hard   | Sixteenth streams, jumps, triples, jacks |

Charts are generated from seeded patterns in `index.html`, so they are identical on every load. Tweak the `DIFFS` table near the top of the script to change density or patterns.

## Publish on GitHub Pages

1. Create a new GitHub repository.
2. Add `index.html` (and this README) to the root of the `main` branch.
3. Go to **Settings > Pages**, set **Source** to "Deploy from a branch", choose `main` and `/ (root)`, then Save.
4. After a minute your game is live at `https://<your-username>.github.io/<repo-name>/`.
