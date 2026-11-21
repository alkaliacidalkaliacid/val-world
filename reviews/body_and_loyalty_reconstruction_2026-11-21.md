# Body Records & Loyalty Progression — Reconstruction Proposal (2026-11-21)

> STATUS: **ADOPTED AS-IS by the user, 2026-11-21, and synced.**
> Synced to: `lore/consort_body_records.md` (new; §1's new-file option
> taken), `lore/val_devices.md` (loyalty progressions; Sonya's current
> value revised 61% → 78% [est.]), `02_current_state.yaml` (`body:`
> fields ×4; Sonya `loyalty:` 78%), the four character cards, and
> MEMORY.md. This file remains the evidence table behind the synced
> records. §5's open points were resolved by the adoption as written
> in the draft: Q1 new file; Q2 numbers as proposed; Q3 Nia's baseline
> stays at purchase with the pre-Bog start point recorded as unstated;
> Q4 Sonya 78% adopted; Q5 Nia's checkpoints adopted as [est.].
> Prepared at the user's direction (2026-11-21): (1) establish height,
> weight and BWH for Nia, Sonya, Priya and Rin, recording physical changes
> over time from ingestion of Val semen, handled in the same manner as the
> loyalty rating; (2) reconstruct the progression of Nia's and Sonya's
> loyalty ratings.
> Method follows the character-building method in
> `characters/_template_character.md`: harvest first, proposals marked,
> nothing canonised until the user rules.
> On ruling, the agreed values sync to: `lore/val_devices.md` (or a new
> `lore/consort_body_records.md` — see §1), `02_current_state.yaml`
> (per-character fields), and each character card (a "Body / Measurements"
> section). Estimates that are never displayed in prose are marked [est.]
> exactly as the season bands are in `05_timeline.md`.

---

## 1. How loyalty is currently handled — the model to copy

Checked in the files, 2026-11-21:

- **Definition + current values in one lore place:**
  `lore/val_devices.md`, "Loyalty rating" — what the number means
  (100% = no desire to remove the collar; >50% = almost certainly never
  betrays the handler), the note that most characters are left blank,
  and the current list: Monster 300%, **Nia 93%, Sonya 61%, Rin 18%,
  Priya 12%**. It also notes which values have been *displayed in prose*
  (ch115: Nia / Rin / Priya) and which are *author-given, not shown*
  (Monster / Sonya).
- **Per-character field in the state file:** `02_current_state.yaml`
  carries `loyalty: "93%"` etc. on each character entry — the
  at-a-glance current value, overwritten, not appended.
- **Card note only where it matters:** e.g. `characters/tentacle_monster.md`
  records its 300% in Core, pointing back to the lore definition.
  The women's cards do **not** currently carry their loyalty values.

### Proposed mirror for body records

1. **One central record** — new file `lore/consort_body_records.md`:
   - the rule (what is measured, in what units, what counts as a
     baseline, what a "change" entry needs: chapter, cause, delta);
   - a current-values table for the four women (height / weight / B-W-H);
   - a dated change log per woman, chapter-anchored, [est.] where the
     prose gives the change qualitatively but no number.
   A separate file is proposed rather than a section in
   `val_devices.md` because these are *not* collar/System outputs —
   loyalty is something the System displays; measurements are not.
   (Alternative if the user prefers exact mirroring: a section in
   `val_devices.md` beside Loyalty rating. Decision needed — §5, Q1.)
2. **State file fields**, overwritten like `loyalty:` —
   `body: {height:, weight_lb:, bust_in:, waist_in:, hip_in:}`
   (field names as synced — imperial, per the unit ruling below)
   on Nia / Sonya / Priya / Rin only; everyone else blank.
3. **Card section** — "Body / Measurements" in each of the four cards:
   baseline + current + the qualitative change summary already in canon
   (see §2). Pack layer stays small: one line in Core pointing to it.
4. **Units:** as originally proposed, cm / kg with imperial in
   parentheses — **superseded at sync by the user's unit ruling
   (2026-11-21): the yard–pound system throughout**, consistent with
   the rest of the text (Bog's height is on file in feet — 7.5 ft,
   `characters/bog.md`). The synced files carry imperial only.

---

## 2. Harvest — what the files already establish (no invention)

