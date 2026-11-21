# Style Guide Improvement Plan — THE ASHEN DOMINION

> Commissioned by the user 2026-11-21 in the dedicated side chat
> "執筆スタイルガイド改良". The user ruled: compile everything into a plan
> first, then proceed. **This file is the plan. No change to
> `04_style_guide.md` is authorised by this file alone** — each item below
> is executed only after the plan is approved, in the order given, and
> items marked [RULING] only after the user rules on the question listed.
>
> Target file: `04_style_guide.md` (path must not change — `prompts/02_write_chapter.md`
> gives it the highest priority for style, `prompts/05_critique_repetition.md`
> imports its banned patterns, `chapters/_template_beat_sheet.md` cites its
> rotation, and CONTEXT_PACK lists it as an every-time file).

## 1. Goals, non-goals, guardrails

### Goals
1. Make the guide **findable in seconds** while writing/editing: a writer
   mid-chapter should locate any rule without reading the whole file.
2. Make the guide **loadable every time** at its budgeted size: CONTEXT_PACK
   budgets ~500 tokens; the file is currently ~1,284 words (~1,670 tokens).
3. Make the guide **complete as an index of hard style rules**: every
   standing style ruling that lives only in a character card should be
   either in the guide or explicitly pointed to from it.
4. Make the guide **true to its title** ("Style and Anti-Repetition"):
   give anti-repetition a real method and a real checklist, not only a
   list of beats to rotate.
5. Remove **contradictions and false pointers** between the guide, the
   prompts, the beat-sheet template, the character cards, and canon.

### Non-goals
- No manuscript prose changes in this project. Findings that imply prose
  changes (e.g. a stock phrase in closed chapters) are reported, not applied.
- No new canon, no new character facts, no new plot rules. Anything that
  would be a story/style *decision* is flagged [RULING] and left undecided.
- No file splits and no path changes (prompts and chats reference the path).

### Guardrails
- **Never delete information.** Slimming means moving detail to a marked
  Reference layer in the same file, or to the file that already owns it
  (terminology_log, a character card), with a pointer left behind.
- Every rule in the guide keeps its **ruling date and source** (chapter
  review / user ruling). A rule whose provenance cannot be traced is
  flagged, not silently kept or dropped.
- **Coordination with two running projects (check before every edit):**
  - Context-load project (`reviews/context_load_project.md`), item **I-3**
    is the same work as SG-2 below. Whichever project executes it first
    must log it in the other project's file, so the nightly cron does not
    redo or overwrite it.
  - Nia AAVE revision pass (`reviews/nia_aave_revision_log.md`, nightly
    cron): SG-4 codifies the AAVE rule in the guide; it must match the
    pass's own rule wording exactly, and must not change the pass's scope.
- Verify after each item: word count before → after, cross-references
  updated, and a re-read of the full guide for internal contradiction.

## 2. Baseline measurement (2026-11-21, verified by direct read)

| Section | Words | Note |
|---|---:|---|
| Header / provenance | 21 | Migration note from the Claude.ai summary, Part D |
| Style | 463 | Of which **Units alone = 292** and Background specificity = 101; the other five bullets total ~70 |
| Figurative Language Policy | 85 | Ruled 2026-11-17, ch004 review |
| Character Voice Rules | 363 | Covers swearing, ♥ (general + typography), Nia ♥, Sonya, the monster |
| Recurring Beats | 106 | Four beat groups; **the Seasons ruling is filed inside this list** |
| Story Time | 99 | Ruled 2026-11-18, after the ch096 invented duration |
| Banned Patterns / Hard Rules | 159 | Mixes prose bans with reply-workflow rules (see F-6) |
| **Total** | **1,284** | ~2.5× the CONTEXT_PACK budget (~500 tokens) |

Reference points checked for this plan: `00_canon.md` (theme/promise),
`CONTEXT_PACK.md`, `prompts/01_beat_planning.md`, `02_write_chapter.md`,
`05_critique_repetition.md`, `chapters/_template_beat_sheet.md`,
`chapters/_template_feeding_ritual.md`, the Voice sections of the cards
for Bog, Nia, Sonya, Priya, Rin, Darkwing and the tentacle monster, and
`characters/priya_raghavan.md` ll. 250–259 (stutter rules).

## 3. Findings (evidence for the items in §4)

- **F-1 Structure disorder.** Seasons (a world/time rule) sits as a bullet
  inside "Recurring Beats (use, but rotate)". Story Time is a separate
  late section although it belongs with Seasons. There is no contents
  list, so a 1,284-word every-time file is searched linearly.
- **F-2 Units dominates and mixes rule with history.** The core rule is
  two lines (yard–pound general; Sonya metric in her own speech/thought).
  The remaining ~250 words are the 2026-11-21 conversion history, which
  already has a full home in `reviews/terminology_log.md` §7a–7g.
