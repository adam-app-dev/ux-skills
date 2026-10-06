# CLAUDE.md

Instructions for any agent working in this repo.
Before anything else, read README.md, SKILL.md, sources.md and every file
in principles/ and rules/ so you know what already exists.

## What this repo is

- ux-skills holds JUDGMENT: what makes a screen work and why. It never holds
  VALUES (colors, fonts, spacing numbers, components). Those belong to each
  project's design system.
- `principles/` = how people think (psychology). Usable in any feature, never
  tied to one screen type.
- `rules/` = how a screen is built (choosing a view, imagery, layout,
  hierarchy, typography, placement, wording, navigation, inputs, states).
- `SKILL.md` = entry point with the core rule ("design for every case, not the
  demo case"), both indexes, and the honesty guardrails.
- `sources.md` = every rule traces back to a source.

## Workflow: adding tips from a UX video

The user gives a YouTube link plus the transcript of a UX video. For each video:

1. **Extract** the real tips. Ignore sponsor segments and course promos.
2. **Sort** every tip with this test:
   - True in any app? → ux-skills (which file, existing or new)
   - About how one project looks (font, palette, spacing values)? → "design
     system", not this repo
   - A decision about one project's feature? → "project brain", not this repo
   - Not useful → skip, with the reason
3. **Show a sorting table BEFORE writing anything:**
   `| Tip | Goes to | Written as (general rule) |`
   Then list separately: design system items, skipped items, and flags.
4. **Flag** anything that is:
   - web-only and doesn't apply to mobile apps (the user builds in Kotlin
     Multiplatform / Compose)
   - an accessibility risk (contrast below WCAG AA 4.5:1, missing screen reader
     labels, tap targets too small)
   - manipulative: fake progress, fake countdowns, shaming "no" buttons,
     pre-ticked paid extras. These break the honesty guardrails in SKILL.md.
     Keep the useful idea, drop the trick, and write a note in the file saying
     the source suggested it and this repo deliberately doesn't.
   - a shaky statistic: keep it as a story, mark it as illustration, not fact.
5. **Wait for approval.** The user may move or skip items.
6. **Write** the approved changes:
   - Write rules in general terms that work for any app, not just the screen
     in the video. Examples must be generic (amounts, profiles, lists,
     settings), never tied to one of the user's projects.
   - Follow the existing file shapes exactly.
     - Rules: title, Why, Do, Don't, optional Example, Source.
     - Principles: memory hook, idea, why it works, before/after, where it
       applies, do, don't, guardrail, source.
   - Paraphrase in your own words. Never copy transcript text verbatim.
   - Add to an existing file when the topic fits; create a new file only when
     nothing fits, and say why.
   - For any new file, update the SKILL.md indexes (with a memory hook and a
     "read it when..." line), plus sources.md, and README.md if the structure
     changes.
7. **Show the full git diff**, then commit with a clear message and push.
   The remote is already set up (`git@github.com-adam:adam-app-dev/ux-skills.git`);
   don't change it.
8. **Remind the user:** the ux-skills rules are copied into design systems
   in Claude Design, so they don't update by themselves. Tell them to open
   each design system that has a `ux-skills/` folder (currently: Pet Design
   System) and ask it to "sync ux-skills".

## How to talk to the user

- Simple language, concrete examples, as if they're new to the topic.
  No jargon unless asked.
- Keep replies short.
- Before writing anything, say whether the video's content belongs here at all.
