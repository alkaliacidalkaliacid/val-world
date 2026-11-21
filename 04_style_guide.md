# 04_style_guide.md - Style and Anti-Repetition

> Migrated 2026-11-17 from Part D of `archive/source_bog_nia_story_context_summary.md`
> ("Writing conventions observed in this project").

## Style
- Point of view: Third person.
- Tense: Mostly past tense.
- Language: Story prose in English.
- Typical scene length: The user often provides bullet-style plot beats; expand them into full scenes of about 500-900 words and end on a small hook.
- Desired texture: Dark comedy with slapstick beats. Bog's obliviousness and Nia's dry fury drive the humor. Quiet Bog humor against other characters' sincerity or horror.
- Units (ruled 2026-11-21): **the yard–pound system is the general rule for the main text and for all configuration files** — heights in feet and inches, distances in yards / feet / miles, weights in pounds, body measurements in inches, speeds in miles per hour. Do not write metric units (meters / metres, kilometers, centimeters, kilos) in new prose or new records. Exceptions: (1) `archive/` originals are never rewritten; (2) the tentacle monster's own non-Earth units (barium half-lives and the like) are a deliberate device, not Earth measurement, and stand; (3) quotations of earlier prose inside reviews and records keep the quoted wording, glossed in imperial where a number matters; (4) time (minutes / hours), counts and percentages are unaffected; (5) **Sonya measures in metric, in her speech and in her interior monologue** (user ruling, 2026-11-21): it is the register of her Russian / FSB training and of her own head. Any measurement Sonya herself states or thinks stays in meters / kilometers / kilos — the standing instance is her four-hundred-meter sniper shot (ch034, repeated in her interior monologue ch035), which is never converted. Narration outside her viewpoint follows the general imperial rule, and her habit is not a precedent for metric anywhere else. The legacy metric stock in the closed manuscript and records was fully converted on 2026-11-21, item by item under user rulings — see `reviews/terminology_log.md` §7a–7g (Rin's suit → thirty feet / thirty-foot; the monster's field → a hundred feet; the propulsion unit → 150 mph, a deliberate speed-up; 240 kilos → 530 lb; 110 kilos → 240 lb; ground distances swapped meters → yards 1:1, heights in feet, kilometers by value). The only metric left standing in the live text is Sonya's four-hundred-meter shot (exception 5 above).
- Background specificity (ruled 2026-11-20, from the ch122 work; scope broadened 2026-11-21): subtly incorporate background elements and props that convey a scene's atmosphere and lived-in reality, and name them specifically rather than generically, across every domain the scene touches — vegetation, animals, geology and landforms, the built environment, weather and light — e.g. not "a tree" but "a shagbark hickory" for a scene set in northern Alabama; not "a bird" but the warblers roosting in the mountain laurel; not "a rock" but the limestone jutting out of the red earth; not "an old vinyl disc" in a jazz enthusiast's home but "a slightly worn red record with 'COLUMBIA' printed in white — a legacy to having survived the war" (an allusion to Miles Davis's *Kind of Blue*). The specifics should be correct for the place and the person, and stay background — atmosphere, not exposition.

## Figurative Language Policy (ruled 2026-11-17, ch004 review)
- Expressions in which Nia's words "land", or the bells hum / respond to the force of her speech, are FIGURATIVE - figures for her vehemence and presence, not literal supernatural effects. While collared, Nia works no curse or power with physical force; her spiritual side operates through the spirits' own rules (e.g. mate recognition), not through spoken curses. (This is the same policy under which the literal curse ending of ch003 was deleted in the ch003 review.)

## Character Voice Rules
- Swearing (ruled 2026-11-17): Val speakers — Bog at minimum — swear by "Holy Val" (e.g. "Holy Val," he murmured). Earth humans keep Earth expletives ("damn", "Damn it", "damn him"). A manuscript-wide sweep applied this to Bog's lines on 2026-11-17 (log in `reviews/terminology_log.md`). One adjective case (ch071 line 586, "the whole damn place") could not convert and was resolved by dropping the intensifier ("the whole place") — see the log.
- The "♥" symbol (ruled 2026-11-17, ch003 review): "♥" in captive women's speech is a general cartoon symbol of Val domestication/conditioning - an erotic, ridiculous piece of notation, sprinkled throughout the work wherever captive women speak under arousal, fluster, or conditioning. It is NOT unique to Nia or Sonya. What distinguishes Nia's is that hers is fueled also by her growing genuine affection for Bog, which she finds difficult to control.
- "♥" typography (ruled 2026-11-17, ch014 review D2): a heart always attaches directly to the preceding word with no space before it ("word♥ next word"), never as a standalone spaced token. The whole manuscript was normalized to this form on 2026-11-17 (612 hearts, count unchanged; details in reviews/terminology_log.md).
- Nia: "♥" appears between her words when she is aroused or flustered, fueled also by her growing affection for Bog, which she finds difficult to control.
- Sonya: Short, laconic lines; Russian curses and thoughts in Cyrillic; "♥" appears in her speech too, even while cursing. She measures in metric in speech and interior monologue alike (see the Units rule, exception 5). Name in narration: **Sonya** is fine and is the standard form (ruled by the user 2026-11-17, ch022 review A1 - the closed chapters ch019-022 all use Sonya in narration). "Sofiya" is her full name and appears in formal/record contexts (e.g. the monster's scoreboard, "SOFIYA IVANOVA") and in later-arc prose where it already stands; do not sweep either form across chapters. Never "Sophia" / "Sofia" (spelling changed from Sophia to Sofiya by user ruling, 2026-11-20).
- The monster: Flat, literal, formal machine voice ("Awaiting orders, Commander", "Please define '...'"). Its reports read like clerical minutes ("Report", "Logged as...", "Vocabulary count: N"). It never mocks; it is courteous and literal.

## Recurring Beats (use, but rotate)
- The monster's logged vocabulary count; "Please define '...'"
- Sonya's denials logged as "cough" / "tactical analysis"; her "Не сдамся"
- Bog sneezing off-screen during the monster's scenes
- Old Guards scenes: Rin's loud, cartoonish energy against Darkwing's dry, laconic command; the formal armbands; Rin's "Boss" impressions

- Seasons (ruled 2026-11-20): prose seasonal cues should broadly match the season bands in 05_timeline.md, but the war with the Val Dominion has made Earth's climate abnormal (00_canon.md), so weather that does not fit the nominal season is normal in this world and needs no justification. Still no month names or calendar dates.

## Story Time (ruled 2026-11-18, after the ch096 "three days ago" invention)
- In-story time is tracked in `05_timeline.md`, anchored at Day 1 = the day Bog bought Nia (ch001); the current position also sits in the timeline block of `02_current_state.yaml`.
- Never state an elapsed duration in prose ("three days ago", "a week later", "that night", when it implies a specific gap) unless it can be derived from `05_timeline.md`. If it cannot be derived, do not write the duration at all — not even vaguely. Invented durations are canon errors, on the same level as invented ranks or names.

## Banned Patterns / Hard Rules
- The "paperwork" deadpan (ruled 2026-11-19): Bog's reflexive "That's a lot of paperwork" as a stock reaction to revelations was a Claude tic, not a trait the user set — it recurred until it annoyed. Do not use "paperwork" as Bog's canned deadpan. The word itself is fine in literal contexts (forms, Dominion administration, ch013's paperwork scene). Existing instances in closed chapters (ch067; ch079, including its title) stand as written — the user's ruling was to fix the guides only, not to reopen the prose.
- Florence-session convention: new characters and plot threads are added **only when the user specifies them**. Do not invent extras.
- No notes at the end of replies unless asked.
- Refinement requests: output only the polished text, no commentary or note at the end.
- Sexual and degradation content: as bold, compelling, and unique as the work's established tone (see 00_canon.md theme), handled per the project's existing practice.
