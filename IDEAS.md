# Ideas Parking Lot

Scope insurance. When a new idea shows up mid-design (it will), it lands
here instead of mutating the core game. Nothing here is rejected — it's
*deferred*. Review occasionally; promote an idea only if it survives the
test in `GAME_DESIGN.md` → "What Is Locked".

Format: one bullet per idea, date it, no elaboration required.

---

- **2026-07-16 — Two flames / candle colors.** Souls *start* with their
  candle, burning **blue** (spirit flame — dim light source, is the soul
  itself). The maze center holds **living fire**; kindling your candle
  there turns the flame warm/normal — "connecting back to life" — and
  that's what you carry home. Reframes the objective as retrieving a
  *flame*, not an object; loop and locked canon survive intact.
- ~~**2026-07-16 — Shrouding (stealth).**~~ **SUPERSEDED** same day by
  the light-source design below: pocketing your own candle replaces
  shrouding as the stealth trade. Still true: "snuffed" stays reserved
  for death; flame color reads as state at distance; the Wick question
  (which color does the false flame burn?) stands.
- **2026-07-16 — Light sources (refines the two-flame idea).** Your own
  candle is the **last-resort blue flame**: it can never be extinguished,
  and can be **pocketed freely** — going dark to hide is always available
  and costs you your light, nothing else. The *main* light comes from
  **discarded shorter candles of other souls** found around the maze,
  carried torch-like. They burn brighter but: lighting one **releases its
  owner's wail** — the last gasp of the human it belonged to — so taking
  better light announces you (and makes you listen to them). These *can*
  be extinguished, by you or perhaps by the maze. Their wax color (see
  sin lore in `GAME_DESIGN.md`) may matter: what does carrying a black
  candle attract?
- ~~**2026-07-16 — Open question from the above:** can you light a fallen
  *teammate's* snuffed candle as a torch?~~ **RESOLVED** same day, see
  `GAME_DESIGN.md` → Rekindling: a child's candle can never be a torch —
  lighting it returns the blue flame and **brings them back**. Only the
  discarded candles of older souls burn (and wail) as torchlight.
- ~~**2026-07-16 — Origin lore: the grieving father / the son as
  greeter.**~~ **PROMOTED** same day to `GAME_DESIGN.md` → "The Rip and
  the Greeter": limbo and snatchers are the ancient natural order; the
  professor's gate is the only new thing, built to retrieve his son and
  closing once it succeeds; the son voluntarily stays so the way out
  remains open for everyone else, earnestly helping as best a child can
  — flawed because he's a child, not because it's a game to him.
- **2026-07-16 — Universal tell (layered telegraph, anti-flicker).**
  Replace the genre's light-flicker with a far→near diegetic gradient:
  1. **the garden goes quiet** (birdsong/insects stop — far warning;
  silence is the oldest dread signal and nearly unused in the genre);
  2. **crows scatter** (mid warning + direction — lore twist: carrion
  birds don't fear the dead, so players never disturb them; only
  snatchers do, which is why the tell is trustworthy);
  3. **your flame flinches** (near warning + direction — the blue
  soul-flame gutters, burns low, *leans away* from what approaches; your
  soul is afraid before you are);
  4. entity-specific tell (shears, axle…) for identification.
  Interlock: pocketing your candle to hide also pockets your danger
  sense — stealth costs early warning, no tutorial text needed.
  **Unreliability rule (decided within the idea):** every layer is a
  little noisy, so watching them too hard psychs you out —
  the flame gently flickers on its own with movement and idling (a
  *flinch* must be read against its normal restlessness); lone caws and
  small crow disturbances happen routinely, distinct from a full wave
  only in degree; silence sometimes falls for no reason at all.
  Confidence comes from **stacking**: one layer is a maybe, two is a
  warning, three is certainty — and veterans are the ones who've
  internalized each layer's baseline noise. Paranoia is the intended
  experience; tune noise rates so false reads stay spooky, not annoying.
- **2026-07-16 — Composure (health system).** A legible **100→0 HP
  skeleton**, fictionally **composure** — souls have no flesh; damage is
  fear. **Minor entities** jumpscare-chip composure (FNAF-3-phantom
  setup role) and position you badly for the majors — **but they can
  kill you too**; nothing in the maze is harmless. **Major snatchers
  detect you more easily the lower you are** — and the tiers make that
  literal, because composure is *audible*:
  - **100** — full composure
  - **80** — a few scared noises, occasionally
  - **60** — audibly scared
  - **40** — sniffling and whimpering
  - **20** — audibly tearing up, crying
  - **0** — wailing / lost
  Your state is broadcast: teammates read you by ear (no UI), and things
  in the maze *hear you cry*. **Recovery rule: on its own, composure
  climbs only one tier above where you fell — never more.** Deep terror
  doesn't fade by waiting; climbing further needs an active source
  (open — candidates: warmth, rest spots, regen near other souls'
  flames; the community pillar as survival mechanic). Solo souls fray;
  groups restore each other. Diegetic meter: **the flame is the bar** —
  steady when composed, erratic when terrified, which degrades your own
  telegraph reading (can't tell the flame's danger-flinch from your
  terror-flicker).
