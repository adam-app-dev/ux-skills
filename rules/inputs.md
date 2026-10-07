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
When only one option can be picked, it behaves like a radio (choosing one
clears the other); when several can, like checkboxes. Make the
difference visible.
Example: sizes, flavors, plan lengths or categories as a row of chips.
When options need more context, use selectable cards with a label, a
short description and an icon, instead of a plain text list.
Note: long lists (countries, many categories) and settings still suit
a plain list, a searchable list or a dropdown. Cards are for short sets
of meaningful choices.
Sources: uxpeak, product page conversion redesign; uxpeak, top UI design tips part 2

## Long lists of options open with search
Why: scrolling a small dropdown of forty countries or currencies on a
phone is slow and error-prone; people know what they want and just
need to type a few letters.
Do: on phones, open a long list of options as a sheet or full screen
with a search field at the top, the most likely choices first (recent,
common, or detected), and the current choice marked. When several can
be picked, show how many are selected and offer "Clear".
Don't: squeeze a long list into a small scrolling dropdown, or make
people scroll the whole alphabet to reach their option.
Accessibility: the search field is focused when the sheet opens, and
the selected option is announced.
Source: How to Design Better UI Components 3.0 (book)

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

## Fields and controls have a visible edge
Why: a text field with a barely-there outline, or a button whose shape
fades into the background, makes people unsure what they can type into
or tap, especially low-vision users and anyone in bright light.
Do: give fields, checkboxes, switches and outlined buttons an edge or
fill that stands out from the background at 3:1 contrast or more (the
WCAG minimum for controls), and keep text inside them at 4.5:1.
Don't: rely on a very light outline or a faint fill as the only sign
that something is a field or a button.
Note: the source labels these minimums "WCAG 3.0"; they come from
WCAG 2.1 and 2.2 level AA.
Source: How to Design Better UI Components 3.0 (book)

## Mark the optional fields, not the required ones
Why: most fields in a good form are needed, so a row of red asterisks
adds noise and makes the form feel strict. Marking the few exceptions
is quieter and just as clear.
Do: ask only for what's needed, then mark the few optional fields with
the word "(optional)" next to the label.
Don't: put an asterisk on every field, or rely on a red dot that screen
readers and colorblind users may miss.
Accessibility: required fields are still marked as required for screen
readers (in Compose, via semantics), even when it isn't shown visually.
Source: How to Design Better UI Components 3.0 (book)

## Check each field as soon as it's done
Why: finding five errors only after tapping "Continue" means scrolling
back up and redoing work. Checking each field right after the user
finishes it lets them fix it while it's in mind.
Do: show the expected format before typing (helper text such as
"DD/MM/YYYY"), check a field when the user leaves it, and once a field
has shown an error, update it as they type so the error clears the
moment it's fixed. Confirm valid input quietly (a check mark).
Don't: show an error while the user is still typing the first time, or
check only on submit. Never use placeholder text as the field's only
label: it disappears on typing.
See also: states.md (an error says what happened and how to fix it).
Source: How to Design Better UI Components 3.0 (book)

## Long forms come in steps
Why: a single screen with twenty fields looks like a wall and invites
quitting. Steps let people focus on one group at a time and see how far
they've come.
Do: split long forms into a few steps of related fields, show the
current step and the total ("Step 2 of 4"), let people go back without
losing what they entered, and show a summary to review before the
final step.
Don't: split a short form into steps just for the effect, or show
progress that isn't real.
See also: head-start.md (count real progress), placement.md (show it,
don't make them remember it).
Source: How to Design Better UI Components 3.0 (book)

## Search helps while the user types
Why: people rarely know the exact word the app uses. A search box that
waits for a perfect query and then answers "nothing" makes them guess
again and again.
Do: when search is central to the app, put it where it's seen at once
(top of the main screen or its own tab). Use the placeholder for an
example of what can be searched ("Search recipes or ingredients"),
suggest matches as the user types, tolerate typos and plurals, and
offer a one-tap clear button.
Don't: hide a main search behind a menu, or make the user press
"Search" before seeing anything.
Accessibility: the field has a label, not just a placeholder; the
number of suggestions is announced as it changes.
See also: smart-defaults.md (empty search shows recent and popular),
states.md (no results).
Source: How to Design Better UI Components 3.0 (book)
