# Contrast (anchoring)

**Memory hook:** the first number becomes the ruler.

## The idea
The brain judges every piece of information relative to what it saw just
before. The same price can feel expensive or like nothing, depending on
context. A number shown alone invites a harsh evaluation; next to a
reference it gets measured against that reference. So control what the
user sees first.

## Why it works
People evaluate relatively, not absolutely. Shown alone, "$50/month"
makes people do the scary math in their head ("that's $600 a year") and
decline. Shown right after a $1,900 item, the same $50 barely registers.
Restaurants put a $90 steak on the menu not to sell it, but so the $40
dish looks reasonable.

## Before / after
- **Before:** a protection plan on its own page: "$50/month". The user
  annualizes it, thinks "too much", taps "No thanks".
- **After:** the same plan shown directly below the $1,900 laptop the user
  just added, with a small label: "just 2.6% of your laptop".
  Nothing changed about the offer; everything changed about how it feels.

## Techniques
- **Pair a number with a reference** shown first or right beside it.
- **Express a cost as a share** of the bigger thing it relates to ("2.6% of…").
- **Place the decision in context:** offer an add-on next to the main item,
  not on a separate screen.

## Where it applies
- **Amounts and spending:** "this month vs last month", "vs your average".
- **Scores and stats:** show the previous value or a normal range next to the current one.
- **Prices and add-ons:** show a cost relative to what it protects or belongs to.
- **Plans:** show options side by side so differences are clear, with
  each option's terms (savings, cancellation) inside its own card.
- **Progress:** "3 km today, 1 km more than yesterday".

## Do
- Pair every important number with one honest reference.
- Decide deliberately which number the user sees first.

## Don't
- Show a cost or number in isolation when a comparison would explain it.
- Stack so many comparisons that the main number gets lost.
- Use a comparison badge ("Cheaper", "Best value") that isn't true
  against the options actually on screen.
- Rely on color alone (a green badge) to say "this is the good one".
  Use words, and check the badge text still meets the 4.5:1 contrast
  minimum.

## Guardrail
References must be real and relevant. No inflated "original prices",
no decoy options that exist only to mislead.
- **Crossed-out prices:** show an old price only if it was really
  charged. In the EU, the "before" price must be the lowest price of the
  last 30 days.
- **Screen readers:** a strikethrough is usually not announced, so a bare
  "€129 €89" is read as two prices. Give it an accessible label
  ("was €129, now €89"; in Compose, via semantics).
- **Plan cards (one-time vs subscription):** both options look equally
  choosable, and neither paid recurring option is pre-selected. If
  something must be selected, pick the one-time option.
- **Selected card:** mark it with a check or radio mark, not a tint alone.
Note: the product page conversion source pre-selects the subscription
and gives it a "Most popular" tag. This repo never pre-selects a
recurring payment, and labels popularity only when it's real
(see social-proof.md).
Note: the third source shows a crossed-out price and a "−31%" badge as a
pure win. This repo keeps the idea only when the old price is real.

Sources: uxpeak, "Six Psychology Principles That Transform UX Design";
uxpeak, three A/B test examples;
uxpeak, product page conversion redesign (see sources.md)
