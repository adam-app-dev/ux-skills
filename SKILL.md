---
name: ux-skills
description: Portable UX judgment for designing and building app screens and features. Use whenever designing, building, reviewing or redesigning any screen, flow or feature UI, in Claude Design or in code (Compose, KMP, web), even if the user doesn't mention UX, psychology or best practices. Covers how people think and decide (defaults, progress, trust, ownership, loss, comparison).
---

# UX Skills

This skill holds **judgment**: what makes a screen work for people, and why.
It never holds **values** (colors, sizes, spacing numbers, components).
Those come from the project's own design system.

- ux-skills says: "the main action must stand out"
- the design system says: "the main button is a green pill"

If a rule here seems to conflict with the project's design system,
follow the design system for how it looks, and this skill for what it does.

## How to use it on any screen or feature

1. Name what the user is trying to do on this screen (decide, enter data,
   track progress, act, compare).
2. Scan the index below. Pick the principles that genuinely fit.
   Usually 1 to 3. Never force all of them in.
3. Read only the files you picked. Each has a before/after example:
   use it to recognize the "before" in your own screen.
4. Apply them using the project's design system for visuals.
5. When you deliver, list which principles you applied and where,
   in one line each, so the work can be reviewed.

## Principle index

| Principle | Memory hook | Look for it when the screen... |
|---|---|---|
| [Smart defaults](principles/smart-defaults.md) | Defaults feel like recommendations | asks the user to choose or enter anything |
| [Head start](principles/head-start.md) | Zero feels like standing still | has steps, goals, completeness or a checklist |
| [Give first](principles/give-first.md) | A gift creates a debt | asks for an account, data, permission or payment |
| [Ownership](principles/ownership.md) | What I built or chose is mine | can be personalized, named or built by the user |
| [Loss framing](principles/loss-framing.md) | Losing hurts twice as much as gaining | asks the user to act, keep, turn on, or confirm a destructive step |
| [Contrast](principles/contrast.md) | The first number becomes the ruler | shows a price, amount, score or statistic |

The common thread: people don't decide logically. They react to what is
pre-chosen, what they already have, what they just saw, and how close
the finish line feels. Design for that, honestly.

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

- `rules/`: concrete screen rules (forms, lists, states, navigation, accessibility)
- `checklist.md`: final self-check before delivering a screen
