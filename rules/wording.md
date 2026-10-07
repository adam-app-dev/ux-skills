# Wording

**Memory hook:** specific words do the convincing.

Typography (typography.md) is how text looks. These rules are about what
the text says: buttons, titles, labels, small helper lines.

## Specific numbers beat vague words
Why: vague words ("quick", "easy", "fast") leave the user guessing; a
number answers the question before it's asked. A line like "Start in
2 taps" removes worries about forms, cards and steps in one go.
Do: replace vague claims with real counts and times ("2 taps",
"about 3 minutes", "arrives in 2 days").
Don't: write a number that isn't true or that you can't keep true for
every user. Don't round real counts into vague ones ("200+" when it's
221): exact real figures are more believable.
Note: the product page source advises picking specific-looking numbers
because they feel authentic. This repo never picks numbers; it shows the
real ones, which are naturally specific.
Example: "Set up in 3 steps" instead of "Quick setup".
(The video says "delivery in 23 minutes" beats "fast delivery"; treat it
as an illustration, not a measured result.)
Sources: uxpeak, three A/B test examples; uxpeak, product page conversion redesign

## The button names what happens now, and the commitment stays visible
Why: a heavy word on a button ("Subscribe", "Commit") makes users imagine
the hardest version of the deal. A word that describes the next step
("Start my free trial") is lighter and accurate.
Do: label the button with what tapping it does right now. Right next to
it, show what the user is agreeing to: price, billing period, and when
the first charge happens.
Don't: use a light word to hide a commitment. If the tap starts a paid
subscription, that must be clear at the button.
Note: the source presents "Start" vs "Subscribe" as a pure wording win.
This repo only allows it with the price and charge date visible beside
the button, which app stores and EU consumer rules require anyway.
Source: uxpeak, three A/B test examples

## Buttons are verbs that name the outcome
Why: "OK", "Yes", "Submit" or "Click here" make people reread the
question to know what the tap will do. Screen reader users often hear
buttons out of context, where a bare "Yes" means nothing.
Do: start the label with a verb and, when it helps, the object ("Save
changes", "Delete photo", "Send 3 invites"), so the button makes sense
on its own.
Don't: use "OK", "Yes/No", "Submit" or "Click here" for actions with a
specific outcome. People tap on phones, they don't click.
See also: hierarchy.md (a destructive confirmation says what it
destroys).
Source: How to Design Better UI Components 3.0 (book)

## Do the math for the user
Why: every calculation left to the user is a small reason to stop.
Do: show totals, durations and counts already worked out: the total on
the pay button ("Pay €445 total"), "5 nights" next to a date range,
day names next to dates ("Fri 28 Mar").
Don't: show raw inputs (two dates, a unit price) and leave the user to
compute what they mean.
Example: a date range shown as "Fri 28 Mar → Wed 2 Apr · 5 nights"
instead of two plain date fields.
See also: smart-defaults.md (buttons that state the result).
Source: uxpeak, three A/B test examples

## Concrete details beat generic labels
Why: a specific detail lets the user picture the thing; a generic label
makes everything sound the same.
Do: when a title or description is written for people (not data from a
user), lead with the one concrete detail that matters most
("2 minutes away", "steps from the beach", "ready in 10 minutes").
Don't: write a detail that isn't accurate. A vivid promise that turns out
false costs more trust than a plain label.
Source: uxpeak, three A/B test examples

## Unfamiliar terms are explained where they appear
Why: a term the user doesn't know (a fee name, a technical setting, a
plan feature) stops the decision. Sending them to a help page to find
out breaks the flow, and many won't come back.
Do: first try plain words instead of the term. If the term must stay,
add a small info button next to it that opens a one- or two-sentence
explanation in place (a tooltip or a small sheet), closable with one tap.
Don't: rely on hover to show explanations (phones have no hover), or
hide the meaning of a fee or a limit behind a link to a help page.
Accessibility: the info button has a label ("What is a service fee?")
and the explanation is read by screen readers.
See also: show-the-catch.md (fees and limits up front).
Source: How to Design Better UI Components 3.0 (book)
