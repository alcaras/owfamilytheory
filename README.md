# owfamilytheory

Personal strategy notes on **Old World family-class theory** — how to play each
nation's fixed family classes well.

- **`index.html`** — a single standalone page (no build step): one card per nation
  with every valid combo, generated from the rules. Open it locally in a browser.
- **`family-combos.md`** — the written doctrine: framework, capital ratings, the
  rules that drive the choices, and the per-nation combo tables.
- **`CLAUDE.md`** — agent guide for working in this repo.
- **`img/`** — nation crests and family-class icons (extracted from the Old World
  install via the [owreference](https://github.com/alcaras/owreference) pipeline).

## The idea

Each nation is dealt a fixed hand of family classes. You field three: one **cap**
(capital), one **mil seat**, a **third**, and feed at most one **spammer**. The
page enumerates every valid assignment per the doctrine; `index.html`'s
`genCombos()` is the rules made executable.

Facts derive from the game XML (`family.xml`, `familyClass.xml`, `effectPlayer.xml`).
