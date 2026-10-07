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

## A selection means what the action says
Why: when "checked" means the opposite of what the button does, users
must reverse the logic in their head, and some will get it wrong.
Do: make the checked items the ones the action applies to, and say it
plainly in the instruction and the button ("Select items to remove" →
"Remove 2 items").
Don't: write instructions with double negatives ("Unselect the items you
want to remove"), or make a checkbox mean "keep" on a screen whose button
removes.
Source: uxpeak, The UI/UX Playbook (book)

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

## Never ask for what you already know or can look up
Why: every field the user types costs time and invites typos. Much of
it is already known (saved details, their last entry) or can be looked
up (an address from a few letters).
Do: fill in what the app already has, offer search-as-you-type for
addresses and places, and let the phone's autofill work (in Compose,
give fields their content type, such as email or postal address).
Keep everything editable.
Don't: ask again for details the user gave earlier in the same flow,
or block the phone's autofill and password managers.
Note: saved payment or personal details are reused only with the
user's consent, and the user can remove them.
See also: smart-defaults.md.
Source: uxpeak, The UI/UX Playbook (book)

## Repeated actions can be done in bulk
Why: when users must apply the same action to many items (archive,
move, mark as done, delete), doing it one by one is slow and tedious.
Do: let users select several items and act on all of them at once,
with the count in the button ("Archive 12"). For actions that can't be
undone, confirm with the count.
Don't: make many-item tasks a long series of single taps when the app
could do them together.
See also: "A selection means what the action says" above.
Source: uxpeak, The UI/UX Playbook (book)

## The field's shape matches the data
Why: a field's size and form tell the user what goes in it before they
read the label. A long box for a three-digit code or a single box for a
six-digit code makes people unsure and invites mistakes.
Do: size each field for what it holds (short fields side by side for
expiry date and security code, a long one for a card number or
address), and show short codes as one box per character when that
makes the length clear.
Don't: give every field the same full width, or split a value into
boxes that behave like separate fields.
Accessibility: per-character code boxes act as one field: one label for
screen readers, paste works, backspace moves back, and the phone can
autofill the code from a message (in Compose, the one-time-code content
type). Short side-by-side fields stack when the text size is large.
Source: uxpeak, The UI/UX Playbook (book)

## Passwords: one field, with show and hide
Why: a "confirm password" field doubles the typing and still misses a
typo typed twice. Seeing the password is the better check. Requirements
discovered only after submitting feel like a trap.
Do: use one password field with a show/hide toggle, list the
requirements before the user types, and tick them off as they are met.
Let password managers fill and save it.
Don't: add a confirm-password field, or reveal the rules only in an
error after submitting.
Accessibility: the toggle is labeled ("Show password") and announces
its state; requirement checks and any strength meter are given in
words, not color alone.
Source: uxpeak, The UI/UX Playbook (book)