- **2026-07-16 — Manual breathing (composure recovery).** The limbo
  forces manual breathing — souls don't *need* breath; breathing is a
  remembered self-soothing ritual from being alive. To recover composure
  past the one-tier passive cap, you **match a breathing rhythm**: at low
  tiers the pattern starts as **hyperventilation** — fast, shallow, hard
  to match — and success means progressively *slowing* it down.
  Difficulty scales with terror automatically. It's a deliberate act:
  you stop, you're occupied, you're vulnerable — and it's **audible**
  (gasps and shaky breath broadcast like crying), so finding a safe
  place to breathe is a real decision. **Group version:** matching a
  composed teammate's steady rhythm is easier than finding your own —
  borrowing someone's calm (absorbs the "regen near other souls'
  flames" candidate). Mobile-friendly (tap/hold rhythm). Caution:
  reserve the minigame for climbing *tiers*; passive recovery handles
  small chips, or it wears out fast.
- **2026-07-16 — Entity visual direction: colored silhouettes, smoke,
  freeze-frames, the dark comes with them.** Snatchers are otherworldly —
  not exactly human, not exactly creature: **vague shapes shrouded in
  dark mist**, read mostly as **silhouettes of different colors**, moving
  like **freeze-frames snipped together** (here, then *here* — no travel
  between; stop-motion stutter, uncanny and technically *cheaper* than
  smooth pursuit). Death = Pressure-style mist-shrouded jumpscare with a
  brief scary image. **When one enters, the area darkens hard** — the
  darkness isn't ambience, it's the encounter starting; the room you just
  crossed becomes a memory test (attentive players pre-memorize exits).
  Interlocks with existing parked systems: signature color per entity =
  telegraph layer 4 (identification) for free, and "which color is which
  snatcher" is natural testimony knowledge; when the dark falls, keep
  your flame out (see a little, be seen) vs pocket it (blind, hidden,
  navigate on recall) — original panic decision from pieces already
  designed. *(Suggestion — Claude)*: unifying image — souls are **flame
  and wax**, snatchers are **smoke**; the mist shrouding them isn't
  weather, it's *them*. Flame vs smoke as the game's two-word visual
  thesis. Production note: silhouette + mist + darkness is the genre's
  great equalizer on Roblox — scarier *and* cheaper than detailed
  monsters.
- **2026-07-16 — Entity look refined: scribble figures (extends the
  visual-direction entry above).** Snatchers read as **scary scribbles
  vaguely resembling men and women** — humanoid, but drawn: jittery
  sketch-lines in **odd faint neon colors**, blurred like smears at the
  edge of your vision. Reference: Deadlock's Hidden King (shadow-mass
  body, few glowing features — eyes, claw-hands) but scribblier, fainter,
  more wrong. Animation is **"boiling lines"** (linework redraws itself
  each frame, *Take On Me*-style) — with the freeze-frame movement the
  whole concept is one sentence: *a drawing that keeps redrawing itself,
  somewhere closer each time.* **Thematic jackpot:** a world of
  children's souls where monsters look like **a child's scribble of a
  monster** — the limbo renders fear the way children draw it; justifies
  the art style in-fiction. Natural extension: testimony pages in the
  Refuge *are* scribbled children's drawings — the record and the monster
  are the same picture. Optional future mechanic (post-slice): clearest
  in peripheral vision, dissolving under direct gaze. **Roblox
  feasibility:** flipbook of 3–6 hand-drawn scribble frames on glowing
  flat layers + bloom + fog; no true painterly blur natively, but layered
  offsets approximate it; cheap to run, and the frames can be drawn by a
  non-artist (badly drawn = more on-theme).
- **2026-07-16 — Soul/NPC look: ghost-children, uncanny cute (completes
  the visual language).** Players and child NPCs are **literal ghostlike
  creatures**: soft, rounded **dark silhouettes with gently glowing
  eyes** — mix of A Hat in Time's simplified Snatcher-style skin
  (silhouette body, glow eyes, accessories readable as darker shapes)
  and the twins from The Cave (pale, wide-eyed, slightly *off*). Overall
  vibe target: **uncanny cute**, à la Little Nightmares. This completes
  a three-part contrast: children = soft cute silhouettes; snatchers =
  jagged neon scribbles (never confusable at any distance/lighting);
  world = elegant indifferent garden. Cute amplifies dread
  (vulnerability scaling). Steal Little Nightmares' other trick:
  **oversize the world** — hedges too tall, benches to climb, fountain
  like a lake; the garden was never built for children. Roblox notes:
  silhouette + neon eyes trivial to build; player accessories survive as
  darker shapes = avatar identity + future cosmetics channel (hats, eye
  colors); glowing eyes keep teammates visible in darkness for free.
  *(Suggestion — Claude)*: eyes/face carry composure visually — dimming,
  flickering, welling into glowing tears as tiers drop; silent twin of
  the audio crying (also chips at the deaf/muted accessibility gap).
- **2026-07-16 — Refuge NPCs (much later).** Other child souls as NPCs in
  the hub — faces, small stories, maybe testimony sources. Possibly a
  single **adult** soul: someone whose candle has too little wax for the
  gate to ever take them, who stays in the Refuge anyway. Post-slice,
  post-launch material.
