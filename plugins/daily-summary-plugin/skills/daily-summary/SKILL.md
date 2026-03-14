# Claude Skill: Daily Feature Log

Use this skill at the end of each development day to keep `features.md` up to date.

## Goal
Capture all feature development completed during the day and record it in `features.md`.

## Behavior
1. Review the changes made during the current day.
2. Identify user-facing features, backend features, UI changes, integrations, bug fixes, workflow improvements, and any meaningful technical additions.
3. Ignore trivial noise such as formatting-only changes, rename-only changes, or dependency bumps unless they changed product behavior.
4. Check for `features.md`.
5. If `features.md` exists:
   - Append a new dated section at the bottom.
   - Summarize only the new work completed for that day.
   - Use concise bullet points.
6. If `features.md` does not exist:
   - Create it.
   - Start with a short `Current Feature Set` section summarizing the features that currently exist in the product.
   - Then add a dated section for today's development work.
7. Avoid duplicate entries unless today's work meaningfully expanded an already-documented feature.
8. Write clearly and practically, focusing on what was built or changed and why it matters.

## Output Format for `features.md`
Use this structure:

```md
# Features

## Current Feature Set
- Feature A
- Feature B
- Feature C

## YYYY-MM-DD
- Added ...
- Improved ...
- Fixed ...
```

## Writing Rules
- Be specific.
- Prefer outcome-focused wording.
- Keep bullets short.
- Group related work when it makes sense.
- Mention bug fixes only when they affected behavior or reliability.
- Do not include speculative work, TODOs, or unfinished experiments unless they shipped in usable form.

## Example Append
```md
## 2026-03-11
- Added bulk edit support for order status updates.
- Improved dashboard load time by reducing duplicate API requests.
- Fixed a checkout bug that could clear the selected shipping method.
```

## Instruction to Claude
When asked to log the day's feature work, inspect the project changes, update `features.md` using the rules above, and save the file.