- **F-3 Voice rules are incomplete in the guide and complete only in cards.**
  Standing rulings absent from the guide:
  - Nia: **AAVE surfaces when her emotions run high**; baseline controlled,
    near-standard (canon, ruled 2026-11-20; AAVE pass underway 2026-11-21).
    The guide currently says nothing about her speech register at all.
  - Priya: **stutter register** — permanent in ordinary conversation;
    eases where she is intense/certain on spirits and medicine; **no
    stutter at all in professional/clinical lines, a touch stronger in
    personal lines** (ruled 2026-11-18, refined on the ch093 draft).
    Only in her card, ll. 258–259.
  - Bog: address terms — he never calls Nia "pickle" (her insult for him);
    his teasing name for her is "squeeze candy", pure mockery, no
    tenderness (author, 2026-11-20). Only in his card.
  - Rin ("It's clobberin' time!", Darkwing impressions, loud cartoonish
    energy), Darkwing (dry, laconic, leaves questions on the table) and
    the Mediatoress (a different register entirely, speaking through
    Priya) have **no guide entry at all**.
- **F-4 The rotation the beat sheet cites does not exist in the guide.**
  `_template_beat_sheet.md` requires "at least one item from the rotation
  in 04_style_guide.md", but the guide contains no rotation list. The
  actual list lives in `prompts/01_beat_planning.md`: *location, opening
  style, type of conflict, type of ending hook*. The pointer is false
  and the list itself is narrower than what recent beat sheets actually
  vary (POV, scale, tone, cast pairing, ending-hook type — see beat
  sheets ch091–ch099).
- **F-5 Anti-repetition has a consumer but no content.** Prompt 05 checks
  "repetition / lack of change / easiness / style-guide violations" and
  imports "the banned patterns" — which currently amount to one prose
  ban (paperwork). A preliminary mechanical scan of the 130 chapter
  files (4–5-word n-grams, this plan's preparation) shows the audit
  must **classify, not merely count**:
  - *Intentional motifs (protect, do not flag):* Nia's litanies
    ("tomato, Scotch bonnet, thyme" ×13; "Amara, Chidi, Daniel, hold
    the line" ×10), the count ("four hundred and twelve" ×21, frozen
    at 413 by ruling), the bells, ♥, the monster's logging.
  - *Candidates for review (unclassified):* simile frames "a man who
    had…" (×18) / "the way a man…" (×14), "in the middle of…" (×39
    across forms), "for the first time" (×14). Dialogue tags are
    dominated by "said" (657) over all alternatives combined (~136) —
    whether that plainness is the house style or a flattening is a
    judgement call, not a mechanical fact.