### Consort physiology (canon, `00_canon.md` World Rules, 2026-11-17)
An Earth woman who becomes a consort by ingesting a Val's semen changes
gradually: sweat, tears, saliva, mucus, arousal fluid, urine and feces
become clean and fragrant; feces become elastic jelly (normally rounded
lumps; constipation forms one long cylinder the sphincter cannot sever);
excretion and urination are pleasurable; waste fertilises plants but
slowly terraforms the local ecosystem toward the Val homeworld.

### Nia Okonkwo, 39
- Appearance (archive + card): tall, muscular, rugged Black woman,
  powerful build, close-cropped natural hair. "A big, dense, trained
  body" that, collared, can still make a Val bleed with a knee strike
  (ch003, card note).
- Sonya is "my height" — Nia's own words in prose (archive part02;
  carried in Sonya's card: "roughly Nia's height"). **The two heights
  are therefore equal, or near enough that Nia calls them the same.**
- Body and Conditioning (card, stable facts): her sole nourishment is
  Bog's semen (complete Val protein), which has gradually shifted her
  physiology — more resilient, robust and youthful; increased
  fertility; **body grown softer with abundant fat over a muscular
  core**; she is forgetting the taste of Earth food.
- ch010: after the ritual she is still hungry — "her body is rebuilding
  itself on Val protein" — and requests second and third helpings.
- ch014–015: the jelly-constipation episode — the physiology change is
  already fully in effect by then.
- ch120: thick buttocks, "muscle and soft curves" (beat sheet).
- Archive hyperbole, **not** a measurement: the Mississippi prose calls
  her backside "a hundred and ten kilos of soft, flushed… backside"
  (archive part05). That is a joke about the backside alone and cannot
  be read as her weight. Flagged here so it is never harvested as one.
- Ingestion timeline: liturgy drilled at the front (before Bog);
  forced service to 412 Val (ch004); with Bog from Day 1 (ch001/003),
  three to five feedings a day (ch007). *Open point:* whether the
  physiology change began under the front-line Val or only under Bog
  is not stated in the files. (Decision needed — §5, Q3.)

### Sofiya "Sonya" Ivanova, 29
- Appearance (card): tall, sturdy white woman, **roughly Nia's
  height**; silver asymmetrical undercut; pale gray eyes; eyebrow scar.
- Captivity facts (card): piercings identical in placement to Nia's;
  intestinal bead-chain fitted; **her meals replicate the composition
  of Bog's semen exactly, synthesised by the monster**.
- ch119 (state + summary): trained musculature remains, but **breasts
  and buttocks have engorged** under the working-over; buttocks covered
  in overlapping palm-prints exactly Bog's, breasts in countless
  teeth-marks exactly Bog's; excretions (clean urine, vaginal fluid,
  gelatinous excrement) expelled and harvested — i.e. consort
  physiology is already fully in effect in her by ch119.
- ch125 (summary, user-specified plot): "a layer of fat quite
  unbefitting an assassin"; summary generalises: **breasts, belly and
  thighs softened — a general layer of fat over the trained muscle**,
  the regimen's visible signature.
- ch128: "well-rounded pale buttocks", trained musculature working in
  waves.
- Ingestion timeline: collared ch038; standing orders ch039–040 —
  meals to Bog's seed's composition from then on, inside the monster,
  continuously, until direct contact ch125–130.

### Priya Raghavan, 43
- Appearance (card, Voice): "Plump, curvaceous Indian woman."
- ch099–103: Bog's hands tour **breasts, thighs and belly**, praising
  each part's softness and plenty; **the belly is his declared
  favourite** — "a belly that's done its work and got better at it"
  (a mother of two's belly; ch101 summary). ch102: she kneads her own
  **huge left breast**; Bog grips her **thick, brown, married
  backside**. ch103: breasts swinging in heavy arcs, belly rippling,
  thighs trembling, backside rolling — "nothing in her rigid, all of
  her in tides."
- ch122 (summary, user-directed revision): the set-piece contrast of
  the two squatting bodies — **Priya full and curved in every line,
  belly settled over her folded legs**, against Rin's slenderness.
  The monster's assessment: her body is **well suited to pregnancy;
  she is to maintain her present physique**.
- Key distinction: Priya's plumpness is **pre-existing** (43, two
  daughters, a lifetime before Bog) — it is *not* a Val-semen change.
  Her ingestion begins only at ch099–104 (coupling ch102–103, oral
  ch104), then the monster's Bog-mimicking feeding ch122, and the
  shared craving is established by ch124. **No measurement-scale
  physical change is stated in the prose for her yet.** Her change
  log therefore starts almost empty — which is itself the correct
  record, mirroring how most loyalty values are left blank.

