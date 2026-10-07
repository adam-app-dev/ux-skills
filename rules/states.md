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

## Loading shows something right away
Why: a blank screen while content loads looks like a broken app. Showing
something at once tells the user it's working and how long to expect.
Do:
- **Content screens:** show placeholder shapes in the layout of the real
  content (rows, cards, images), and replace them as content arrives.
  Show anything already known (the title, saved data) immediately.
- **Short actions** (saving, sending): an indicator on or near the
  button the user tapped, and keep the rest of the screen usable.
- **Long tasks** (uploads, imports): a progress bar with the real
  amount done when it's known; a looping indicator when it isn't.
  Let people do other things while they wait.
Don't: block the whole screen with a spinner for a short wait, or show
a percentage that isn't the real progress.
Accessibility: screen readers announce that content is loading and when
it's ready. Placeholder shimmer respects the "reduce motion" setting.
Note: an invented percentage bar or a slowed-down fake "analyzing" step
breaks the honesty guardrails in SKILL.md. This repo shows only real
progress.
Source: platform guidelines (Apple HIG loading and progress indicators;
Material Design 3 progress indicators)

## Controls show every state they can be in
Why: a button that looks the same when pressed, busy or unavailable
leaves people tapping again, waiting for nothing, or unsure why nothing
happens.
Do: design each control's states: normal, pressed, focused (for
keyboards on tablets and desktop), disabled, and loading. Make each one
clearly different but calm. When the main button is disabled, say what
is missing next to it ("Add a date to continue"), or keep it enabled and
point to the missing field when tapped.
Don't: disable a button with no explanation, or rely on a faded color
alone to show it can't be used.
Accessibility: disabled and busy states are announced to screen
readers, and the keyboard focus is always visible.
Note: hover states only exist with a mouse; on phones they don't apply.
Source: How to Design Better UI Components 3.0 (book)

## An error says what happened and how to fix it
Why: "Something went wrong" leaves the user stuck: they don't know if
it's their fault, if their work is lost, or what to try next.
Do: say in plain words what happened and what to do ("Couldn't save.
Check your connection and try again"), offer a "Try again" button where
retrying can help, and keep everything the user typed or chose. For a
field error, show it next to the field, in words, not only in red.
Don't: show bare error codes, blame the user, clear a form after a
failed send, or replace the whole screen when only one part failed.
Accessibility: errors are announced to screen readers, and marked with
an icon or text as well as color.
Source: platform guidelines (Material Design 3 text fields and
snackbars; Apple HIG alerts)

## Offline keeps the app useful
Why: phones lose signal often (trains, lifts, basements). An app that
goes blank or shows only an error when offline throws away content the
user already had.
Do: keep showing what was last loaded, with a calm note of how fresh it
is ("Offline · updated 10:42"). Save the user's actions and send them
when the connection returns, showing which ones are waiting. If
something truly can't work offline, say so at that action, not for the
whole app.
Don't: wipe the screen, block everything with a full-screen error, or
let an action look done when it hasn't been sent.
Accessibility: going offline and coming back are announced to screen
readers, not shown by color alone.
Note: the platform guides say little about offline; this rule is
common practice, in line with their loading and error guidance.
Source: common practice; platform guidelines (loading, errors)

## A missing page is never a dead end
Why: an old link, a deleted item or a moved page lands the user on
"Not found" with nowhere to go. They didn't do anything wrong, and a
bare message makes them feel stuck.
Do: say plainly what's missing ("This item was deleted or moved"), then
offer ways forward: search, the list it came from, home, or the most
likely related items. A touch of the app's personality is fine.
Don't: show only an error code, blame the user, or let a joke replace
the explanation and the way back.
Example: opening a shared link to a removed item shows "This item is no
longer available", a search field, and the newest similar items.
See also: "An error says what happened and how to fix it" above.
Source: uxpeak, The UI/UX Playbook (book)
