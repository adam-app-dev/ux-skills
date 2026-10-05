# States

**Memory hook:** the screen still works when there's nothing to show.

A screen isn't only its filled-in version. The core rule in SKILL.md
lists the states every screen meets: empty, loading, error, offline.
Illustration style and colors come from the design system.
These rules say what each state must do.

## An empty screen shows the way forward
Why: a screen that only says "No items" is a dead end. The user doesn't
know what belongs there, why it matters, or what to do next, and a new
user may decide the app isn't for them.
Do: give every empty screen three things:
- what will appear here and why it's useful ("Keep all your projects in
  one place"),
- optionally one or two short tips for getting the most out of it,
- one clear button to create the first item ("Create project").
A light illustration can make it feel less bare.
Don't: show only "Nothing here", add several competing buttons, or
fill the space with a long tutorial.
Example: an empty list of saved items says what saving is for and offers
one button to find something to save.
Accessibility: a decorative illustration is hidden from screen readers,
and it must not push the button below the fold on small phones.
See also: where-they-are.md (newcomers see empty states most).
Source: uxpeak, top UI design tips part 2