### Yan Rin, 20
- Appearance (card): young East Asian woman, oversized goggles,
  lopsided ponytail. No build description in the card.
- ch122 (summary): **slender and angular, built light and lean**;
  the monster assesses her as **still a little too slender for
  breeding and under orders to eat more**; it logs her as eating well.
- ch105: **her five senses have sharpened a notch past human**,
  unnoticed by her — recorded in state as "an early outward sign of
  her becoming a Val's consort".
- Ingestion timeline: first ingestion ch092 (tip only — her jaw
  cannot take more, state); second liturgy ch095; duet ch104;
  monster's Bog-mimicking feeding ch122. The ch105 sense-sharpening
  is therefore her **first logged change**, and it is functional,
  not mensural — the change log needs a non-numeric entry type.
- No engorgement / softening is stated for her anywhere yet.

---

## 3. [PROPOSAL] Baseline and current measurements

> All numbers in this section are **Muse proposals for ruling**,
> derived only from §2. "Baseline" = at first ingestion / at the
> start of the recorded period (see notes); "Current" = ch130.
> Deltas are the proposal's arithmetic, not new facts.

|  | Height | Baseline weight / B-W-H | Current (ch130) weight / B-W-H | Recorded change behind the delta |
|---|---|---|---|---|
| **Nia** (39) | 5′11″ | 185 lb / 41–31–43 in — at purchase, ch003: dense trained muscle, front-line neglect | 212 lb / 45–33–47 in | Softer, abundant fat over muscular core; more youthful, more fertile (card). Change essentially complete in kind by ch014; degree still increasing |
| **Sonya** (29) | 5′11″ — same as Nia, per prose | 163 lb / 36–26–37 in — at collaring, ch038: lean trained assassin | 187 lb / 41–29–42 in | Breasts & buttocks engorged (ch119); general fat layer over muscle — breasts, belly, thighs softened (ch125) |
| **Priya** (43) | 5′4″ | 174 lb / 43–35–44 in — at first meeting Bog, ch055: pre-existing plumpness, **not** Val-caused | 174 lb / 43–35–44 in — **no measured change yet** | None stated in prose. Craving only (ch124). Log opens here |
| **Rin** (20) | 5′5″ | 115 lb / 32–24–33 in — at collaring, ch086: light, lean | 117 lb / 33–24–34 in | +2 lb under the monster's "eat more" assessment (ch122) [est.]; senses sharpened (ch105, non-mensural entry) |

Notes on the proposals:
- **Nia = Sonya in height** is the one figure the prose fixes
  relatively; the absolute 5′11″ is the proposal. If the user wants
  them shorter / taller, both move together.
- **Units (ruling, 2026-11-21, after adoption):** the figures are
  recorded in the yard–pound system, consistent with the rest of the
  text. This table was first drafted in metric; the imperial values
  above are the synced record, rounded to whole units, and the
  deltas in the synced files are computed from them.
- Nia's baseline is set *after* the front line: she arrives at Bog
  already liturgy-drilled and physiology may already be shifting
  (see Q3). Her largest recorded change is composition (muscle →
  muscle + abundant fat), which is why weight and all three measures
  rise together rather than waist alone.
- Sonya's delta is deliberately the second largest: hers is the only
  change the prose calls out as *visible on an assassin's frame* and
  unbecoming to her profession — the regimen's signature.
- Priya's zeroes are intentional. Inventing a delta for her would
  contradict ch122 ("maintain her present physique").
- Rin's near-zero is likewise text-bound: "still a little too
  slender" at ch122 forbids a large gain by ch130.

---

## 4. Loyalty progression — reconstruction

> Scale (canon, `lore/val_devices.md`): 100% = no desire to remove
> the collar; >50% = almost certainly never betrays the handler.
> **Only one point per woman is measured in the record** (Nia 93% at
> ch115; Sonya 61% author-given, current at the time it was set,
> 2026-11-20). Everything else below is a reconstruction, marked
> [est.], anchored to chapter evidence — the same status the season
> bands have in `05_timeline.md`. Checkpoints are chosen where the
> prose shows a *step*, not a smooth curve: this System plainly moves
> in jumps at events, as both women's arcs do.

