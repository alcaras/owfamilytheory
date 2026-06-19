# Old World — family-class combo theory

A per-nation plan for how to play each nation's **fixed** family classes, under
one doctrine: **field three families, one good capital, at most one spammer.**

Family classes are fixed per nation in the game XML — you don't draft them. A
"combo" is the *role assignment* for the families you choose to field.

---

## The model

**You field 3 of the nation's 4 families.** The unpicked family is *out* — no
cities, no effect, no penalties. (Tamil has only 3 families, so it fields all
three; Maurya has 6 and fields 3 of them.)

Your three families fill three roles, plus a spam designation:

- **CAP** — your capital anchor. Must be a good cap.
- **MIL SEAT** — your second seat family, a military one where the roster has it,
  otherwise any seat-class family.
- **THIRD** — the remaining fielded family.
- **SPAM** — **at most one** spammer you actually feed cities. May be the same
  family as CAP (only if the spammer is a good cap), or sit in the THIRD slot.

### The ten classes

| Bucket | Classes | Use |
|---|---|---|
| **Spammers** | Statesmen, Sages, Clerics, Landowners | Reward many cities. Feed only one. |
| **Seat-only** | Champions, Riders, Artisans | Strong from just their seat. |
| **Good-site** | Traders, Hunters, Patrons | Place on the right tile. |

### Capital rating

- **Always-good cap:** Sages, Landowners, Artisans, Patrons
- **Conditional:** Riders (2nd military family) · Hunters (2nd military + resource)
  · Traders (resource). The resource caps (**Traders, Hunters**) are *always
  competitive with the right starting location* — treat them as full options, not
  fallbacks, whenever the cap site has the resource.
- **Workable, not ideal:** Clerics, Statesmen — they *can* be capitals, just not
  your first choice over a good cap.
- **Avoid as cap:** Champions (the only true non-cap)

Military families (the "2nd military family" test) = **Champions, Riders, Hunters.**

### The two rules that actually drive choices

1. **Landowners only matters if you field it.** Only Landowners carries
   `iFewestCitiesOpinion −40` (`familyClass.xml`); the other spammers merely
   *benefit* from cities and are never penalized for staying small. So:
   - Field Landowners → it is *forced* to be your spam.
   - Don't want to spam Landowners → **leave it out.**
   - **Tamil can't** (only 3 families, Landowners always fielded → always its spam).
     **Egypt can** (4 families → drop Landowners), which frees its whole plan.
   Spammer-class families that *aren't* Landowners (Sages/Clerics/Statesmen) can be
   fielded **unfed** — e.g. Sages sitting as the capital — with no penalty.
2. **Cap = spam is allowed for any spammer** (all four are cap-capable). Ideal with
   **Sages/Landowners**, workable with **Clerics/Statesmen**. When cap = spam, the
   THIRD slot becomes a separate non-spam family; when they differ, the cap is an
   unfed showpiece and the THIRD spammer sprawls. (Champions is the only family that
   can't anchor a capital — and it isn't a spammer anyway.)

---

## The combos

One row per viable option. The **dropped** column is the family left out (its slot
freed); for Maurya, "rest" = the three of six it doesn't field.

| Nation | CAP | MIL SEAT | THIRD | SPAM | dropped |
|---|---|---|---|---|---|
| **Babylonia** | Artisans | Hunters | Sages | Sages | Traders |
| **Babylonia** | Traders | Hunters | Sages | Sages | Artisans |
| | Sages | Hunters | Artisans | Sages | Traders |
| | Sages | Hunters | Traders | Sages | Artisans |
| **Greece** | Artisans | Champions | Sages | Sages | Patrons |
| | Patrons | Champions | Sages | Sages | Artisans |
| | Sages | Champions | Artisans | Sages | Patrons |
| | Sages | Champions | Patrons | Sages | Artisans |
| **Kush** | Artisans | Hunters | Landowners | Landowners | Traders |
| **Kush** | Traders | Hunters | Landowners | Landowners | Artisans |
| **Carthage** | Artisans | Riders | Statesmen | Statesmen | Traders |
| **Carthage** | Traders | Riders | Statesmen | Statesmen | Artisans |
| **Assyria** | Patrons | Champions | Clerics | Clerics | Hunters |
| | Patrons | Hunters | Clerics | Clerics | Champions |
| | Hunters | Champions | Clerics | Clerics | Patrons |
| **Aksum** | Patrons | Champions | Clerics | Clerics | Traders |
| **Aksum** | Traders | Champions | Clerics | Clerics | Patrons |
| **Hittite** | Patrons | Riders | Landowners | Landowners | Traders |
| **Hittite** | Traders | Riders | Landowners | Landowners | Patrons |
| **Rome** | Patrons | Champions | Landowners | Landowners | Statesmen |
| | Patrons | Champions | Statesmen | Statesmen | Landowners |
| **Persia** | Riders | Hunters | Clerics | Clerics | Statesmen |
| | Hunters | Riders | Clerics | Clerics | Statesmen |
| **Yuezhi** | Riders | Champions | Clerics | Clerics | Traders |
| **Yuezhi** | Traders | Riders | Clerics | Clerics | Champions |
| **Yuezhi** | Traders | Champions | Clerics | Clerics | Riders |
| **Maurya** | Patrons | Riders | Sages | Sages | rest |
| | Riders | Champions | Sages | Sages | rest |
| | Hunters | Champions | Sages | Sages | rest |
| | Sages | Riders | Patrons | Sages | rest |
| **Tamil** | Artisans | Landowners | Traders | Landowners | — |
| **Egypt** | Sages | Riders | Clerics | Clerics | Landowners |
| | Sages | Riders | Clerics | Sages | Landowners |
| | Sages | Riders | Landowners | Landowners | Clerics |
| | Landowners | Riders | Clerics | Landowners | Sages |

