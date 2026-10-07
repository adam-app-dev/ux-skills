---
name: ux-skills
description: Portable UX judgment for designing and building app screens and features. Use whenever designing, building, reviewing or redesigning any screen, flow or feature UI, in Claude Design or in code (Compose, KMP, web), even if the user doesn't mention UX, psychology or best practices. Covers how people think and decide (defaults, progress, trust, ownership, loss, comparison, easy decisions, transparency, user stage, social proof) and concrete screen rules (choosing a view, imagery, layout, hierarchy, typography, placement, wording, navigation, inputs, states).
---

# UX Skills

This skill holds **judgment**: what makes a screen work for people, and why.
It never holds **values** (colors, sizes, spacing numbers, fonts, components).
Those come from the project's own design system.

- ux-skills says: "the main action must stand out"
- the design system says: "the main button is a green pill"

If a rule here seems to conflict with the project's design system,
follow the design system for how it looks, and this skill for what it does.

## Core rule: design for every case, not the demo case

A screen that only works with the example content is broken.
Before delivering, test it in your head against the real range:

- Images: dark, bright, busy, user-uploaded, missing
- Text: very short, very long, other languages (Italian and German run long)
- Lists: empty, one item, a hundred items
- Numbers: zero, huge, negative, with decimals
- States: loading, error, offline
- Devices: small phone, large phone, wide screen, large text setting,
  light and dark mode

Design for the system the screen lives in, not the one screenshot.

## How to use it on any screen or feature

1. Name what the user is trying to do on this screen (decide, enter data,
   track progress, act, compare, buy).
2. Scan both indexes below. Pick what genuinely fits.
   Usually 1 to 3 principles; rules apply more broadly.
   Never force everything in.
3. Read only the files you picked. Each has examples: use them to
   recognize the "before" in your own screen.
4. Apply them using the project's design system for visuals.
5. Run the core rule check above.
6. When you deliver, list which principles and rules you applied and where,
   in one line each, so the work can be reviewed.

## Principle index (how people think)

| Principle | Memory hook | Look for it when the screen... |
|---|---|---|
| [Smart defaults](principles/smart-defaults.md) | Defaults feel like recommendations | asks the user to choose or enter anything |
| [Head start](principles/head-start.md) | Zero feels like standing still | has steps, goals, completeness or a checklist |
| [Give first](principles/give-first.md) | A gift creates a debt | asks for an account, data, permission or payment |
| [Ownership](principles/ownership.md) | What I built or chose is mine | can be personalized, named or built by the user |
| [Loss framing](principles/loss-framing.md) | Losing hurts twice as much as gaining | asks the user to act, keep, turn on, or confirm a destructive step |
| [Contrast](principles/contrast.md) | The first number becomes the ruler | shows a price, amount, score or statistic |
| [Where they are](principles/where-they-are.md) | Day 1 and day 100 need different screens | is seen by both new and regular users (home, dashboards, empty states) |
| [Social proof](principles/social-proof.md) | People follow people | shows ratings, reviews, counts, or a "most chosen" option |
| [Easy question](principles/easy-question.md) | Every screen asks a question; make it an easy one | asks the user to decide, pay, or pick between options |
| [Show the catch](principles/show-the-catch.md) | Say the catch before they find it | involves a charge, trial, deadline, fee, limit or cancellation |

## Rules index (how a screen is built)

| Rule file | Memory hook | Read it when the screen... |
|---|---|---|
| [Imagery](rules/imagery.md) | Works on any photo | shows photos, especially with anything on top of them |
| [Layout](rules/layout.md) | One grid, meaningful space | has more than one section (almost always) |
| [Hierarchy](rules/hierarchy.md) | Clear, never shouting | has a title, buttons or actions, stats or values, icons, colors, dividers or shadows |
| [Typography](rules/typography.md) | Headlines attract, paragraphs support | has text beyond a single label |
| [Placement](rules/placement.md) | Put it where the user needs it | has information the user needs to decide or act |
| [Wording](rules/wording.md) | Specific words do the convincing | has buttons, titles, dates, totals or helper lines |
| [Navigation](rules/navigation.md) | The backbone, not a toolbox | has a bottom bar, tabs, a side rail or moves between main sections |
| [Inputs](rules/inputs.md) | Match the input to how often and how exactly | asks the user to enter numbers, amounts or values, or to pick or select options |
| [States](rules/states.md) | Still works when there's nothing to show | can be empty, loading, failed or offline (lists, dashboards, search) |
| [Choosing a view](rules/choosing-a-view.md) | The purpose picks the view | shows a set of items or data and you're choosing how (list, grid, cards, timeline, summary, calendar, map), or the user is unsure |

## When the user is unsure or asks you to be creative

1. Start from the feature's purpose: is the user here to scan, compare,
   track, act fast, or enter data?
2. Read [rules/choosing-a-view.md](rules/choosing-a-view.md).
3. Propose 2 to 3 clearly different approaches, each with one line on
   which rules support it. Recommend one, and wait for the user's choice.
4. Creativity happens inside the rules and the design system, never
   against them. If an idea breaks a rule, name the rule and let the
   user decide.

The common thread of the principles: people don't decide logically.
They react to what is pre-chosen, what they already have, what they just
saw, and how close the finish line feels. Design for that, honestly.

## Honesty guardrails (apply to every principle)

These principles influence behavior, so they must stay honest:

- Everything shown must be **true**: real progress, real losses, real numbers.
- No invented urgency: no fake countdowns, no fake scarcity.
- The "no" option stays neutral and easy to find ("Not now"), never shaming
  ("I'll risk it", "No, I don't care about my pet").
- Defaults must serve the user, never pre-tick paid extras or marketing consent.

If a principle can only work by breaking one of these, don't apply it.
Some source material suggests tactics that break these rules; this repo
deliberately does not follow them (reasons: EU rules against manipulative
design, app store review policies, and user trust).

## Coming later

- `checklist.md`: final self-check before delivering a screen
