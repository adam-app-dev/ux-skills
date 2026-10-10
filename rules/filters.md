# Filters

**Memory hook:** filters help people explore, not just fill in a form.

Filters and sort turn a huge set (hundreds of items, places, products,
jobs) into the few worth looking at. The look of chips, sheets, sliders
and buttons comes from the design system. These rules say what filters
must do.

## Filters are for exploring trade-offs, not only for collecting values
Why: people rarely arrive with fixed requirements. "Three rooms" often
means "three, unless two gives me much better options". A filter that
just asks for values and hides everything else makes them guess, apply,
look, and start over.
Do: design filters so people can see the effect of loosening or
tightening each choice while they make it (the rules below show how).
Treat every requirement as something the user may still change.
Don't: treat the filter as a form to complete once, with the results
only revealed at the end.
Example: someone looking for a place with a budget and a minimum number
of rooms finds that a slightly higher budget opens up many more options,
and adjusts before applying.
Source: uxpeak, junior vs senior vs staff redesigns (food list, filters)

## The common filters are visible, the rest one tap away
Why: filters hidden inside dropdowns are filters nobody knows exist.
People can't use an option they never see.
Do: above the results, show the most-used filters as tappable chips,
next to a "Filters" button that opens the full set and a sort button
beside it. Show how many results the list holds ("640 places") and
update the number when filters change. When filters are active, show
how many on the "Filters" button.
Don't: hide all filters and sort options in dropdowns, or show results
with no idea of how many there are.
Accessibility: each chip announces its name and whether it's on, and
the result count is announced when it changes.
See also: inputs.md (a few options are shown, not hidden), choosing-a-view.md
(let people switch views).
Source: uxpeak, junior vs senior vs staff redesigns (food list, filters)

## All filters on one screen, over the results
Why: filter choices are connected: the budget depends on the size, the
size on the area. One page per filter means choosing each value without
seeing the others, and many more taps. Replacing the results with a
full screen also makes people forget what they were filtering.
Do: put all filters in one scrolling sheet that opens over the results,
so the list is still hinted behind it. Group related filters with clear
headings.
Don't: send each filter to its own page, or make people go back and
forth to change two values.
Note: a sheet with many filters needs a clear way out (close, the back
gesture) and a "Clear all" (see placement.md, dialogs).
Source: uxpeak, junior vs senior vs staff redesigns (food list, filters)

## The apply button shows the live count
Why: "Show results" hides the answer to the one question that matters:
did I narrow it too much or not enough? People find out only after
tapping, then have to come back.
Do: label the button with the number of results the current choices
return ("Show 41 homes"), and update it as each filter changes. When a
choice would leave zero results, say so before the user applies it.
Don't: use a generic "Apply" or "Show results" when the count is known.
Accessibility: the new count is announced as filters change.
See also: smart-defaults.md (buttons state the result).
Source: uxpeak, junior vs senior vs staff redesigns (food list, filters)

## Options match how people think
Why: when someone asks for three rooms, they usually mean "at least
three". If choosing "3" quietly removes every four-room option, the
filter throws away exactly what they'd want.
Do: for counts (rooms, seats, stars), offer the options as visible
chips that mean "at least" ("1+", "2+", "3+"). Offer an exact match
separately when it's genuinely useful, and when people may want a
range, let them tap two options to select everything between them.
Don't: make people tap a stepper up to a value they already know, or
make a minimum act as an exact match.
Accessibility: chips announce their full meaning ("3 or more rooms"),
and a selected range is announced ("2 to 4 rooms").
See also: inputs.md (pick the input by how it will be used).
Source: uxpeak, junior vs senior vs staff redesigns (food list, filters)

## Show what each choice leaves before it's chosen
Why: without counts, filtering is trial and error: choose, see what
happened, go back, try again. A count on each option shows the cost of
being stricter up front.
Do: next to each option, show how many results it would leave, given
the other filters already set ("3+ · 459", "4+ · 229").
Don't: show counts that ignore the other active filters, or counts that
are stale.
Accessibility: the count is part of each option's label ("4 or more
rooms, 229 results").
Source: uxpeak, junior vs senior vs staff redesigns (food list, filters)

## Show where the options are
Why: a price range of two numbers says nothing about the market. People
can't tell whether they're near the edge, or whether a small stretch
would open up many more options.
Do: for a range (price, size, distance), show how the options are
spread along it, for example small bars behind the slider showing how
many items fall at each price. Add a line of context: how many items
match the current filters out of the total ("459 of 1,557"), and a
typical value when useful.
Don't: show a bare slider when you know the distribution, or a chart
so detailed it takes longer to read than to try.
Accessibility: the chart has a text summary for screen readers ("Most
options between 650 and 750 thousand"), and slider handles have
full-size tap areas (see layout.md) and can be typed (see inputs.md).
Source: uxpeak, junior vs senior vs staff redesigns (food list, filters)

## Every extra piece of context earns its place
Why: counts, charts and helpers make each decision easier, but each
one also makes the sheet busier. Past a point, the screen is harder to
use than plain filters.
Do: for each piece of context, ask whether it changes a decision the
user makes here. Keep it if it does, drop it if it only looks clever.
Start with the count on the button, then add more where people often
hesitate.
Don't: add every possible helper to every filter.
See also: placement.md (what the task needs, no more and no less).
Source: uxpeak, junior vs senior vs staff redesigns (food list, filters)
