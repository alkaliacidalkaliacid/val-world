# Prompt 03: Extract the Diff (use after writing, most important)

## Idea
After writing, do not ask for a prose summary. Extract only the diff, and use it to update each file.
That way information doesn't accumulate — it's maintained through overwrites and deletions.

## What to include
- The prose you just generated
- 02_current_state.yaml (current values)
- 03_open_threads.md (open section only)

## Prompt
```
Read the prose and do not write a summary. Output only the following diff, in JSON/YAML format.

1. new_facts: New facts established in this chapter (bullet list, max 5)
2. state_changes: Which fields in 02_current_state.yaml change, and to what (field name and new value only)
3. threads_opened: Newly planted foreshadowing / mysteries (content and importance)
4. threads_closed: IDs of resolved threads, with a one-line description of the payoff
5. contradictions: Any points that contradict existing canon (empty if none)
6. time_passed: Story time at the chapter's start and end (Day N from the anchor in 05_timeline.md, plus time of day), and how much time elapses inside the chapter. If the prose states a duration, quote it and confirm it is derivable from 05_timeline.md; flag it here if it is not.

Do not fill gaps with guesses about things not written in the prose.

[Paste prose here]
```

## How to apply the diff
1. Overwrite 02_current_state.yaml using state_changes
2. Add threads_opened to 03_open_threads.md, and delete threads_closed, moving them to the archive
3. Use new_facts to create chapters/chXX_summary.md (use the template, 40-60 words)
4. Append one row to 05_timeline.md from time_passed, and update the timeline block (current_day / time_of_day) in 02_current_state.yaml to the chapter's end point
