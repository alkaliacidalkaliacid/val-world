# Prompt 05: Repetition Check (for revision, keep separate from generation)

## What to include
- The prose you just generated
- Previous chapter summary, and if possible only the opening and ending of the previous chapter's prose
- The banned patterns from 04_style_guide.md

## Prompt
```
Do not rewrite the prose. Point out problems only, from the following angles:

1. Repetition: Phrasing, metaphors, emotional expressions, or scene transitions similar to the previous chapter
2. Lack of change: Places where nothing has changed between the start and end of the chapter
3. Easiness: Coincidences, expository dialogue, or conflicts settled just by talking
4. Style guide violations: Anything that hits a banned pattern

For each point, add a one-line suggestion for how to fix it. If there are no problems, reply only with "No issues."

[Paste prose here]
```

## How to use it
Ask for a rewrite only of the flagged passages. Rewriting the whole chapter wastes tokens and homogenizes the parts that were already good.
