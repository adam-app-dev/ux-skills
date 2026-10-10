# Choosing a view

**Memory hook:** the purpose picks the view.

Lists, grids, cards and the rest are just containers. Before picking one,
name what the user is trying to do with this content (scan, recognize,
compare, track, check, act, enter data). The purpose picks the view; the
look of each view comes from the design system.

## Start from the purpose, not from a favorite view
Why: the same content can be shown many ways, and each way makes one
task easy and others slow. A view chosen because it looks nice (cards
everywhere, a grid for text) makes users work around it.
Do: write down the main thing the user does with this content, then
pick the view from the rules below.
Don't: pick a view first and fit the content into it, or copy the view
of another screen whose purpose is different.
Source: platform guidelines (Material Design 3, Apple HIG)

## Scanning many similar items → a list
Why: a list puts items in one column with the same shape, so the eye
runs straight down and spots the one it wants.
Do: use a list when items are alike and told apart mainly by text
(a name, a date, an amount). Put the most telling detail first in each
row, and keep rows the same shape.
Don't: use a list when people pick items by how they look; they'd have
to read every row to find a picture they'd recognize instantly.
Example: messages, transactions, contacts, settings.
Source: platform guidelines (Material Design 3 lists; Apple HIG lists
and tables)

## Recognized by their picture → a grid
Why: when people know an item by its image, a grid shows many images
at once and lets the eye jump to the right one.
Do: use a grid when the picture is the main way to tell items apart.
Keep images in one visual style (see imagery.md), and give every item a
text name, at least for screen readers.
Don't: use a grid for items that are told apart by text or numbers;
cutting text into narrow tiles makes it harder to read. Don't use a
grid for a handful of items where a short row would do.
Example: photos, products, templates, albums.
Source: platform guidelines (Apple HIG collections; Material Design 3)

## Rich items with several details or actions → cards
Why: a card groups everything about one item (image, title, a few
details, its own actions) into one unit, so different-looking items
stay readable side by side.
Do: use cards when each item has several kinds of content or its own
actions, and items vary in what they contain. A card is either one big
tap target that opens the detail, or holds a few clear buttons, not
both fighting for the same tap.
Don't: wrap simple, alike items in cards; a list scans faster and takes
less space. Don't force content into cards when space, headings or
dividers would make the hierarchy simpler.
Example: plans to choose from, bookings, articles with a picture and
a summary.
Source: platform guidelines (Material Design 3 cards)

## Things that happen over time → a timeline
Why: when order in time is the point, the user's question is "what
happened, and what's next?". A timeline answers it by position, without
anyone reading the dates.
Do: order by time (newest first for activity; next first for what's
coming), group by day when there are many entries, and mark "now" or
the current step with more than color (see placement.md, steps).
Don't: use a timeline when time doesn't matter to the user; a list sorted
by what's most useful is easier.
Example: account activity, history of changes, order stages.
Note: neither platform guide names "timeline" as a view; this is common
practice built from their lists and progress indicators.
Source: platform guidelines (lists, progress indicators); common practice

