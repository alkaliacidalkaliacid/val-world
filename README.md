# LLM Long-Form Novel Template - Hierarchical Summaries + State Management

A template set designed so that the context you pass when generating does not grow, even as the story gets longer.

## How this answers "summaries keep bloating"
- Summaries bloat when you keep appending to a single file → Hierarchize them, and rewrite the upper levels at a fixed length
- Summaries bloat when you write them as prose → Manage current state by overwriting a YAML file
- Summaries bloat when you read everything every time → Limit what you pass to a fixed set (CONTEXT_PACK)

As a result, whether you're on chapter 10 or chapter 100, the amount you pass stays constant at roughly 4,000-5,000 tokens.

## Folder Structure
```
novel-llm-template-en/
├── README.md                ← This file
├── CONTEXT_PACK.md          ← Fixed list of what to include every time (most important)
├── 00_canon.md              ← Immutable canon
├── 01_synopsis.md           ← Full synopsis (fixed length, rewrite only)
├── 02_current_state.yaml    ← Current state (overwrite only)
├── 03_open_threads.md       ← Open foreshadowing only
├── 04_style_guide.md        ← Style and anti-repetition
├── 05_timeline.md           ← Story timeline, one row per chapter (anchor: Day 1 = ch01)
├── characters/
│   └── _template_character.md
├── arcs/
│   └── _template_arc.md
├── chapters/
│   ├── _template_beat_sheet.md
│   └── _template_chapter_summary.md
└── prompts/
    ├── 01_beat_planning.md       Beat planning
    ├── 02_write_chapter.md       Write the chapter
    ├── 03_extract_diff.md        Extract the diff
    ├── 04_rollup_synopsis.md     Compress when an arc ends
    └── 05_critique_repetition.md Repetition check
```

## Workflow for One Chapter
1. **Beat planning** - Use prompts/01. Don't write prose yet. Kill chapters with no change at this stage
2. **Write the chapter** - Use prompts/02. Include only the fixed set from CONTEXT_PACK. **After writing, always present the manuscript file itself in the chat** (attach the chapter's manuscript file so the user can open it — user instruction, 2026-11-20). This applies to the first draft and to every revised version.
3. **Repetition check** - Use prompts/05 to get feedback only, then fix only those passages
4. **Extract the diff** - Use prompts/03 to extract only the diff, update 02_current_state.yaml and 03_open_threads.md, and create the chapter summary
5. **Only when an arc ends** - Use prompts/04 to create the arc summary and rewrite 01_synopsis.md

## Getting Started
1. Fill in 00_canon.md and 04_style_guide.md
2. Create character cards in characters/ for your cast
3. Write your current plan into the synopsis in 01_synopsis.md
4. Set the initial state in 02_current_state.yaml
5. Run the workflow above

## Three Rules That Make This Work
1. The only files you append to are chapter summaries and the archive. Everything else is overwritten or rewritten
2. Never put the full prose of past chapters into context. At most, the previous scene
3. Delete resolved foreshadowing. Keeping it is another source of bloat and confusion