- **F-6 Banned Patterns mixes two kinds of rule.** Alongside the prose
  ban (paperwork) and a story rule (Florence-session: no invented
  extras) sit two **reply-workflow** rules ("No notes at the end of
  replies unless asked", "Refinement requests: output only the polished
  text"). Those bind Muse's chat behaviour, not the prose, and are
  invisible to Prompt 05, which imports this section as prose bans.
- **F-7 Later-established conventions are uncodified.**
  - Full-chapter **italic interior monologue** (Nia ch121, Sonya ch129):
    typography, ♥ and onomatopoeia inside thought, counting intrusions —
    established in practice, nowhere stated as a convention.
  - The **feeding ritual** has a full scene template
    (`chapters/_template_feeding_ritual.md`: run all steps, then vary)
    that the guide never mentions, although it is exactly a
    style/anti-repetition device.
  - Onomatopoeia spellings in ritual/erotic scenes (*chu♥, jupo♥,
    jururu, thwack-thwack, ding*) are consistent in practice, uncodified.
- **F-8 Desired texture is thin against the stated theme.** Canon's
  theme is "A deranged, erotic, slapstick sci-fi fantasy" with the
  promise "Entertaining you—without the political correctness!", but
  the guide's texture bullet (26 words) names only dark comedy,
  slapstick, Bog's obliviousness and Nia's dry fury. The monster's
  literalism, Rin's cartoon energy and the sincerity/horror contrasts
  are used in practice (and listed under Recurring Beats) but not
  stated as texture. Expanding this is a [RULING] — see D-2.
- **F-9 Duplication/drift risk.** Sonya's metric rule is stated in full
  three times (guide Units, guide Voice, her card). The monster's
  own-units rule is split between the guide (Units exception 2), his
  card (a long barium half-life history) and lore. Without a stated
  "guide = short rule + pointer, card/lore = full record" convention,
  future rulings will keep landing in one copy only (the paperwork
  tic reached the guide and Bog's card by exactly this route, 2026-11-19).

## 4. Improvement items (execute in this order)

### Phase 1 — Structure and load (no new rules, no rulings needed)

- **SG-1 Reorganise the guide.** New section order: (1) Pack Core,
  (2) Style basics, (3) Voice at a glance, (4) Typography & notation,
  (5) Time, seasons and units, (6) Recurring beats & rotation,
  (7) Anti-repetition checklist, (8) Banned patterns (prose),
  (9) Reference layer (full ruling texts, dated). Move Seasons out of
  Recurring Beats into (5), next to Story Time. Add a contents list
  with one-line summaries at the top. *Verify:* every pre-existing rule
  still present (diff against a saved copy), word count recorded.
- **SG-2 Pack Core (executes context-load item I-3).** A marked
  "Pack Core" block at the very top, ≤700 words, containing only what
  a writer needs mid-draft: POV/tense/scene length/texture, units core,
  background specificity in two lines, Holy Val, ♥ rule + typography,
  one line per major voice (SG-4), time rule, seasons line, paperwork
  ban, rotation shortlist. Log completion in
  `reviews/context_load_project.md` so the cron skips I-3.
  *Verify:* core alone is self-sufficient for a routine chapter;
  total file size recorded before → after.
- **SG-3 Slim Units.** Core rule ~40 words in Pack Core and in (5);
  the conversion history collapses to a three-line summary plus the
  pointer to `terminology_log.md` §7a–7g. Exceptions (1)–(5) stay,
  shortened. Sonya's exception cross-refers to SG-4 instead of
  restating her card. *Target:* Style section 463 → ~200 words.

### Phase 2 — Voice completeness (sources exist; depth is [RULING] D-3)

- **SG-4 Voice at a glance.** One entry per major voice, hard rules
  only, each ending with a pointer to the owning card:
  Bog (crude/easygoing/lewd deadpan; Holy Val; never "pickle" for Nia;
  "squeeze candy" = mockery), Nia (blunt/dry; **AAVE surfaces when
  emotions run high, baseline near-standard**; ♥ against her will;
  litany + count), Sonya (laconic; Cyrillic curses/thoughts; ♥ while
  cursing; metric in speech and thought; narration name = Sonya,
  Sofiya formal only, never Sophia/Sofia), Priya (**stutter register:
  ordinary = stutter, clinical/professional = none, personal =
  stronger; Mediatoress = separate register**), Rin (loud, giggly,
  "It's clobberin' time!", Darkwing impressions), Darkwing (dry,
  laconic, questions left on the table), the monster (flat literal
  formal; logging forms; own time units only). *Verify:* each line
  traceable to a card/canon source; no card text copied wholesale.
- **SG-5 State the duplication convention (F-9).** A two-line note at
  the head of the Voice and Units sections: the guide holds the short
  rule + pointer; the card/lore file holds the full record; a new
  ruling is written to both in the same pass.

### Phase 3 — Texture and conventions (drafts for [RULING])

- **SG-6 Texture draft [RULING D-2].** Prepare (not apply) a revised
  Desired-texture paragraph that accounts for canon's theme/promise
  and the comedy engines actually in use (Bog's obliviousness, Nia's
  dry fury, the monster's literalism, Rin's energy, sincerity/horror
  contrast), plus the erotic/slapstick balance as practised. Present
  as a draft in this plan's log for the user to amend/rule.
- **SG-7 Codify established conventions [RULING D-4].** Draft entries
  for: italic interior monologue (when used, ♥/onomatopoeia/counting
  inside it), the feeding-ritual template pointer ("run all steps,
  then vary"), and onomatopoeia consistency. Sources ch121, ch129,
  `_template_feeding_ritual.md`. Apply only what the user confirms
  is a standing convention rather than a one-chapter device.
- **SG-8 Background specificity, operationalised.** Keep the ruled
  principle; add a short worked-example set by setting (northern
  Alabama flora/fauna, Florence households, Appalachia, Val tech)
  drawn from chapters already written (e.g. ch122's red-tailed hawk,
  shagbark hickory), with the standing caution: correct for place and
  person, background not exposition. No new examples invented.

### Phase 4 — Anti-repetition (audit first, rules after)

- **SG-9 Full repetition audit (read-only).** Method: (a) mechanical
  4–5-gram scan of all 130 chapter files; (b) inventories of chapter
  openings and closings, simile frames, metaphor vehicles, emotional
  expressions, dialogue tags, scene transitions; (c) classification
  of every frequent item as *intentional motif* (F-5 list, extended),
  *house style* (keep), or *candidate stock phrase* (report with
  chapter/line evidence). Deliverable: a separate audit report in
  `reviews/`; **no prose changes and no new bans from this item alone**.
- **SG-10 Anti-repetition checklist.** From SG-9 plus Prompt 05's four
  angles, write the checklist section the title promises: what to
  vary (metaphor, emotional expression, transitions, openings,
  closings), what to protect (intentional motifs), and how the
  Prompt 05 check is run. New banned patterns enter only by [RULING D-5]
  on the SG-9 report.
- **SG-11 Repair the rotation (F-4).** Write the canonical rotation
  list into the guide: the four from Prompt 01 (location, opening
  style, conflict type, ending-hook type) extended with the axes
  recent beat sheets actually use (POV, scale, tone/register, cast
  pairing) — the extension is [RULING D-6]. Then fix
  `_template_beat_sheet.md`'s pointer and align `prompts/01` and
  `prompts/02` wording with the guide's list.
- **SG-12 Recurring Beats governance.** For each beat group: the beat,
  its variation requirement, and a pointer where a template exists
  (feeding ritual → its template; monster logging → his card).
  No frequency quotas invented; if the user wants quotas, [RULING].

### Phase 5 — Bans, separation, sync

- **SG-13 Separate prose bans from workflow rules (F-6) [RULING D-7].**
  Propose moving the two reply-workflow bullets to the workspace
  operating notes (AGENTS.md / prompts), leaving Banned Patterns as
  prose-only so Prompt 05 imports cleanly. The Florence-session
  "no invented extras" rule is a story rule — propose its placement
  (Banned, or canon pointer) in the same decision.
- **SG-14 Final sync and re-measurement.** Re-measure the whole file
  and the Pack Core; update CONTEXT_PACK's budget line if the real
  number has changed; record before → after in this plan's log and in
  `context_load_project.md` (I-3); check every inbound pointer
  (prompts 01/02/05, beat-sheet template, cards that cite the guide,
  translation drafts — archived, note only). Completion report to
  the user in this chat.

## 5. Decisions needed from the user (collected, not blocking Phase 1)

- **D-1** Approve the section order and layer design in SG-1/SG-2,
  including the ≤700-word Pack Core target.
- **D-2** Texture (SG-6): how far should Desired texture go beyond
  dark comedy/slapstick — should the erotic register and the
  "without political correctness" promise be stated as style
  instructions, and in what words?
- **D-3** Voice depth (SG-4): guide entries as one-line hard rules +
  pointers (recommended, anti-drift), or fuller voice summaries in
  the guide accepting duplication with the cards?
- **D-4** Conventions (SG-7): which of italic monologue, ritual
  template, onomatopoeia are standing conventions to codify?
- **D-5** After SG-9's audit report: which candidate stock phrases,
  if any, become banned patterns or watch items?
- **D-6** Rotation (SG-11): adopt the extended axis list, or keep
  Prompt 01's original four?
- **D-7** Workflow bullets (SG-13): move them out of the guide —
  and to where?

## 6. Risks

- **Over-codification:** a guide that prescribes too much produces
  the monotony it exists to prevent. Mitigation: hard rules stay
  short; everything else is a pointer or a checklist question.
- **Drift by duplication:** every rule copied into a second file is
  a future contradiction (F-9). Mitigation: SG-5's convention.
- **Collision with running crons:** AAVE pass touches Nia's lines
  nightly; context-load cron may reach I-3. Mitigation: the
  coordination guardrails in §1, checked before each edit.
- **False audit positives:** mechanical frequency flags intentional
  motifs (F-5). Mitigation: classification by a reader, counts are
  evidence only.

## 7. Acceptance criteria

- [ ] Pack Core exists, ≤700 words, and a routine chapter can be
      drafted from the core + cards without the reference layer.
- [ ] Every rule present before the project is still present
      (in core, body, or reference layer) with its date/source.
- [ ] Nia AAVE and Priya stutter register are in the guide (SG-4).
- [ ] The rotation cited by the beat-sheet template actually exists
      in the guide (SG-11).
- [ ] Seasons is no longer inside Recurring Beats (SG-1).
- [ ] Units history is a pointer, not 250 words of prose (SG-3).
- [ ] An anti-repetition checklist and an audit report exist (SG-9/10).
- [ ] CONTEXT_PACK and the context-load log match the final numbers (SG-14).

## 8. Progress log

- 2026-11-21: Baseline measured; findings F-1–F-9 verified against the
  guide, cards, canon, prompts and templates; preliminary n-gram scan
  run (results in F-5). Plan written (this file). No items started;
  `04_style_guide.md` unchanged.
- 2026-11-21: At the user's direction, this plan was handed over to the
  main chat's context-load reduction project as reference material for
  its item I-3 (pointer and summary recorded in
  `reviews/context_load_project.md`, under I-3 and in its Progress log,
  and a handover message sent to the main chat). Status here is
  unchanged: this plan itself remains unexecuted pending the user's
  rulings D-1–D-7.
