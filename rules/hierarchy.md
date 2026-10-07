# Hierarchy

**Memory hook:** clear, never shouting.

Colors, weights and sizes come from the design system.
These rules say how much attention each element should get.

## Rank the information before designing it
Why: when every piece of information is shown the same way (a column of
"label: value" pairs), users must read everything to find what matters.
The screen is tidy but flat.
Do: before designing, list what the screen shows and rank it by how much
the user needs it. Then give the top items more size, weight, color or
an icon, and let the rest step back.
Don't: format every field identically because they're all "data".
Example: a profile or account screen leads with the name and the one or
two values people check most, styled larger; secondary details follow
in a quieter style.
Source: uxpeak, five UX/UI design tips (Playbook)

## The value is louder than its label
Why: on a number or a stat, the user came for the value. A big label
("Sales") and a small number makes them hunt for what they wanted.
Do: make the value the strongest text, and the label smaller and softer.
Don't: give labels equal or greater weight than the values they name.
Example: a summary card shows "591" large and "Sales" small beneath or
above it; the same goes for balances, totals, scores and counts.
Accessibility: softer labels still meet 4.5:1 contrast
(see typography.md).
Source: uxpeak, five UX/UI design tips (Playbook)

## Few things compete for attention
Why: when many elements are bright, saturated or bold, nothing stands
out, the screen gets harder to read and the hierarchy collapses.
Do: decide what matters most on the screen and let only that be strong.
Use color to support the content, not to decorate.
Don't: use bright or saturated color on many elements at once.
Source: uxpeak, product page redesign

## Color is intentional
Why: color sets the mood and directs the eye. Random colors confuse both.
Do: use several colors only when each has a job (status, category, action).
Keep the palette calm enough that the content stays the focus.
Don't: give every icon or badge its own color "to make it lively".
Source: uxpeak, product page redesign

## Colored labels stay readable
Why: status tags and chips (Blocked, In progress, Paid) are often white
text on a bright fill. That looks lively but usually fails contrast, so
the one word that matters becomes hard to read.
Do: give a tag a soft tint of its color as background and a dark shade
of the same color as text, and check it meets 4.5:1. Keep each color to
one meaning across the whole app (green always means done or good), and
let the word carry the meaning, so color is never the only signal.
Don't: put white text on light or saturated fills without checking, or
reuse a status color for a different status.
See also: typography.md (badges are scannable).
Source: uxpeak, The UI/UX Playbook (book)

## The title stands out without shouting
Why: the title tells users what they're looking at, so it must be easy to
find and scan, but an overly heavy title unbalances the screen.
Do: make the title the clearest text on the screen, balanced with the
rest of the layout.
Don't: make it so bold or large that it dominates everything else.
Source: uxpeak, product page redesign

## The main action is clear but calm
Why: the main button should be the most important action on the screen,
but an aggressive button (huge, all caps) feels pushy.
Do: one primary button, clearly the strongest action, in normal case.
Don't: use all caps or oversized buttons to force attention.
Source: uxpeak, product page redesign

## Every action has a rank
Why: when several buttons look alike, users stop to work out which one
moves them forward. Giving each button its own color doesn't solve it:
three bright buttons are still three equal buttons.
Do: list the actions on the screen and give each a level. The main
action is the strongest. Secondary actions stay visible but quieter
(for example a neutral fill or an outline). Actions on single items and
destructive ones (remove, delete) are the quietest, often just text.
Rank them by style, fill and weight, not by color alone. The same rank
looks the same everywhere: the main button is identical on every card
and every screen.
Don't: show every action as the same full button, tell them apart only
by color, or re-color buttons to match each card's image or content.
Example: a basket with "Remove" on each item, "Continue shopping" and
"Pay": "Pay" is the strong button, "Continue shopping" a quiet one,
"Remove" a small text action on each row.
Accessibility: a quiet action still gets a full-size tap area (see
layout.md) and text that meets 4.5:1 contrast. A quiet delete needs an
undo or a confirmation that names what goes (see loss-framing.md).
Source: uxpeak, The UI/UX Playbook (book)

## Icons share one visual style
Why: mixed icon styles (some filled, some outlined, some heavy, some
light, many colors) make a section feel messy and pull too much attention.
Do: use one style (all outlined or all filled), similar weight, similar
level of detail, limited colors.
Don't: mix icon sets or styles on the same screen.
Exception: a selected state may switch one icon from outlined to filled
(for example the current tab, see navigation.md). That change is the
signal, not a mismatch.
Sources: uxpeak, product page redesign; uxpeak, bottom navigation guide

## Icons are the familiar ones
Why: an icon only saves time if people recognize it at a glance. An
unusual or artistic icon makes users stop and guess.
Do: use the symbol people already know for that function (a magnifying
glass for search, a house for home, a bell for notifications), drawn
simply.
Don't: invent a creative alternative (binoculars for search) or use a
detailed illustration as an icon.
Source: uxpeak, bottom navigation guide

## Icons come with a name
Why: an icon alone looks clean but makes users guess. A row of icon-only
switches or tiles can mean many things, and a wrong guess turns
something on or off by mistake.
Do: give every icon that sits next to a control (a switch, a tile, a
setting, a filter) a short visible text name. Icon-only is fine only for
a few universal symbols in top bars (back, search, close), and those
still get an accessible label.
Don't: strip names to make a screen look simpler. Too little
information is as unclear as too much.
Accessibility: a switch is read with its name and state ("Lights, off";
in Compose, via semantics), and "on" is shown by more than color.
See also: navigation.md (every tab has a label).
Source: uxpeak, The UI/UX Playbook (book)

## Separators and depth stay subtle
Why: dividers and shadows exist to separate, not to be noticed. Heavy
dark lines or harsh shadows chop the screen into blocks and make it look
unfinished.
Do: use light, thin dividers, soft shadows, or space alone, to separate
sections and lift cards.
Don't: use strong, dark divider lines or hard, dark shadows.
Accessibility: a soft shadow can vanish for low-vision users and in dark
mode. When a card's edge matters (it's tappable, it groups content), back
the shadow with a light outline or a slightly different background.
Small details like this are often what makes an interface feel premium.
Sources: uxpeak, product page redesign; uxpeak, five UX/UI design tips (Playbook)