### Notes

- **Egypt** is free: drop Landowners and spam Clerics or Sages (Sages as an unfed
  cap), or keep Landowners and spam it. Four real lines.
- **Rome** can drop Landowners and spam Statesmen instead — the escape hatch if you
  dislike Landowner-spam.
- **Kush / Carthage / Aksum / Hittite / Yuezhi** have one spammer; they can also
  drop it for a no-spam tall build (all seats/sites) — not listed.
- **Tamil** breaks the framework — it's a **Coalition Nation** (see below), so the
  "cap" isn't a pick. Landowners is always its forced spam (only 3 families, no
  military).
- **Maurya** fields 3 of 6; MIL SEAT is any military family it didn't cap; Statesmen
  is the worse spam alternative to Sages.
- **Yuezhi** has **no always-good cap** — Riders (2nd mil), Clerics (workable) and
  Traders (resource) are all conditional/workable. So a **Traders capital** on a good
  trade/resource site is a co-equal option there, not a fallback.
- Where **CAP = SPAM** (the Sages-cap rows), the capital itself is your spam
  cluster and THIRD is a separate side seat; where they differ, the cap is an unfed
  showpiece and the THIRD spammer sprawls.

### Workable-but-not-ideal: Clerics / Statesmen capitals

Clerics and Statesmen can anchor a capital (cap = spam) — fine as a fallback or for
an economy-capital flavor, just weaker than the good caps above. MIL SEAT swaps
among the nation's military families as usual.

| Nation | CAP | MIL SEAT | THIRD | SPAM | dropped |
|---|---|---|---|---|---|
| **Assyria** | Clerics | Champions | Patrons | Clerics | Hunters |
| **Assyria** | Clerics | Hunters | Patrons | Clerics | Champions |
| **Aksum** | Clerics | Champions | Patrons | Clerics | Traders |
| **Persia** | Clerics | Hunters | Riders | Clerics | Statesmen |
| **Persia** | Clerics | Riders | Hunters | Clerics | Statesmen |
| **Yuezhi** | Clerics | Riders | Traders | Clerics | Champions |
| **Carthage** | Statesmen | Riders | Artisans | Statesmen | Traders |
| **Rome** | Statesmen | Champions | Patrons | Statesmen | Landowners |

---

## Tamil — the coalition exception

Tamil is a **Coalition Nation**: each family has a *Family Control* score (the
number of characters it has in positions of power). Whichever family leads holds
**Supremacy** — **its seat is the capital, its head is your Leader**, and its
player-wide **Supremacy effect** applies. If another family overtakes it, the
throne (and capital) moves. So Tamil's real choice isn't CAP/MIL/THIRD — it's
**which family you let win Control**, i.e. which of three supremacies you run.
Landowners is still the forced spam regardless (only 3 families, no military).

| Supremacy → capital | Class | Supremacy effect |
|---|---|---|
| **Chera** | Landowners | +1 Training / Rural Specialist · free Elephant · Coalition bonus |
| **Chola** | Artisans | +1 Orders / Harbor · +20% Strength in own territory |
| **Pandya** | Traders | +1 Civics / Shrine · unlocks Sangam Literature |

**Chera supremacy** is the natural default: its rural-specialist Training and free
Elephants scale off the Landowner sprawl you're spamming anyway. Chola gives a
defensive/economy capital; Pandya a civics/culture one.

Opening order (play experience): an Artisans capital feels weak early since its
luxury/culture bonuses come online late. On bigger maps you can open with
**Traders**; otherwise start the **Landowners** seat first and take **Artisans**
next, leaning on those until the Landowners seat has some rurals worked in.

Source: `family.xml` (`SupremacyEffectPlayer`), `effectPlayer.xml`,
`CONCEPT_COALITION_NATION` help text.

---

## Roster reference (fixed family classes per nation)

| Nation | Families (class) | DLC |
|---|---|---|
| Assyria | Champions, Hunters, Patrons, Clerics | base |
| Babylonia | Hunters, Artisans, Traders, Sages | base |
| Carthage | Riders, Artisans, Traders, Statesmen | base |
| Egypt | Riders, Landowners, Clerics, Sages | base |
| Greece | Champions, Artisans, Patrons, Sages | base |
| Hittite | Riders, Landowners, Patrons, Traders | base |
| Persia | Clerics, Hunters, Riders, Statesmen | base |
| Rome | Champions, Landowners, Patrons, Statesmen | base |
| Aksum | Champions, Traders, Clerics, Patrons | Aksum |
| Kush | Hunters, Artisans, Traders, Landowners | Pharaohs of the Nile |
| Maurya | Champions, Hunters, Statesmen, Sages, Patrons, Riders | Empires of the Indus |
| Tamil | Traders, Artisans, Landowners | Empires of the Indus |
| Yuezhi | Riders, Champions, Clerics, Traders | Empires of the Indus |

Source: `family.xml` / `familyClass.xml` in the Old World install, as projected by
the owreference pipeline (`../owreference/src/data/nations.json`).
