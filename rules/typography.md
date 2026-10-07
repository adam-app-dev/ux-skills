# Typography

**Memory hook:** headlines attract, paragraphs support.

The font family and the type scale come from the design system.
These rules say how to use them.

## One font family is enough
Why: many font styles make a screen feel inconsistent and weaken its
foundation.
Do: build hierarchy with size, weight, color and line height within one
family.
Don't: add a second or third font to create emphasis.
Source: uxpeak, product page redesign

## Headlines attract, paragraphs support
Why: body text should help users understand, not fight for attention.
Do: give paragraphs comfortable line height so they are easy to read,
and a slightly softer color than headlines.
Don't: set body text with tight lines or at full headline strength.
Accessibility limit: softer body text must still meet the minimum
contrast for readable text (WCAG AA, 4.5:1). Never go below it.
Source: uxpeak, product page redesign

## Long text keeps a comfortable line length
Why: very long lines make the eye lose its place when jumping back to
the start of the next line; very short lines break every few words.
Both make reading tiring.
Do: keep reading text to a comfortable width. On a phone in portrait
this mostly happens by itself. On tablets, landscape and desktop
windows, cap the width of the text column instead of stretching it
across the screen. As a rough guide: about 45 to 75 characters per line
on wide screens, and roughly 30 to 40 on phones.
Don't: let paragraphs run edge to edge on a wide window.
Note: the character ranges are common guidance from print and web
reading, not exact limits; treat them as a rough guide.
See also: navigation.md (on wide screens, the bar moves to the side).
Source: uxpeak, The UI/UX Playbook (book)

## Long text comes in short, labeled pieces
Why: a long block of text looks like work, so people skip it, including
the one line they needed. Short paragraphs and subheadings let them scan
for their part and stop there.
Do: split any text longer than a few lines (help, descriptions, terms,
onboarding) into short paragraphs, one idea each, with a subheading
that says what the piece is about.
Don't: put several ideas in one long paragraph, or write subheadings
that are decorative rather than descriptive.
Accessibility: subheadings are marked as headings so screen reader users
can jump between them (in Compose, semantics `heading()`); icons next to
subheadings are decorative and hidden from screen readers.
Source: uxpeak, The UI/UX Playbook (book)

## Align text by what it is
Why: the eye needs a fixed place to start each line. Text that starts
somewhere different on every line is tiring to read, and numbers that
don't line up are hard to compare.
Do:
- **Text people read** (paragraphs, lists, labels): align to the start
  edge, so every line begins in the same place.
- **Numbers people compare** (amounts, prices, columns of values): align
  to the end edge, so units line up under units.
- **Short standalone text** (a title, a one-line empty-state message, a
  button label): centering is fine.
In Compose, use start and end, never left and right, so the layout flips
by itself for right-to-left languages.
Don't: center paragraphs or lists longer than a couple of lines, or
start-align a column of amounts the user compares.
Source: uxpeak, The UI/UX Playbook (book)

## Small uppercase labels need room
Why: small capital letters set tightly feel cramped and are harder to read.
Do: add a little letter spacing to small uppercase labels.
Don't: use default (tight) spacing on small all-caps text.
Source: uxpeak, product page redesign

## Badges are scannable in a glance
Why: a badge must be understood instantly. Extra words and icons slow it
down and steal attention from the content.
Do: keep badges to the essential words ("20% off", "New", "Due soon").
Don't: say the same thing twice ("20% off discount") or add an icon that
repeats the text.
Source: uxpeak, product page redesign
