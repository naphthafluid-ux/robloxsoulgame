# Roadmap — from design to vertical slice

The design phase has done its job (see `GAME_DESIGN.md`). The next
information about this game can only come from something walkable. Order
of operations:

## 1. First greybox (no code) — NOW
- Install Roblox Studio; complete the basic build tutorial.
- Build **one garden room**: a hedge corridor opening into a fountain
  court. Gray boxes, one light source, heavy fog.
- Questions it answers: hedge height/scale, darkness level, whether a
  corridor sightline feels tense. Iterate until walking it feels *right*.

## 2. Reference study (parallel, casual)
- Play **Doors** and re-play **Pressure** with `docs/reference-study.md`
  open; fill in notes. Watch no-commentary runs of **Rooms** and
  **Grace**.
- Goal: internalize the genre grammar (room pacing, tell timing, hide
  verbs) before building our own.

## 3. The Gardener — full design pass (one session, with Claude)
- Take the slice-recommended entity from
  `docs/entity-main-recurring-candidates.md` end-to-end: exact tells and
  timing, detection rules, testimony tiers, encounter pacing.

## 4. Wire it up (Claude writes the code)
- Set up **Rojo** to connect this repo to Studio.
- First scripts: candle pickup, run start/finish loop, Gardener patrol +
  movement-detection, snuff-on-death.
- Division of labor: you build spaces, Claude makes them dangerous.

## 5. Vertical slice — the finish line
One room chain + the Gardener + grab-candle-and-get-out + a bare Refuge,
playable by two people. A friend screaming or laughing in the right place
is the green light for further investment.

## Rule for the whole stretch
No new systems or lore into `GAME_DESIGN.md` until the slice exists —
everything goes to `IDEAS.md`. Ideas invented after touching the real
thing are consistently better.
