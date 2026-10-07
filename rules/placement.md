# Placement

**Memory hook:** put it where the user needs it.

Good UI is not just arranging elements. It's placing information at the
moment and spot where the user needs it to decide or act.

## Key information comes early
Why: users want to know quickly what something is, how good it is and
what it costs (or what it means for them).
Do: show the essentials (what, how trusted, how much / how urgent)
near the top, before details.
Don't: push a deciding piece of information (like the price) far down
the screen.
Source: uxpeak, product page redesign

## Each screen shows what its task needs, no more and no less
Why: every extra button, figure or line competes with the task the user
came for. But cutting too far is just as bad: a screen without the facts
needed to act leaves the user guessing.
Do: name the screen's task (pay, check today, change a setting), keep
what helps with it, and move everything else to where it's relevant
(a detail screen, settings, "See all").
Don't: fill a task screen with details that belong elsewhere (view
counts, full specifications, unrelated suggestions), or remove what the
user needs to decide.
Example: a basket shows each item's name, chosen options, quantity,
price and the total; how many people viewed the item stays on the item's
own page.
Note: the source treats a return-policy note in a basket as clutter.
This repo keeps the terms the user is agreeing to (total, fees,
cancellation) next to the pay step: they are part of the task (see
show-the-catch.md).
Source: uxpeak, The UI/UX Playbook (book)

## Trust information sits next to what it confirms
Why: ratings and reviews are among the strongest trust signals. Users
ask "what is it?" and "can I trust it?" in the same moment.
Do: place the rating or trust signal right next to the title it refers to.
Don't: separate trust signals from the thing they validate.
Source: uxpeak, product page redesign

## Things used together sit together
Why: users act in sequences. Choose amount, then add to cart. Pick a date,
then confirm. Splitting those controls makes users hunt.
Do: place controls that are used one after another side by side.
Add units inside controls where they apply ("1 kg", "2 doses").
Don't: place a selector far from the button that uses its value.
Source: uxpeak, product page redesign

## Inside an item, follow the order people decide in
Why: the same elements read very differently depending on their order.
A card that opens with the price, or puts the button before the
description, asks the user to judge or act before they know what it is.
Do: inside a card or item block, go from recognizing it (image, name),
to understanding it (one short detail), to its cost or key value, and
end with the action. The button comes after the information it acts on.
Don't: lead with the price or the button, or put the description below
the button where it's read after the decision.
Note: this is the order inside one compact item, where everything is
visible at once. On a long screen, "Key information comes early" still
applies: the price must not be pushed far down.
Source: uxpeak, The UI/UX Playbook (book)

## Fixed text never holds a changeable value
Why: if a title says "1 kg" but the user can change the quantity, the
title becomes wrong.
Do: titles describe the thing itself; values the user can change live in
the controls that change them.
Don't: put a variable value (quantity, size, date) in a fixed label.
Source: uxpeak, product page redesign

## Drop labels the content already explains, consistently
Why: a currency symbol already says "price"; a label saying "Price" adds
noise.
Do: remove redundant visible labels, and apply the same decision to
similar elements (if you label one value, label its neighbors too).
Don't: remove the meaning for screen readers. The visible label can go,
but keep an accessible label (in Compose: a contentDescription or
semantics) so blind users don't just hear a bare number.
Source: uxpeak, product page redesign

## Keep context while scrolling
Why: on long screens, users lose track of what they're looking at.
Do: when the main image or header scrolls away, keep the title visible
(for example, it moves into the top bar and stays there).
Don't: let users scroll into details with no reminder of what they're on.
Source: uxpeak, product page redesign

## The main action stays reachable
Why: people don't always decide at the top. They read, scroll, compare,
and decide later.
Do: on long screens, keep the main action (and the control it needs) in
a sticky bottom area.
Don't: make users scroll back up to act once they're ready.
Source: uxpeak, product page redesign

## Status screens open with the answer
Why: after a user commits (pays, sends, books, applies), they wait with
one question: "is it going OK?". A screen of raw data makes them dig for
the answer and adds worry.
Do: lead with a plain status line ("On the way", "Approved",
"Being reviewed"), then the key details (when, where, what's next).
Don't: open with reference numbers, item lists or a log of dates.
Example: an order, a request or an application screen starts with its
status and expected time, and the reference number sits further down.
Source: uxpeak, five advanced UX/UI tips

## A process with stages is shown as steps
Why: a list of dates makes users work out where things stand; a row of
steps shows it at a glance.
Do: show the stages as a timeline with done, current and upcoming steps,
the current one marked by more than color (filled shape, label, bold
text). Screen readers announce it ("Step 3 of 4, out for delivery").
Don't: show progress only as timestamps, or mark the current step with
color alone.
Source: uxpeak, five advanced UX/UI tips

## When a person handles the request, show who and how to reach them
Why: a name (or photo) and a one-tap way to get in touch make waiting
feel personal and safe, instead of anonymous.
Do: show who is handling it (a courier, a support agent, a host) with
quick actions to call or message, placed with the status they relate to.
Don't: hide contact options in a help menu while the user is waiting
on that person.
Note: show a worker's photo only with their consent; a name is enough.
Source: uxpeak, five advanced UX/UI tips

## Show the content, not a door to it
Why: every tap before the user sees something useful is a cost, and new
users are the least willing to pay it. A banner that promises content
("Discover 100+ items") adds a step between the user and the value.
Do: put a few real items on the screen right away (the top picks, the
most relevant entries), with a "See all" link for the rest.
Don't: replace content with a banner or button that only leads to it.
Example: a home screen shows the top 10 recommended items in a row,
instead of a banner announcing that recommendations exist.
See also: give-first.md (value before asking).
Source: uxpeak, top UI design tips part 2

## Frequent actions sit within thumb reach
Why: phones are often used one-handed. Controls in the top corners make
users stretch or change grip, which is slow, and harder still for people
with limited mobility.
Do: place the main and most-used actions in the lower, central part of
the screen, where the thumb naturally rests (sticky bottom buttons,
bottom bars).
Don't: put the main action in a top corner on phone screens. Keep
destructive actions (delete, sign out) out of the easiest spot, so they
aren't tapped by accident.
Note: this applies to phones. On tablets and desktop windows, follow
navigation.md (wide screens).
See also: "The main action stays reachable" above.
Source: uxpeak, top UI design tips part 2