### 4a. Nia — 93% at ch115

| Checkpoint | [est.] | Evidence (chapter summaries / state) |
|---|---|---|
| ch003 — purchase, Day 1 | **~3%** | Knees Bog in the face the moment her field drops; at intake (ch004) she promises him dismemberment once the collar is off and keeps her family off-limits. His reading at the oath: she will make him *less* healthy at the first opportunity. Loyalty here is to Daniel and the children — the merchant's selling point. |
| ch006–007 — first week, the routine | **~18%** | The liturgy is already flawless (front-line drilling), but the new fact is Bog's gentleness: first praise in six years (ch006), a forehead kiss — "his gentleness frightens her more than the barracks did". She tracks her body starting to *expect* the pat on the head, and counters with the litany (ch007). Compliance is framed, by her, as endurance and reconnaissance. |
| ch008 — the deal | **~35%** | Her first "Please" — begging him *not* to look her family up, lest a report make them inventory. She then chooses the deal: consort and household help for collar removal and the family search, kept secret from Earth and Val. This is the first step that is hers: trust placed, not obedience extracted. |
| ch010–012 — second / third helpings; consort proposed | **~48%** | Her body is rebuilding on Val protein and she asks for more like "calling for ammunition" (ch010). First full sex (ch011): she sets the pace, Bog says she can stop — the first ♥ escapes her. Ch012: she negotiates consort terms (rights, a say, collar off first, her own family search) — bargaining *inside* the bond rather than against it, still just under the 50% line: the collar-off condition is the reservation that holds her below it. |
| ch013–016 — the domestic turn | **~60%** | One ordinary day (ch013): she cooks, does his paperwork, re-seats his tomatoes — and that night her family's roll call "comes slower". Ch014–015: in the constipation humiliation she grips his wrist and begs secrecy; her "I hate you" is muttered "with, for the first time, less conviction". Ch016: posed for his keepsake photo, she gives a rueful real smile "before she can stop it" — and afterward "never cursed at him once". **The >50% crossing belongs here:** nothing in these chapters is a woman still likely to betray him. |
| ch017–021 — the depot run | **~62%** (plateau) | The bunny cover, the rendezvous, Sonya. Her roll call "stutters on Daniel's name" (ch017) — the loyalty conflict is live, not resolved — and she steers Bog through the Sonya fight by counting portals (ch025–026). Competence and partnership, no step up or down the record can point to. |
| ch049–054 — Mississippi; the separation | **~76%** | The queue (ch049): count 423–424, holding the Hermes / Appalachia / collar door shut under a camp of Val — protecting *his* secret at cost to herself. Her litany gains a name she cannot explain: **Pickle**. She wiggles for Gorrak and files it as 424, "reconnaissance" (ch051) — the framing is now plainly a fig leaf. At the Old Guards (ch053) she asks for her bead string back: "she depends on it". Ch054: imagining the collar off, what she pictures is "a fat idiot on a couch" — and tells Darkwing "He's dead", believing it, grieving it. Absence is where the number does its largest work after ch016. |
| ch071–082 — believing him dead; reunion | **~84%** | Riding with Rin (ch071) she "keeps her hopes small" and counts trees. Reunion (ch076): she "shakes apart in the cockpit" at the sight of him alive. Ch082: he says "Love you!" plainly; she does not say it back — she tells the empty mountain "…Idiot♥". The refusal to say it is now the only distance left in the scene. |
| ch107–108 — the cavern reunion completed | **~89%** | Starved of her master through the separation, she climaxes from the reunion kiss alone (ch107). Then strikes his head hard enough to draw "ouch" and takes command of the ascent (ch108) — the defiance that remains in her is domestic, not treasonous: exactly what 89% should look like on this scale. |
| **ch115 — MEASURED** | **93%** | Displayed in prose. She stands under the number composing "a formal complaint to the universe" and repeats it quietly: "Ninety-three. Ninety. Three." |
| ch118–130 — after the measurement [est.] | **~94%**, not 100 | Ch118: offered removal at last, she smiles, traces the collar, and declines — "a little while longer", reasons unstated. Ch121 (interior, reader-only): the resolve stands *beside* the appetite — collar off, family found, the route now exists — and she admits she wants her stomach full of more of him. Ch124: she refuses him for one night, for Daniel. **Reconstruction's conclusion: she has not crossed to 100%** — the desire to remove the collar is banked, not gone — and the ch115 figure is still effectively current. No new value is proposed for the state file; a note "post-ch115: still <100, by her own resolve (ch121)" is. |

