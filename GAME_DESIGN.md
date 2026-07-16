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

- **Who is the greeter?** A former lost soul? Something neutral to the
  limbo? Or — dark option — one of the snatchers wearing a kind face?
  A community-knowledge game can dangle this mystery for a very long time.
- **Personal candle vs. communal 5,000:** if your candle opens your gate,
  what are the candles decorating the Refuge? *(Suggestion — Claude)*:
  when a soul escapes, **their candle stays behind, burning in the
  Refuge** — every flame in the lobby is a child who got free. The
  communal counter becomes a memorial of successes rather than a donation
  meter. To accept, replace, or rework.

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
- *(Suggestion — Claude)* **Echoes:** a snatched soul leaves a faint echo at
  the site of their death — a diegetic warning that later runners can find,
  carrying a sliver of information home on the victim's behalf. Fits the
  folklore tone (will-o'-wisps, ghost lights).
- Records could reveal progressively: silhouette → name → behavior →
  weaknesses, over multiple delivered testimonies.

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
- Since each candle is personal ("your candle, your gate" — see Canon
  Frame), can you carry an ally's candle home for them, or must every soul
  carry their own? (Big cooperative-design fork.)

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

- Do players enter the maze **solo, in squads, or staggered** into a shared
  maze instance?
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
