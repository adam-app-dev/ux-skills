# Smart defaults

**Memory hook:** defaults feel like recommendations.

## The idea
Every empty field is a decision. Stack too many decisions at once and people
make no decision at all: they leave (decision fatigue). Pre-fill each choice
with what most people, or this user, would pick. The user's job changes from
"fill this out from scratch" to "scan and adjust what doesn't fit",
which is a much easier task.

## Why it works
- **More choice = harder, not better.** Classic story: a store showing
  24 jam flavors sold far fewer jars than one showing 6.
  (Treat this as an illustration: later studies found the effect
  real but not always that strong.)
- **People trust defaults.** Most users never change a default value.
  That's not laziness; they read it as "this is what most people pick".

## Before / after
- **Before:** a booking screen with five empty fields and a button that says "Search".
- **After:** the same five fields pre-filled with the most common choices,
  and the button says "See 12 results", so the user knows the outcome before tapping.
- **Before:** a quantity stepper the user must tap many times, and an
  "Add to cart" button that hides the cost.
- **After:** one-tap quick picks (500 g / 1 kg / 2 kg) based on what most
  people actually buy, the stepper still there for custom amounts, and the
  button shows the total ("Add to cart · €8.40"), so there's no uncertainty
  before tapping.
- **Before:** tapping the search bar opens a blank screen. Only users who
  already know the exact word get anywhere.
- **After:** the empty search screen shows the user's recent searches,
  a few genuinely popular items and, if the user agreed, personal
  suggestions. Anyone who knows what they want just types.

## Where it applies
- **Data entry:** a date field defaults to today; an amount to the last amount used.
- **Repeated actions:** a new entry pre-picks the category or option used last time.
- **Common values:** offer the most common choices as one-tap options
  (chips), based on real usage data, and keep a custom option for everyone else.
- **Settings:** reminders start on, at a sensible time, instead of a blank picker.
- **Search and filters:** start with the most useful filter applied, not an empty state.
- **Empty search:** before the user types, show recent searches and
  popular picks, never a blank screen.
- **Buttons:** state the result of the action ("See 12 results",
  "Pay €8.40"), not just "Search" or "Pay".

## Do
- Pre-select the most common or most recent choice for every field.
- Keep every default visible and one tap to change.

## Don't
- Show a form where every field starts empty when you already know the likely answer.
- Hide a default the user can't easily see or change.
- Replace free input entirely with quick picks; always keep a custom option.
- Keep recent searches with no way to clear them.

## Guardrail
A default must serve the user. Never pre-select paid extras,
data sharing or marketing consent.
"Popular" suggestions must reflect real use, never paid placements
dressed up as popular.

Sources: uxpeak, "Six Psychology Principles That Transform UX Design";
uxpeak, product page redesign;
uxpeak, five advanced UX/UI tips (see sources.md)