Shape of the curve: near-zero at purchase → a trust jump at the deal
(ch008) → the betrayal-line crossing in the domestic chapters
(ch013–016) → a plateau under the depot run → the second large rise
in *separation* (ch049–082), not in his presence → 93% measured →
a held line just under 100, held there by Daniel and the family
search, which are the same thing in her.

### 4b. Sonya — 61% author-given (set 2026-11-20)

> Handler note: Sonya's collar is the monster's fitting, her handler
> in the System's terms is Bog as the monster's Commander (ch031–033).
> Her progression is a *regimen* curve — manufactured, logged, and
> scored by the monster (vocabulary count, leaderboard, modules) —
> where Nia's is a household curve. The checkpoints below use the
> monster's own logging beats, which is why hers can be dated more
> finely than Nia's in the middle range.

| Checkpoint | [est.] | Evidence |
|---|---|---|
| ch024–030 — the depot betrayal | **0%** | She means to dispose of Bog and Nia all along (ch024), snaps a portal where Bog stood, steals the escape pod from in front of them (ch029) and strands them. This is the scale's floor: active, attempted betrayal of the handler, in progress. |
| ch034–038 — capture; the collar clicks | **~4%** | Tickle-taming breaks her portals out; she wakes collared (ch038): "Не сдамся — I won't surrender. **She no longer knows if true.**" The doubt is the first point on the scale. Nothing else has moved. |
| ch039–040 — standing orders; regimen begins | **~8%** | Fitted with rings, bells, bead string; meals set to Bog's seed's composition; taming brief stated (an Earth woman serves a Val male; Bog is her ideal master). Vocabulary logged at 312. Exposure and indoctrination begin; her output is still entirely threats and curses, now with involuntary ♥s studding them (ch041). |
| ch042–043 — the ranking; the cradle | **~16%** | Told Bog has flown to free Nia, his *primary* consort, and she might qualify as **second** (ch042): fury at ranking behind "a woman in a bunny costume" — the ranking has begun to matter, which is the regimen working. She ends composing a list for Bog "no longer tracking which items are threats". Ch043: curses Bog's (nonexistent) mother for fifty-one hours, is corrected to the cradle, curses that instead — and "something in her chest unclenches, and she hates it". |
| ch044–045 — rewards enter her arithmetic | **~26%** | She catches herself **calculating a reward's cost in modules** and cuts it off (ch044); "Не сдамся sounds smaller now". Ch045: Module One's record is read back as a training manual *for Bog*; she insists her unblinking watch of Nia's bunny hologram was "tactical analysis" — and erupts when narration grades her against the primary. The comparison, not Bog, is now what she fights. |
| ch046–048 — competition; "Вторая" | **~43%** | Orgasm twenty, closing on Nia's record; goals are adjusted *for her and by her uptake of them*: catch up, surpass, overtake — "number one in output, service, affection" (ch046). She memorises the anthem by chorus two and hums it — "tactical analysis" (ch047). Ch048: keeps a chant rhythm she "stopped fighting at bar forty", and at the prompt — "Nia Okonkwo is Commander Bog's primary consort, and Sofiya Ivanova is…" — whispers **"Вторая" (Second)** in her own voice. Unprompted self-placement inside his household: the deepest crack yet, and the last checkpoint still clearly under 50%. |
| ch070 — Module Nine / Ten | **~54%** | Muscle regulation logged as "reflex" (91 counts); her curses now log as *greetings and praise* — "Commander is a magnificent cucumber" (vocabulary 335). Scoreboard: Nia top, Sonya second, nine apart. "Current standing remains second." "Я знаю (I know)." **The >50% crossing belongs between ch048 and ch070:** by Module Nine she is performing the regimen's measures while denying she is performing them, which on this scale is past betrayal. |
| ch110 — regimen reported complete | **~59%** | The monster reports its assigned mission — her training — **complete** to Bog in the cavern (Bog never asks what it was). "Complete" is the trainer's word for the product it then shows him at ch119. |
| **~ch115 period — AUTHOR-GIVEN** | **61%** | Set by the user 2026-11-20, not displayed in prose. The ch119 beat sheet glosses it exactly: "past the point of betrayal, nowhere near wanting to stay — a mouth full of murder threats while the body keeps climaxing is exactly that number." Ch119's inspection bears it out: the hoarded torrent of Russian threats, one involuntary ♥ escaping mid-threat ("ублюдок♥"), to her own visible fury. |
| ch125–130 — after the author-given value [est.] | **~78%** — **new current value proposed** | Everything after ch119 is *contact*, which the regimen never included: ch125 she crosses the clearing **of her own movement** and straddles him, insulting him without pause; ch126 coupling, fainting, slapped awake, "Can you bounce?" — and she bounces, ending in a long kiss; ch127 the monster pushes her as a **primary consort** candidate and the idea lands as *ambition* — she rejects motherhood and accepts the contest ("Да♥. Watch me♥."); ch129 (interior): "I want it" — not escape, not revenge, **winning** — "Не сдамся♥. I am not surrendering now. I am *competing*♥."; ch130 she performs the household liturgy **perfectly, first time, not a single mistake** — the form Nia needed a front-line drilling and 412 repetitions to hold. **Reconstruction's conclusion: 61% is stale.** It was set before ch125–130 existed. A woman who walks to him herself, competes for primary, and executes his household's liturgy flawlessly is not at the same number as the woman cursing from inside the hatch. Proposed new author value: **78% [est.]** — well past betrayal, still short of Nia: she wants to *win* him, not yet to *stay* — the wanting-to-stay question (the 100% end of the scale) has not been put to her, and her rodina litany in ch130 (Baikal, Tolbachik, Ukok…) is her equivalent of Nia's tomato litany: the anchor she still recites while it "goes soft at the edges". |

