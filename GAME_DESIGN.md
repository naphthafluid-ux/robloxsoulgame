# Game Design Document — Working Title: *Soul Game*

> Status: first draft, capturing the core concept. Everything here is open to change.
> Inspired by *Pressure* (Roblox), but with its own identity.
> Platform decision: **Roblox** (see "Why Roblox" at the bottom).

---

## High Concept

Players are the **lost souls of children**, wandering a limbo drawn from old
folklore — a vast **garden-hedge maze** between worlds. **Soul snatchers** and
other entities stalk the maze, each wanting the children for their own
interests. Souls venture into the maze to retrieve a **candle** (placeholder
name) from its center and carry it back out. Every candle brought home makes
the **Refuge** — the communal shelter where all souls gather — a little
warmer and brighter.

**The twist:** knowledge about the entities is not given automatically. It
must be *witnessed* and *carried home alive*. If nobody survives, the
community learns nothing.

---

## What Is Locked (v1)

Only four things are set in stone. Every new idea is tested against them:
*does it break one of these?* If no, it's fair game to explore. If yes, it
goes to `IDEAS.md` (the parking lot) instead of mutating the core.

1. **The fantasy:** you are a lost child's soul that must go into the maze
   and make it back.
2. **The core loop:** Refuge → maze → center → return → deliver candle
   and testimony.
3. **The witness rule:** knowledge only exists if a living witness carries
   it home.
4. **The communal Refuge:** progress is collective and visible.

