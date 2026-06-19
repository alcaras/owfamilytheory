# CLAUDE.md — owfamilytheory

Personal strategy notes (alcaras) on **Old World family-class theory**: how to
play each nation's fixed family classes well. Not code — a small, evolving set of
markdown analyses. The flagship is [`family-combos.md`](family-combos.md).

## What this is

A doctrine for assigning *roles* to a nation's families, since family classes are
**fixed per nation** in the game XML (you don't draft them). See `family-combos.md`
for the full model, the per-nation combo table, and the roster reference.

## The model (don't relitigate without being asked)

- **Field 3 of the nation's 4 families.** The unpicked family is *out* — no cities,
  no effect, no penalties. Tamil fields all 3 it has; Maurya fields 3 of 6.
- Roles: **CAP** (capital anchor, must be a good cap) · **MIL SEAT** (second seat,
  military where the roster has one, else any seat family) · **THIRD** · **SPAM**
  (at most one spammer you feed; may equal CAP when the spammer is a good cap).
- **Buckets:** Spammers = Statesmen, Sages, Clerics, Landowners (feed only one).
  Seat-only = Champions, Riders, Artisans. Good-site = Traders, Hunters, Patrons.
- **Always-good caps:** Sages, Landowners, Artisans, Patrons. **Workable, not
  ideal:** Clerics, Statesmen (can be capitals). **Avoid as cap:** Champions only.
  **Conditional:** Riders/Hunters (need a 2nd military family), Traders/Hunters/
  Patrons (need a resource).
- **Military families:** Champions, Riders, Hunters.

### Two rules that drive the choices

1. **Landowners only matters if you field it.** Only Landowners has
   `iFewestCitiesOpinion −40`; the other spammers are never penalized for staying
   small. Field Landowners → it's *forced* to be your spam; don't want that → leave
   it out. Tamil can't (only 3 families); Egypt can (drop it). A non-Landowners
   spammer can be fielded **unfed** (e.g. Sages as the cap).
2. **Cap = spam is allowed for any spammer** (all four are cap-capable) — ideal with
   Sages/Landowners, workable with Clerics/Statesmen. When cap ≠ spam, the cap is a
   separate family and the spammer sits in THIRD.

### Table conventions

- Columns: CAP · MIL SEAT · THIRD · SPAM · dropped. One row per viable option.
- **No parentheticals inside table cells** — keep qualifiers in notes below.
- Reference families by class name (Sages, Landowners, …), not internal IDs.

## Ground rules

- **Facts come from the game XML**, same source as the owreference site
  (`../owreference/reference/XML/Infos/` → `family.xml`, `familyClass.xml`; built
  `../owreference/src/data/nations.json`). Verify any number against XML before
  writing it down.
- Markdown only, plain text, no build step.
- When a patch changes a nation's family classes, re-derive from `../owreference`
  (it resyncs from the Steam install each patch) and update the roster + rows.
