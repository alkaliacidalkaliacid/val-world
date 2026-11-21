# Migration Notes - The Ashen Dominion

## Decisions made by the user (2026-11-17)
- Resistance alliance: **The Old Guards** (unified). "Ash Guard" was an earlier concept name.
- Highway raiders: **Raiders** (unified). "The Cinder Kings" is abandoned.
- Smuggler network: **Traders** (unified). "The Gilded Hand" is abandoned.
- Protagonist: **Bog**, a low-ranking Val soldier of the invading Dominion. **Nia is his partner.** Bog was entirely absent from the original setting document - a provisional card (characters/bog.md) has been created and is mostly [UNKNOWN].
- Cults: no proper name, deliberately.
- **The Uncrowned: abolished.** Former supervillains belong to various separate groups (e.g. the League of Shi).
- Story present: **provisionally 2047**, on the understanding that it can be retroactively revised if a contradiction appears.
- **The Bound**: adopted as the term for collared captive heroes.
- Theme: "A deranged, erotic, slapstick sci-fi fantasy"
- Promise to the reader: "Entertaining you—without the political correctness!"
- Ending direction: "After a long journey filled with both hardships and joys, Bog builds the ultimate harem and finds happiness—but when all is said and done, Nia remains his number one!"

## Pending tasks
- [~] Prose unification pass (running, per dump): dump 1 had 1 hit ("Ash Guard camp" -> fixed in manuscript). Dump 2 had 1 hit ("Raiders, probably Cinder Kings" -> "Raiders, hired muscle", ch019). Archive originals are never edited; fixes live in manuscript/ and are logged in chapters/_session_to_chapter_map.md.
- [ ] Same check for "Ash Guard" in draft prose -> "The Old Guards".
- [ ] Step 4: chapter summaries for sessions 33–48 only (Mississippi / Florence) — awaiting the prose dumps. Sessions 1–32 are done (ch001–048, summaries verified 40–60 words each). Session → chapter rule decided 2026-11-17: use Claude's auto-generated chapter divisions as-is. Worksheet at `chapters/_session_to_chapter_map.md` is filled for sessions 1–32; only 33–48 remain blank.

## Resolved at step 3 (2026-11-17)
- Black Huntress's powers list duplicated strength in the source (`archive/black_huntress.md`: "Exceptional physical strength" in the Powers line and again in the awakening paragraph). Consolidated to a single phrasing in `characters/nia_okonkwo.md` ("Exceptional strength, dense skin, heightened agility...").
- Bog has no character document anywhere; confirmed at step 3. `characters/bog.md` is built from the summary alone, with unknown fields marked [UNKNOWN]. Nothing further to expect at the character step.
- Priya's surname is now known: Raghavan (`characters/priya_raghavan.md`).
- Sonya's card is built (`characters/sonya_ivanova.md`, from `pale_murderess.md`).

