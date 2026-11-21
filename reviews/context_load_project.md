# Context-Load Reduction Project — Plan and Log

Commissioned by the user 2026-11-21: investigate which MD files burden the context window during writing/editing, design the investigation and the improvements first, then implement autonomously in spare time as a continuing project. This file is the plan and the progress log.

## Baseline measurement (2026-11-21, word counts; ~1 word ≈ 1.3 tokens)

| File | Words | Pack budget (CONTEXT_PACK.md) | Verdict |
|---|---|---|---|
| 02_current_state.yaml | 8,107 | ~400 tokens | **Critical** — "every time" file, ~25× over budget. Only 147 lines: per-character entries carry long prose notes. |
| 05_timeline.md | 7,432 | ~150 tokens (position + last 10 rows) | File size OK as archive; extraction is manual — needs a self-contained position block. |
| 03_open_threads.md | 2,712 | ~300 tokens (Open only) | Open section must be measured separately; Resolved Archive is already one-line. |
| 00_canon.md | 2,320 | excerpts only | Growing by accretion of World Rules; needs excerpt markers/index. |
| 01_synopsis.md | 540 | synopsis proper capped 200–250 words | Over its own cap — measure sections separately. |
| 04_style_guide.md | 1,284 | ~500 tokens | ~2.5× over; rulings accumulate in the always-load file. |
| lore/relationships.md | 5,873 | ~450 tokens (Pack Layer) | Already mitigated 2026-11-21 (Pack Layer added). Model for the other files. |
| lore/val_devices.md | 2,360 | excerpts | Loyalty progression history now inflates the reference file; needs a Pack block. |
| lore/consort_body_records.md | 1,364 | excerpts | Small; Pack line suffices. |
| characters/priya_raghavan.md | 3,531 | cards total ~800 tokens for 2–4 cards | **Heavy** — Background is reference-only by rule, but no Pack block exists. |
| characters/nia_okonkwo.md / sonya_ivanova.md / yan_rin.md / bog.md / darkwing.md | 2,026 / 2,083 / 1,809 / 1,222 / 1,129 | same | All over a per-card share; same fix. |
| reviews/ (total) | 99,519 | never in writing packs | Editing loads one chapter's review at a time; terminology_log.md grows unbounded — index only. |
| chapters/ (total) | 66,542 | last 1–2 summaries only | Fine as designed. |
| MIGRATION_NOTES.md | 1,494 | never | Historical; confirm exclusion in CONTEXT_PACK. |