**The vertical slice** (the real first project — everything else is "after
the slice"): one maze region, one entity, the candle run, and the Refuge in
two states (gloomy / first candle lit).

### The Canon Frame (locked)

The story that opens and closes the loop:

- You die and arrive at the **Refuge**. Someone **welcomes you** — who they
  are is deliberately unknown (see lore hooks below) — and explains the
  rule: *all lost souls must do their part and collect their candle to
  open the gate for their soul.*
- You enter the maze, retrieve **your candle**, and bring it back.
- Doing so **opens your gate**: by canon, you escape the limbo.
- Escaped souls may **choose to return** and remain part of the community
  as the game repeats — this is the in-fiction identity of returning
  players.

Why this frame earns its lock:

- **Diegetic onboarding** — the tutorial *is* the welcome; new players and
  newly-arrived souls are the same thing.
- **The candle has personal stakes** — it is *your* candle, *your* gate,
  not an abstract progress token.
- **Replayability is canon** — veterans are souls who came back to help,
  not people re-queuing.

#### Lore hooks left open (on purpose)

- ~~**Who is the greeter?**~~ — **RESOLVED** (design-side; stays a mystery
  in-game), see "The Rip and the Greeter" below.
- ~~**Personal candle vs. communal 5,000**~~ — **RESOLVED**, see
  "Snuffed Candles" below.

### The Rip and the Greeter (origin lore — decided)

**The limbo, the maze, and the snatchers are real and ancient — the
natural order.** Souls have always wandered the maze until a snatcher
found them and carried them off to whatever comes next — nonexistence,
heaven, unknown. No way home. That is simply how it works, and it was
never meant to be otherwise.

The only *new* thing is the way out. Someone living — a grieving
professor/occultist (era deliberately ambiguous; keep it folklore, not
sci-fi) — dabbled in an afterlife he did not understand and **tore open a
gate into the limbo** for one purpose: to bring his dead son back.

**The greeter is the son — and he refuses to go home.**

- The gate exists to retrieve *him*. The moment he steps through it, the
  professor has what he wanted and **the gate closes behind him — for
  everyone, forever**.
- So he **voluntarily stays**, keeping his father waiting on the other
  side, and uses the rescue built for him to free every other soul
  instead.
- He is **half-aware** — he may not fully remember who he was, or fully
  grasp what he is; but this much he understands: *as long as I don't
  leave, the way out stays open.*
- The rules — one candle per soul, carry it home yourself, snuffed
  candles for the fallen — are *his* rules, but he is **not playing a
  game**. He is earnestly **trying his best to be helpful**; the system
  is flawed only because its maker is a child. Every rule is a sincere,
  imperfect act of care — which is the diegetic explanation for why the
  escape works the way it does.

Consequences for entity design: the snatchers are not connected to the
gate — they are the old order, doing what they have always done. But the
son is still the single point of failure: **lure or drive him through the
gate and it closes for good**. A bargainer-type entity (the Baba Yaga
archetype) that understands this is dangerous in a new way — the deal it
really wants was never with you. And a snatcher taking the son *out* of
limbo entirely would leave the professor holding a gate open for a child
who is no longer there.

#### Soul-candles: why only children (decided)

Every human has a candle — it *is* their soul — and it **melts down as
they age**. Wax is unlived life. The professor's gate works by harnessing
the energy of what remains, and by the teenage years there is already too
little wax left: the gate cannot pull an adult, or even a teenager,
through. Children carry the most unlived life, so **only children's souls
can escape**.

- This grounds the locked fantasy ("you are a lost child's soul") in the
  cosmology instead of leaving it arbitrary.
- It unifies the game's imagery: soul-candles, snuffed candles, wax
  pools — the limbo speaks entirely in wax and flame because souls *are*
  candles.
- Open question: do older souls exist in the limbo — arrivals the gate
  can never take? (See `IDEAS.md`: hub NPCs, possibly an adult.)

**Wax color is sin (decided).** A candle starts **pure white** — a
child's — and darkens with the life's sins, down to pure black. Two axes,
one object: **age shortens the candle, sin darkens it**. A soul's whole
life is legible at a glance from the stub it left behind.

- **The limbo and its snatchers judge by the candle.** What exactly each
  entity does with that judgment is an entity-design axis (prioritize the
  dark? covet the pure? distrust what doesn't match its bearer?) — TBD
  per entity.
- Players' candles are white, or nearly — which may itself be part of
  why the snatchers want children so badly.
- The maze is littered with the **discarded candles of souls that came
  before** — short, darkened stubs the gate could never have taken.
  These double as the game's found light sources (see `IDEAS.md`).

**Player-facing:** this is canon for *us*, a **mystery for players**. The
community should earn it slowly — fragments in testimony, details in the
Refuge, the greeter's slips of memory — over a very long time.

### Snuffed Candles (decided)

When a soul **dies or leaves**, their candle is **snuffed out**. A lit
candle can only ever be carried by its own soul — nobody can open your
gate for you. But snuffed candles can be **recovered and carried home**
by others.

- **Two counters in the Refuge:** lit candles (souls who escaped) and
  snuffed candles (souls who were taken) — an actual memorial. The lobby
  tells both halves of the story: warmth for the ones who made it, dark
  candles for the ones who didn't.
- **Disconnects handled in-fiction:** a player who leaves mid-run simply
  has their flame go out, same as death.
- **Tie-in with the witness system:** the snuffed candle is the *physical
  vessel* of testimony. Candidate rule (to tune): witnessing a snatch
  yields a fragment; recovering and returning the victim's snuffed candle
  delivers the full testimony of how they died. "We have to go back for
  their candle" becomes a real mid-run decision — risk against
  remembrance and knowledge.

**Inventory rule (decided):** each candle — lit or snuffed — takes **one
inventory slot**. Carrying the dead is a real capacity decision, not free
loot.

### Rekindling (revive — decided, implementation open)

If a snatched player **has not yet left the lobby** (still connected,
presumably spectating), their snuffed candle can be **rekindled** to bring
their soul back. Souls that leave are truly gone — this keeps the memorial
honest.

- **The form (decided):** rekindling means **lighting the child's candle
  so it takes the blue flame again** — the soul flame returning to its
  wick is the life returning. A child's candle can never be burned as a
  torch: light it, and what you get is not light but *them*.
- **The method — open.** It requires a **specific, deliberate
  procedure** — not an innate "spirit power" every soul just has.
  What exactly, TBD. Candidates: passing flame from a lit candle
  (vigil-style, soul to soul — makes the candle-bearer even more
  precious), shrines/braziers in the maze, or only at the center flame.
  Mid-run, most players haven't retrieved their own candle yet, so the
  choice shapes the whole rescue play.
- **Testimony interaction:** a rescued soul is the *best possible witness*
  — the victim themselves made it back. Rescue upgrades the knowledge
  system rather than bypassing it.
- **Tuning risk:** death becoming too cheap. Expect limits — a rekindle
  time window, one revive per soul per run, or a cost.
- A rekindled candle never reaches the memorial counter (they came back).

Open mechanical questions:

- How many snuffed candles can one soul carry beyond the slot rule —
  and does carrying them attract anything?
- If nobody recovers a snuffed candle, does it persist in the maze across
  runs (a limbo littered with old failures), or is it lost when the run
  ends?
- Does the memorial counter *do* anything (unlocks, protections, lore
  reveals) or is remembrance itself the reward?

---

## Design Pillars

1. **Someone has to make it back.** Information about entities only enters
   the community record when a living witness returns to the Refuge.
   Survival isn't just personal — it's a duty to everyone else.
2. **The community builds the light.** Progress (knowledge, the Refuge's
   transformation) is collective, not individual. No one player can do it
   alone.
3. **One coherent mythology.** Souls, candles, snatchers, limbo, folklore.
   Every entity, item, and place should feel like it belongs to the same
   old story.

---

## Core Loop

1. Souls gather in the **Refuge** (lobby) and set out into the maze.
2. Navigate the hedge maze; avoid or survive entity encounters.
3. Reach the **center** and take the **candle**.
4. Escape the maze carrying it — the return trip is the second act.
5. Survivors deliver: the candle (Refuge progress) and their **testimony**
   (entity knowledge from what they witnessed).
6. The Refuge grows warmer; the community grows wiser; repeat.

---

## The Knowledge System (the hook)

Contrast with Pressure: there, dying to an entity automatically reveals its
document. Here, **death teaches nothing by itself.**

- **Witnessing a snatch** (an ally taken by an entity) or **surviving an
  encounter** yourself gives you testimony about that entity.
- Testimony only counts if the witness **makes it back to the Refuge alive**.
- Delivered testimony fills in the community's entity records — behavior,
  tells, weaknesses — visible to everyone in the Refuge.

### Open tuning problem (the biggest one)
If everyone dies, nothing is learned, and a struggling community could
stall. Candidate pressure-release valves, to playtest:

- **Partial witnesses:** seeing an encounter from afar yields a fragment;
  a close witness yields more. Records assemble from fragments.
- **Snuffed candles** (decided — see the locked section): the victim's
  extinguished candle remains at the death site and can be recovered and
  carried home as the physical vessel of full testimony. This largely
  supersedes the earlier "echoes" suggestion, or the two can merge (the
  snuffed candle *is* the echo).
- Records could reveal progressively: silhouette → name → behavior →
  weaknesses, over multiple delivered testimonies.
- **Wax pools (candidate):** Dark Souls-style ambient death markers,
  reskinned for our fiction — where many candles have been snuffed,
  melted wax accumulates in pale, layered stains: "many flames went out
  here." No blood needed (fiction- and rating-appropriate). Persisted
  across servers; very feasible on Roblox. Distinct from recoverable
  snuffed candles — wax is permanent ambient data, not an object.

### Open questions
- What mechanically counts as "witnessing"? (Proximity? Line of sight?
  Duration?)
- Is knowledge **per-server** or **globally persistent** across all servers?
  (The 5,000-candle figure suggests global; global knowledge would be a
  striking community experiment.)
- Can players *choose* not to share testimony? (Probably no — keep it
  automatic on return, avoid griefing.)

---

## The Refuge (lobby)

- All souls funnel here between runs, like Pressure's lobby — but it is a
  **living progress meter**.
- Starts dark, gloomy, cold. **Candles brought back decorate it**,
  transforming it stage by stage into a true shelter.
- Milestones are **communal**: e.g. ~5,000 candles for the first small
  change (a tiny candle lights), scaling up from there. Exact numbers TBD
  from playtest data.
- Houses the **entity records** built from delivered testimony.

### Open questions
- Refuge progress: per-server or global?
- What do later Refuge stages *do*? (Cosmetic warmth only, or unlock
  gameplay: new maze regions, tools, blessings?)

---

## The Candle Run (objective)

- The candle sits at the **center of the maze**; runs are in-and-out, not
  one-way.
- *(Suggestion — Claude)* Carrying the candle should have a **cost**: its
  light marks you — perhaps drawing snatchers, perhaps revealing the path,
  perhaps warding lesser things while attracting worse ones. The carrier
  becomes both the most important and the most hunted soul in the maze.
- "Candle" is a placeholder name; the item's true identity/lore TBD.

### Open questions
- One candle per run, or several smaller ones?
- Can the candle be handed off between players (relay under pressure)?
- What happens to a dropped candle when its carrier is snatched?
- ~~Can you carry an ally's candle home for them?~~ **RESOLVED:** no — a
  lit candle answers only to its own soul; on death or leaving it is
  snuffed, and only the *snuffed* candle can be carried home (memorial +
  testimony). See "Snuffed Candles" in the locked section.

---

## Entities / Soul Snatchers

Barely sketched so far — by design, since the knowledge system makes entity
design the heart of the game. Guiding notes:

- Each snatcher wants the children **for its own interest** — they are not
  generic monsters; each has a motive rooted in folklore (a collector, a
  bargainer, a mimic of a parent's voice…).
- Each needs **learnable tells and counterplay**, so testimony is *worth*
  dying for.
- Roster, behaviors, and lore: **TBD** — likely the first big design
  session after this document.

---

## Structure & Session Questions (unresolved)

- ~~Do players enter the maze solo, in squads, or staggered?~~
  **RESOLVED:** Pressure-style — a persistent social **Refuge** lobby
  funnels small groups into **instanced maze runs** (Roblox reserved
  servers). Squad size TBD, but the witness system wants ≥2 souls per run
  to shine; solo remains valid (surviving an encounter is your own
  testimony). Likely sweet spot to playtest: 3–6.
- Maze generation: **procedural, handcrafted, or handcrafted pieces
  procedurally assembled**? Does the maze shift between (or during) runs?
- What happens to a snatched player? (Spectate, return to Refuge, become an
  echo?) Is there any permanence?
- Session length target for a full run?
- Audience/rating considerations: horror tone on Roblox, "children's souls"
  framing — keep dread atmospheric, not graphic.

---

## Why Roblox

- The Pressure/Doors-like audience lives on Roblox and discovers games
  through it; the genre's context is native to the platform.
- Multiplayer networking, servers, cross-platform, distribution, and
  payments are provided — the hardest parts of a standalone build.
- Roblox Studio suits a design-first creator: environments, lighting, and
  atmosphere can be built visually before any code exists.
- Trade-offs accepted: platform revenue share, platform dependency.
  Revisit standalone only if/when the game outgrows the platform.

---

## Next Steps

1. Design the **first entity** end-to-end (motive, tells, counterplay,
   what testimony reveals) as the template for the roster.
2. Decide the **witnessing rules** and knowledge scope (server vs global).
3. Sketch the **Refuge progression stages** (what changes, at what counts).
4. Open Roblox Studio and block out a tiny greybox maze — no code, just
   feel for scale and sightlines in a hedge corridor.