## Findings from the Bog & Nia summary (2026-11-17)
- The summary calls itself an "Ashen Dominion side story" - RESOLVED 2026-11-17: that label was added by Claude (Claude.ai) on its own. The Bog & Nia line IS the main storyline. Ignore the label.
- The summary still uses "Cinder Kings" 3 times (Part A, session 38, Part C) despite the Raiders unification. Covered by the pending prose unification task; instance files use "Raiders".
- The summary references documents not yet received: `black_huntress.md`, `pale_murderess.md`, `yan_rin.md`. Needed at step 3. — RESOLVED 2026-11-17: all received (Rin's arrived as `orange_clobberess.md`, not `yan_rin.md`), plus `red_mediatoress.md`; all archived.
- The source is organized by sessions (1-48), not chapters. Chapter mapping decided at step 4 (2026-11-17: use Claude's divisions as-is); filled in `chapters/_session_to_chapter_map.md` for sessions 1–32, pending 33–48.
- Bog has no character document anywhere; characters/bog.md was built from the summary alone. — Confirmed; see Resolved at step 3 above.
- Priya's surname is never given. Sonya's card is still to be built (step 3, from pale_murderess.md). — RESOLVED: Raghavan; Sonya's card built.

## Migration progress
- [x] Step 1: Settings / world -> 00_canon.md, lore/factions.md, lore/val_devices.md, source archived
- [x] Step 2: Existing synopsis -> 01_synopsis.md (215 words). Source archived.
- [x] Step 3: Characters -> DONE 2026-11-17. Cards: Bog, Nia (definitive), Sonya, Yan Rin, Priya Raghavan, Darkwing, the tentacle monster, all 12 roster heroes, and a shared _minor_cast.md (Broker, Dr. Hermes, Arjun, Dadi, the five former supervillains from lore, etc.). Source docs archived (black_huntress.md, pale_murderess.md, orange_clobberess.md, red_mediatoress.md).
  - Notes: Rin's file arrived as `orange_clobberess.md`, not `yan_rin.md`. Priya's surname is Raghavan. `red_mediatoress.md` itself flags how Priya and Arjun met as an unconfirmed draft - marked [UNCONFIRMED DRAFT] in her card, not canon. Sonya's vocabulary count: her doc says 334, the summary's session 48 says 335; the state file uses 335 (later). Lookalike traps flagged in the cards: Sunspike (Asha Raman) vs Priya Raghavan; Afterimage (Sofia Petrov) vs Sofiya Ivanova. Minor ambiguity left open: Hermes's clinic is called the Appalachian branch, while Rin speaks of driving to Tennessee - the branch may simply be in Tennessee.
- [~] Step 4: 02_current_state.yaml pre-filled from the summary's Part C. Prose dump 1 received 2026-11-17 (18,096 words): it already had chapter divisions and titles - ch001-ch013, covering summary sessions 1-9. Prose split into manuscript/ (plus a full-volume copy), chapter summaries written for all 13 (each verified at 40-60 words), naming fix applied in the manuscript copy only ("Ash Guard camp" -> "Old Guards camp", ch008; the only banned-name hit in the dump). Prose dump 2 received 2026-11-17 (4,859 words; internal sections 1-8 adopted as ch014-021, covering summary sessions 10-14). Summaries written for all 8 (verified 40-60 words).
Prose dump 3 received 2026-11-17 (10,259 words; sections 1-19 adopted as ch022-040, covering summary sessions 15-24, the depot raid). Summaries written for all 19 (verified 40-60 words; all 40 chapter summaries now pass). No banned-name hits.
Prose dump 4 received 2026-11-17 (3,595 words; Prologue + Chapters 1-7 adopted as ch041-048, covering summary sessions 25-32, The Burrow). Summaries written for all 8 (verified; all 48 chapter summaries now pass). No banned-name hits. FORM NOTE (user, 2026-11-17): the Burrow part is barely in novel form (dialogue/log style); whether to edit it into prose is to be considered AFTER the migration completes - do not edit it during migration.
Prose dump 5 received 2026-11-17 (5,649 words; sections 1-6 adopted as ch049-054, covering summary sessions 33-38, Mississippi). Summaries written for all 6 (verified; all 54 chapter summaries now pass). One banned-name hit ("Cinder Kings", Darkwing dialogue) unified to Raiders in the manuscript copy.
Prose dump 6 received 2026-11-17 (7,694 words; sections 1-16 adopted as ch055-070, covering summary sessions 39-48, Florence). Summaries written for all 16 (verified; ALL 70 chapter summaries pass at 40-60 words). No banned-name hits.

## MIGRATION COMPLETE (2026-11-17), plus one extra dump
All four steps done: (1) canon/lore, (2) synopsis + state + threads + style, (3) 20 character files, (4) full prose as 71 chapters with 71 summaries. Instance inventory: chapters/ 71 summary files + map; manuscript/ 71 chapter files + 7 part volumes; archive/ 13 source files (unedited); characters/ 20 files; 02_current_state.yaml valid.
Extra dump (2026-11-17): "The Road to Tennessee" (15,348 words, single chapter -> ch071), prose NOT covered by the Bog & Nia summary - it continues past session 48: the reunion happens, Rin is collared with a Hermes-lab collar and made third consort, Priya partly buries the singularity, the laser and the suit are lost.
TOP POST-MIGRATION TASK: refresh 01_synopsis.md (rewrite, 200-250 words), 02_current_state.yaml, and 03_open_threads.md to the post-ch071 "now" before new writing starts - they currently describe the session-48 state.
Other open post-migration items (user decisions):
- Whether to edit the Burrow chapters (ch041-048) from dialogue/log form into novel prose.
- Whether to create arc summary files in arcs/ (e.g. one per dump part).
- Instance folder renamed by the user on 2026-11-17: novel-instance-en -> val-world (this folder). Backup regenerated as val-world_backup_2026-11-17.zip.
- ch071 is 15,338 words in a single chapter (source's own division, adopted as-is); it has clear scene breaks if the user ever wants it split.
- Next step after this chat: start a fresh writing chat from the finished instance. Chapter divisions: the user decided (2026-11-17) to use Claude's auto-generated chapter divisions as-is - so ch007 is NOT split, ch011 stays whole, and ch002 stays a short beat chapter. Worksheet `chapters/_session_to_chapter_map.md` is now filled for sessions 1–32; only sessions 33–48 remain blank.
- [~] Step 5: 03_open_threads.md pre-filled from the summary's Part C (T01-T12); 04_style_guide.md filled from its Part D.

## Post-migration refresh DONE (2026-11-17, editing chat)
The TOP POST-MIGRATION TASK above is complete: 01_synopsis.md rewritten (239 words), 02_current_state.yaml overwritten (current_chapter: 71, all six active characters at the mountain / burrow / bunker as of ch071's end), and 03_open_threads.md refreshed - all to the post-ch071 state. Threads: T04 (reunion) resolved in ch071 and archived; T13 (what Bog hides from Nia), T14 (Priya and Nia's talk), T15 (Darkwing's reaction) added; T02, T03, T08, T12 updated. 14 threads open. YAML validated; banned-name scan clean. Remaining user-decision items: Burrow prose edit (ch041-048), arc summaries in arcs/, splitting ch071.

## Chapter numbering padded to 3 digits (2026-11-21)
At the user's direction, all chapter identifiers were padded from 2 to 3 digits (ch01 -> ch001) across the instance: 312 files renamed (manuscript/, chapters/, reviews/, blocks/, translation/), range endpoints padded as well (part01_ch001-013.md, volume05_ch091-108.md), and in-text references updated in the same pass (255 files). part / arc / volume numbers unchanged. archive/ untouched (it contains no chNN references). The PDFs contain no chNN identifiers (chapter headings only), so they were not regenerated. Pre-rename snapshot: ~/workspace/val-world_pre-rename_2026-11-21.zip.