## Root causes
1. Append-only accumulation: rulings, histories, and progressions are added to the same files that hold current state (state YAML, val_devices, style guide).
2. Current vs history not separated, except where already fixed (relationships Pack Layer, threads Resolved Archive, cards' Background rule).
3. Budget numbers in CONTEXT_PACK.md were never re-measured as files grew, so overruns are invisible.

## Improvement items (in order; one item per background run)
- **I-1 State YAML slimming.** Move per-character long prose notes out of 02_current_state.yaml into the character cards / lore (where they belong); the YAML keeps snapshot fields only (position, status, loyalty, body, inventory, one-line relationship dict). Verify YAML parses and that no fact is lost (moved, not deleted). Target ≤1,500 words.
- **I-2 Synopsis cap.** Measure 01_synopsis.md by section; rewrite the Synopsis section back to 200–250 words (rewrite, never append — its own rule); keep Turning Points ≤7 and Where We Are Now ≤3 lines.
- **I-3 Style guide core.** Add a marked "Pack Core" section at the top of 04_style_guide.md (the always-load rules, ≤700 words); detailed rulings stay below as reference. Do not split the file (prompts reference this path).
  - **Reference material (supplied by the user 2026-11-21, from the side chat "執筆スタイルガイド改良"):** `reviews/style_guide_improvement_plan.md` — a full style-guide improvement plan (findings F-1–F-9, items SG-1–SG-14, decisions D-1–D-7). Its SG-2 is the same work as this I-3, and SG-1/SG-3 (reorganisation; slimming the Units rule from 292 words to a core rule + pointer to `terminology_log.md` §7) are the natural companions to it. When this project reaches I-3, read that plan first and use it as reference: Pack Core contents should cover the gaps it identifies (Nia's AAVE rule, Priya's stutter register, the rotation list that the beat-sheet template cites but the guide lacks), not only a compression of the current text. Conversely, do not execute the style-guide plan's other items (SG-4 onward) under this project — they need the user's rulings D-1–D-7 in that side chat.
- **I-4 Timeline position block.** Ensure 05_timeline.md opens with a self-contained Current Position block (position, season band, last-10-rows digest) so extraction is copy-one-block, not a judgement call.
- **I-5 Canon index.** Add a section index with one-line summaries at the top of 00_canon.md so excerpts can be pulled by section without loading the whole file.
- **I-6 Character card Pack blocks.** Add a ~120–150-word Pack block at the top of the six major cards (Bog, Nia, Sonya, Rin, Priya, Darkwing): identity, voice essentials, current status at ch130. Rest of each card is reference-only.
- **I-7 val_devices Pack block.** Top block: GCS revealed truth (short form), knowledge restriction, current loyalty values. Progression history stays below as reference.
- **I-8 Body records Pack line.** Top block: current values table only (already compact); logs stay below.
- **I-9 Threads check.** Measure the Open section alone; if >~600 words, tighten one-line-per-thread discipline (details live in chapter summaries). Resolved Archive unchanged.
- **I-10 terminology_log index.** Add a section index at the top (editing lookups); the log itself is never in a pack.
- **I-11 CONTEXT_PACK update.** Re-measure everything after I-1…I-10; rewrite the budget table with real numbers; add the audit command (`wc -w` on the every-time files) and a note that MIGRATION_NOTES.md and reviews/ are never pack material.
- **I-12 Re-audit.** Full re-measurement; compute a realistic total pack size; close the project with a report.

## Guardrails
- Never delete information: move it to a reference layer/file in the same directory system, with a pointer left behind.
- Keep file paths stable (prompts and chats reference them). No manuscript text changes in this project.
- If an item needs a user ruling (e.g. what counts as "current" is genuinely ambiguous), flag it in this log, skip to the next item, and surface it in the completion report — do not guess.
- Verify after each item: YAML parses (I-1), word counts recorded here (before → after), cross-references updated.
- One item per nightly run; silent per run; completion report to the main chat when all items are done or flagged.

## Progress
- 2026-11-21: Baseline measured; plan written (this file). No items started.
- 2026-11-21: Reference material received for I-3: `reviews/style_guide_improvement_plan.md` (style-guide side chat, handed over at the user's direction). See the note under I-3 above.
- 2026-11-21: **I-1 DONE — 02_current_state.yaml 8,107 → 1,497 words (target ≤1,500 met).** Snapshot-only rewrite; YAML parses; all 6 characters and all snapshot fields kept (position, status, loyalty, body, inventory, one-line relationship dicts). Loyalty values (Nia 93%, Sonya 78% [est.], Priya 12%, Rin 18%) and body values verified unchanged; current chapter still 130. changed_facts merged 41 → 11 chapter-group entries; secrets_active still 8; public_knowledge still 1. No information deleted: full pre-slimming text preserved verbatim in `02_current_state_archive_2026-11-21.yaml` (8,107 words, reference only, never in packs), with a pointer in the slim file's header; chapter-level detail lives in `chapters/chXXX.md`, relationship detail in `lore/relationships.md` (synced ch130), GCS/loyalty progression in `lore/val_devices.md`, body records in `lore/consort_body_records.md`. Deliberate choices: relationship dicts trimmed to load-bearing entries only (full detail already in relationships.md); moved prose was NOT pasted into character cards (cards are also over budget; I-6 handles them — the archive + chapter summaries hold the detail). Noted gap, not fixed here: the original file never had changed_facts entries for ch120–121 and ch123–130 (only character entries covered them); the slim file records this in a comment rather than inventing entries. No user ruling needed. Next item: I-2.
