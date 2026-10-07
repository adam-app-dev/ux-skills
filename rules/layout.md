# Layout

**Memory hook:** one grid, meaningful space.

The actual margin and spacing values come from the design system's
spacing tokens. These rules say how to use them.

## Everything follows one grid
Why: when elements sit slightly off (some a bit further left, some a bit
further right), users don't consciously notice, but they feel it.
The screen feels less calm and less trustworthy.
Do: use the same side margins for all content on a screen, and align text,
icons, prices and buttons to the same edges.
Don't: let individual elements drift a few pixels from the shared edge,
or mix start and center alignment inside one card or one group of
similar items.
Example: if content starts at the standard screen margin, every section
starts there too, not just the first one.
Sources: uxpeak, product page redesign; uxpeak, The UI/UX Playbook (book)

## Space shows what belongs together
Why: the gap between elements tells users which things are related.
Related items close together, unrelated items further apart.
Do: use smaller gaps inside a group and larger gaps between groups,
consistently, from the spacing scale.
Don't: add space just because white space looks "premium". Too much space
in the wrong place disconnects things that belong together and makes the
screen harder to scan.
Example: in a form, each label sits clearly closer to its own field than
to the field above it; with equal gaps, users can't tell which field a
label belongs to.
Sources: uxpeak, product page redesign; uxpeak, The UI/UX Playbook (book)

## Spacing is consistent across the screen
Why: inconsistent gaps make a layout feel accidental.
Do: reuse the same spacing value for the same relationship
(e.g. every section gap is the same token).
Don't: pick a slightly different gap for each section.
Source: uxpeak, product page redesign

## Content stays inside the safe area
Why: modern phones have a home swipe bar, rounded corners and camera
cut-outs. Controls placed under them are hard to tap, and a tap near the
home bar can send the user out of the app by accident.
Do: keep bars, sticky buttons and other controls inside the device's
safe area, above the home bar (in Compose: respect the window insets,
for example through Scaffold).
Don't: hide the home bar, overlap it, or squeeze controls against it.
Source: uxpeak, bottom navigation guide

## Tap areas are bigger than what they show
Why: a small icon is fine to look at but hard to hit with a thumb,
especially for people with less precise hands. Too-small targets cause
mis-taps and frustration.
Do: give every tappable element a touch area at least the platform
minimum (iOS: 44pt; Android: 48dp), even when the visible icon is
smaller. Keep enough space between targets that neighbors aren't hit
by mistake.
Don't: make the touch area the same size as a small icon.
Source: uxpeak, bottom navigation guide

## Check it on a real phone
Why: a screen that looks right on a big monitor can feel cramped,
tiny or hard to reach in the hand.
Do: try the design on a real device, held in one hand, on a small and a
large phone.
Don't: approve tap sizes and spacing only from a desktop preview.
Source: uxpeak, bottom navigation guide
