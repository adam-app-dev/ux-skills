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
Source: Five advanced UX/UI tips (YouTube)

## Every value can also be typed
Why: wheels and sliders are hard for screen reader users and for people
with less steady hands, and dragging to an exact value is slow for
everyone.
Do: let the user tap the value to type it, and give wheels and sliders a
clear accessible label and value ("Height, 175 centimeters"; in Compose,
via semantics).
Don't: make a wheel or slider the only way to enter a value.
Source: Five advanced UX/UI tips (YouTube)

## Number fields open the right keyboard and accept local formats
Why: a full letter keyboard for a number wastes taps, and rejecting
"2,5" where people write decimals with a comma feels broken.
Do: open the numeric keyboard (with a decimal key when decimals are
allowed), and accept the user's local decimal separator.
Don't: force a dot as the only decimal separator, or show an error for
a valid local format.
Source: Five advanced UX/UI tips (YouTube)
