# Inputs

**Memory hook:** match the input to how often and how exactly.

The look of fields, wheels, sliders and steppers comes from the design
system. These rules say which one to use, and when.

## Pick the input by how it will be used, not by how it looks
Why: the same kind of value (a number) can be entered once in a lifetime
or ten times a day. A control that feels pleasant once becomes slow and
fiddly when repeated, and an imprecise control frustrates anyone who
needs an exact value.
Do:
- **One-time, approximate values** with a known range (age, height,
  a rough goal at setup): a scroll wheel or slider is quick and needs no
  typing.
- **Frequent or exact values** (amounts, quantities, daily entries):
  a number field, a stepper, or quick picks plus a field
  (see smart-defaults.md).
Don't: choose a wheel or slider for an entry the user makes often, or
for a value that must be exact.
Example: setting your height at sign-up with a wheel is fine; entering
an exact amount every day with a slider is not.
Source: uxpeak, five advanced UX/UI tips

## Every value can also be typed
Why: wheels and sliders are hard for screen reader users and for people
with less steady hands, and dragging to an exact value is slow for
everyone.
Do: let the user tap the value to type it, and give wheels and sliders a
clear accessible label and value ("Height, 175 centimeters"; in Compose,
via semantics).
Don't: make a wheel or slider the only way to enter a value.
Source: uxpeak, five advanced UX/UI tips

## Number fields open the right keyboard and accept local formats
Why: a full letter keyboard for a number wastes taps, and rejecting
"2,5" where people write decimals with a comma feels broken.
Do: open the numeric keyboard (with a decimal key when decimals are
allowed), and accept the user's local decimal separator.
Don't: force a dot as the only decimal separator, or show an error for
a valid local format.
Source: uxpeak, five advanced UX/UI tips

## A few options are shown, not hidden in a dropdown
Why: a dropdown makes users tap, open and read just to find out what
the choices are. With only a handful of options, that work is wasted.
Do: show a small set of options (roughly up to six) as visible chips,
swatches or cards, each with a text name. Mark the selected one with
more than color (a check, a border, bold text).
Don't: hide two or three choices in a dropdown, or use color or icon
swatches without a name (screen readers and colorblind users need it).
Example: sizes, flavors, plan lengths or categories as a row of chips.
When options need more context, use selectable cards with a label, a
short description and an icon, instead of a plain text list.
Note: long lists (countries, many categories) and settings still suit
a plain list, a searchable list or a dropdown. Cards are for short sets
of meaningful choices.
Sources: uxpeak, product page conversion redesign; uxpeak, top UI design tips part 2

## The chosen option explains itself
Why: at the moment of choosing, people hesitate over "what will this be
like?". A short answer right there removes the doubt.
Do: when an option is selected, show one short line about it under the
options ("Light and tart, not too sweet", "Best for daily use").
Don't: hide this information behind hover (phones have none) or in a
separate details screen.
Note: the source shows the description as a hover tooltip, which only
works with a mouse. This repo shows it on selection instead.
Source: uxpeak, product page conversion redesign

## Follow-up options appear only when they apply
Why: showing every possible option at once makes the first view heavy;
most users never need some of them.
Do: reveal extra options right after the choice that makes them
relevant (choose "one-time" → see bundle sizes), and keep the first
view simple.
Don't: pre-select an upsell inside the revealed options, or hide
something the user needs to decide correctly.
Source: uxpeak, product page conversion redesign