## "How am I doing?" → a summary on top, details below
Why: a person checking their state wants the answer first, then the
evidence. A long list of entries makes them add it all up themselves.
Do: lead with the one or two numbers that answer the question (a total,
a trend, what's left), each with an honest reference (see contrast.md),
then the entries that make it up.
Don't: open with the raw list, or fill the top with so many numbers
that none of them is the answer.
Example: monthly spending total and its change from last month, then
the transactions; a goal's progress, then the logged entries.
Note: this is common practice, not a named view in the platform guides.
See also: hierarchy.md (value louder than label), where-they-are.md.
Source: common practice, in line with platform guidelines

## One item in depth → a detail screen
Why: when the user has picked one item, they want everything about it
and what they can do with it, without other items competing.
Do: open a detail screen from the list, grid or card, lead with the key
information and the main action (see placement.md), and keep the item's
title visible while scrolling.
Don't: cram full details into the list rows, or make users open a
detail screen just to see the one value they need every time.
Example: a profile, an order, a saved item.
Source: platform guidelines (Material Design 3, Apple HIG)

## Entering data → a form
Why: a form lets people enter several values in order and check them
before saving.
Do: keep it short, ask only what's needed, group related fields, label
every field, pre-fill what you can (see smart-defaults.md) and pick each
input by how it's used (see inputs.md).
Don't: hide entry inside a list of tappable rows that each open their
own screen, when a few fields on one screen would do.
Example: adding an entry, editing a profile, a settings group.
Source: platform guidelines (Material Design 3 text fields; Apple HIG)

## Creating something others will see → a form shaped like the result
Why: a plain column of fields hides what the user is actually making.
When the form looks like the finished thing, they understand each field's
role at once and see their creation take shape as they fill it in.
Do: when the user creates something that will be displayed (a listing,
a profile, a post, an event), lay the form out like the final result:
the photo slot where the photo will be, name and price where they'll
appear. Keep a visible label on every field.
Don't: rely on placeholder text as the only label, or let the visual
arrangement scramble the order fields are filled in.
Accessibility: screen readers and the keyboard move through the fields
in reading order, and an empty photo slot is announced as a button
("Add photo").
See also: ownership.md (what I built is mine), "Entering data → a form"
above.
Source: uxpeak, The UI/UX Playbook (book)

## When dates matter most → a calendar
Why: when the user plans around days ("what's on Friday?", "is the 12th
free?"), a calendar shows the shape of the week or month at a glance.
Do: use a calendar when picking or seeing days is the main task, and
always offer a list of the same entries (an agenda) next to it or one
tap away. Screen readers read each day with its entries ("Friday 12,
2 events").
Don't: use a calendar when the date is just one detail of each item; a
list grouped by day reads more easily.
Example: bookings, appointments, availability.
Source: platform guidelines (Material Design 3 date pickers; Apple HIG
date pickers)

## When places matter most → a map
Why: when the user chooses by where something is ("what's near me?"),
a map shows distance and grouping that no list can.
Do: use a map when location drives the choice, and always pair it with
a list of the same items (sorted by distance), which screen reader users
rely on. Keep the map and the list in sync when one is filtered.
Don't: use a map just to show one address; a line of text with an "Open
in Maps" button is enough.
Example: nearby stores, places to visit, delivery areas.
Source: platform guidelines (Apple HIG maps)

## When no view is right for everyone, let people switch
Why: some content serves two purposes equally. Large photo cards make
people want something; a compact list lets them compare quickly. Some
people prefer one, some the other, and picking for everyone fails half
of them.
Do: when two views genuinely serve different users, offer a simple
switch between them (for example cards and a compact list) near the
results, and remember the choice.
Don't: add a switch to avoid deciding: when one view clearly fits the
purpose, use it. Don't reset the user's choice every visit.
Accessibility: the switch has a label and announces the current view
("View: compact list").
Source: uxpeak, junior vs senior vs staff redesigns (food list, filters)

## For a new screen, propose 2-3 views and wait
Why: the right view depends on what the user values most, which only
they know. Picking one silently hides a real choice, and reaching for
the components that already exist repeats the same few layouts on every
screen.
Do: for a new screen, or whenever the user is unsure, propose two or
three clearly different views (not three versions of the same list),
with one line each on why it fits the purpose, recommend one, and wait
for the user to choose. Include at least one view the app doesn't use
yet when the purpose allows it.
Don't: build one view and present it as the only option, offer a long
menu of every possible view, or limit the options to the components the
design system already has.
Example: for a screen of saved items: a list (fastest to scan by name),
a grid (best if people know items by their picture), or cards (best if
each item has its own actions). Recommendation: grid, if every item has
a photo.
See also: SKILL.md (explore before you build).
Source: this repo's own working rule
