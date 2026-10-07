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
