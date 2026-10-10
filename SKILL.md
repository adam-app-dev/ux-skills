---
name: ux-skills
description: Portable UX judgment for designing and building app screens and features. Use whenever designing, building, reviewing or redesigning any screen, flow or feature UI, in Claude Design or in code (Compose, KMP, web), even if the user doesn't mention UX, psychology or best practices. Covers how people think and decide (defaults, progress, trust, ownership, loss, comparison, easy decisions, transparency, user stage, social proof) and concrete screen rules (choosing a view, imagery, layout, hierarchy, typography, placement, wording, navigation, inputs, filters, states).
---

# UX Skills

This skill holds **judgment**: what makes a screen work for people, and why.
It never holds **values** (colors, sizes, spacing numbers, fonts, components).
Those come from the project's own design system.

- ux-skills says: "the main action must stand out"
- the design system says: "the main button is a green pill"

If a rule here seems to conflict with the project's design system,
follow the design system for how it looks, and this skill for what it does.

The design system's components are the defaults, not the limit. When a
screen's purpose needs something the library doesn't have, build it from
the design system's tokens and mark it as a proposed new component, so
the user decides whether it joins the system.

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
4. For a new screen or feature, explore before you build (next section)
   and wait for the user's choice.
5. Build the chosen direction with the project's design system for
   visuals.
6. Run the core rule check above.
7. When you deliver, list which principles and rules you applied and where,
   in one line each, so the work can be reviewed, plus any proposed new
   components.

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
| [Filters](rules/filters.md) | Filters help people explore, not fill in a form | lets people narrow or sort a large set (filters, sort, result counts, ranges) |
| [States](rules/states.md) | Still works when there's nothing to show | can be empty, loading, failed or offline (lists, dashboards, search) |
| [Choosing a view](rules/choosing-a-view.md) | The purpose picks the view | shows a set of items or data and you're choosing how (list, grid, cards, timeline, summary, calendar, map), is a new screen, or the user is unsure |

## Explore before you build

Do this by default for any new screen or feature, and whenever the user
is unsure or asks for ideas. Skip it only for small changes to an
existing screen, when the user already described the exact layout, or
when they say to just build it.

1. List what the screen needs that the user didn't mention: states
   (empty, loading, error, offline), edge cases from the core rule,
   missing fields or actions. Keep it short, and wait for the user's
   answer.
2. Start from the purpose, not from the component library: is the user
   here to scan, compare, track, act fast, or enter data? What question
   must the screen answer first?
3. Look at how strong, shipped products solve the same problem. If a
   screen reference library is connected as a tool (for example the
   Mobbin MCP), use it: find the most relevant real screens and flows,
   name the patterns they share and where they differ, and show the
   references. If none is connected, work from what you know and say so.
   References show what's possible; they don't replace this repo's
   rules, and patterns that break the honesty guardrails are not copied.
4. Read [rules/choosing-a-view.md](rules/choosing-a-view.md).
5. Propose 2 to 3 clearly different directions, not three versions of
   the same layout. Different means a different structure: what leads
   the screen, which view holds the content, where the main action
   lives, or whether it's a screen at all (a bottom sheet, an inline
   edit, a step in a flow).
6. At least one direction must go beyond what the design system's
   components already show, when the purpose allows it. Name the new
   element it would need.
7. For each direction, give one or two lines: what it does best, what
   it costs, and which rules support it. Recommend one, and wait for
   the user's choice.
8. Build only the chosen direction. Reuse existing components where
   they fit; build anything new from the design system's tokens and
   mark it "proposed new component".

Creativity happens inside the rules, never against them. Being new is
not a reason on its own: every direction must serve the screen's
purpose. If an idea breaks a rule, name the rule and let the user
decide.

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