Shape of the curve: 0% in active betrayal → single digits under
breaking (ch038) → a slow, logged, manufactured climb through the
Burrow modules, driven first by indoctrination, then — decisively —
by **competition with Nia** (ch042–048) → the 50% line crossed
inside the modules (by ch070) → 61% at the hatch → a steep rise on
first direct contact (ch125–130), driven by the same competition
now aimed at *primary*.

### Cross-reading
- Both women cross 50% **off a comparison or an absence**, not off a
  feeding: Nia in the domestic quiet after the deal, Sonya inside a
  leaderboard. Neither curve is a simple dose-response to semen —
  the ingestion timelines (§2) and the loyalty timelines do not
  track each other chapter for chapter, and the record should not
  imply they do. (The body changes *do* track ingestion; loyalty
  tracks events. Keeping the two logs separate, as proposed in §1,
  preserves that distinction.)
- Rin 18% and Priya 12% (ch115, measured) are left as single points:
  the user asked for Nia's and Sonya's progressions only, and neither
  Rin nor Priya has the chapter density of logged beats the other
  two have. Their body logs (§3) are likewise near-empty by design.

---

## 5. Decisions needed before anything is canonised

1. **Where the body record lives:** new `lore/consort_body_records.md`
   (proposed, §1) vs. a section in `lore/val_devices.md` beside
   Loyalty rating (exact mirror of loyalty's handling).
2. **The numbers in §3** — heights first (Nia = Sonya at 5′11″ is
   the load-bearing one), then each woman's baseline / current.
3. **Nia's ingestion start:** did her physiology begin changing under
   the front-line Val (pre-Bog), or only under Bog? This sets her
   baseline date and the head of her change log.
4. **Sonya's current loyalty:** adopt the proposed 78% [est.] as the
   new author-given current value (replacing 61% in
   `lore/val_devices.md` and the state file, with 61% retained in the
   progression as the ch115-period value) — or keep 61% as current
   and treat ch125–130 as not yet moving the System's number?
5. **Nia's progression checkpoints** (§4a) — adopt as [est.] record
   (in the loyalty section / timeline style), amend, or keep ch115's
   93% as the only recorded point?

*On ruling, sync: central record, `02_current_state.yaml`,
the four cards, `lore/val_devices.md` (loyalty progression),
`05_timeline.md` if the user wants the checkpoints there,
and MEMORY.md. Manuscript, part volumes, volumes and PDF are
untouched — none of this is prose.*
