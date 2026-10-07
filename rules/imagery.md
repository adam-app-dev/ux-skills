# Imagery

**Memory hook:** works on any photo.

Values (corner radius, overlay color, opacity) come from the design system.
These rules say what images must do.

## Anything on top of a photo gets its own background
Why: icons or text placed directly on a photo are only readable because
that particular photo happens to be dark (or light). Swap the photo and
they disappear.
Do: put a subtle container behind overlaid icons and text, with enough
contrast and, if needed, a thin outline, so they stay readable on dark,
bright and busy images. For text along an edge (a caption, a title on a
card), the background can also be a soft gradient (scrim) or a blur of
the image behind the text.
Don't: rely on the demo photo to make overlays readable.
Example: back and favorite icons over a header photo look fine on a dark
image and vanish on a bright one (a pineapple, a white dog).
Note: blur isn't available everywhere (in Compose, `Modifier.blur` needs
Android 12 or later). Where it isn't, fall back to the gradient.
Sources: uxpeak, product page redesign; uxpeak, The UI/UX Playbook (book)

## Every image has one clear focal point
Why: when the whole frame is busy, the eye has nowhere to land.
Do: make the subject (product, pet, item) the obvious focus.
Don't: use images where the subject fills the frame chaotically, or where
something else (hands, props) becomes the focus.
Source: uxpeak, product page redesign

## The image matches what the user actually gets
Why: a mismatch between image and reality creates small doubts.
Do: show the thing as it's sold or used (sold by weight → show a portion,
not a single piece).
Don't: use an image that implies a different quantity, size or version.
Source: uxpeak, product page redesign

## Show the real thing, not decoration
Why: people can't commit to something they can't picture. A decorative
illustration can be beautiful and still not answer "what am I actually
getting?"
Do: use images of the real content, product or result (actual items,
real screens, real examples from the library).
Don't: fill the key image slot with generic art or mood pictures when
real content exists.
Example: an upgrade screen shows a few of the actual items the plan
unlocks, instead of an abstract illustration.
Example: for content people get (a guide, a template, a course), show a
peek inside (sample pages, real screenshots), not only the cover.
(The source reports a big conversion jump from this on its own sales
page, without data; treat it as an illustration.)
Sources: uxpeak, three A/B test examples; uxpeak, five UX/UI design tips (Playbook)

## Show it in use, not only on its own
Why: people can't touch what's on a screen. An object alone on a plain
background makes them imagine the experience themselves; a picture of it
in use (or of its result) answers "what will this be like?" at a glance.
Do: pair the plain item with an image of it being used or of the
result (the finished dish, the filled-in template, the set-up room).
Don't: let the "in use" image promise more than the user gets. If extras
appear in the photo that aren't included, it breaks "The image matches
what the user actually gets" above.
Note: the source says the brain processes images "infinitely faster"
than text. That's a popular exaggeration; the safe claim is simply that
a picture is understood faster than a description.
Source: uxpeak, product page conversion redesign

## When the image is the thing being chosen, give it room
Why: for a place, a product or anything chosen mostly by how it looks,
the photo is the main information. Squeezed into a small thumbnail, it
turns an exciting choice into a form to fill in.
Do: give the main image a large share of the screen, and show when more
images exist (for example "1 of 24").
Don't: shrink the deciding image to make room for fields and labels.
Note: this is about images that drive the decision. Lists, settings and
data screens don't need large images.
Source: uxpeak, three A/B test examples

## When the image only identifies the item, keep it small
Why: in a basket, a list or a summary, the user already knows what the
item is. The picture is a reminder; the name, amount and actions are what
they came for. An oversized image pushes those aside and makes every row
taller to scan.
Do: keep the image small enough that the name and value lead the row,
and the same size for every row.
Don't: carry the large image from the detail screen into lists and
summaries.
See also: "When the image is the thing being chosen, give it room" above
(the opposite case), and hierarchy.md (rank the information).
Source: uxpeak, The UI/UX Playbook (book)

## Images that appear together follow one visual system
Why: a single beautiful image can still make a list feel messy if every
item has different backgrounds, lighting and props.
Do: keep backgrounds, lighting and framing consistent across items that
appear side by side (grids, lists, catalogs). When the images themselves
vary in shape and size, place each one in the same frame (same shape,
same size, same position) so the set still looks like one family.
Don't: judge an image alone; judge it inside the list it will live in.
Note: when users upload their own images (profiles, pets), you can't
control them, so the layout around them must handle any photo
(see the first rule, and the core rule in SKILL.md).
Sources: uxpeak, product page redesign; uxpeak, The UI/UX Playbook (book)

## The image's mood fits the content
Why: style sets expectations. Artificial styling can undermine content
that should feel natural or trustworthy.
Do: match the visual feel to what the content promises (fresh, natural,
calm, professional).
Don't: add styling that fights the message.
Source: uxpeak, product page redesign

## Options people browse get a visual cue in one shared style
Why: a plain list of names makes users read every line; busy photos make
every option shout. A simple, matching visual per option lets people
recognize what they want at a glance.
Do: give each browsable option (categories, collections, types) a clear
image or icon of its subject, all in the same style, on a calm, solid
background. Text on that background meets the 4.5:1 contrast minimum.
Don't: use mismatched stock photos with text laid on top, or a long
plain list when people browse more than they search.
See also: "Images that appear together follow one visual system" and
"Anything on top of a photo gets its own background" above.
Source: uxpeak, five advanced UX/UI tips

## Steps that explain a process each get a picture
Why: three blocks of text that look alike ("Order", "On the way",
"Delivered") make a new user read everything to grasp the flow. A simple
picture per step is understood at a glance and makes the order easy to
remember.
Do: when explaining how something works (onboarding, a "how it works"
section, the stages of a request), give each step one simple picture of
what happens in it, in one shared style, and mark which step this is
with a number or text ("Step 2 of 3").
Don't: mark the position with a colored bar alone, or use pictures that
are decoration rather than a picture of the step.
Accessibility: the pictures are decorative for screen readers when the
step text already says everything.
See also: placement.md (a process with stages is shown as steps), for
showing where a live request stands.
Source: uxpeak, The UI/UX Playbook (book)

## People and companies are shown with their face or logo
Why: a photo or logo is recognized faster than a name, so users spot who
a message, payment or item is from at a glance.
Do: show the person's photo or the company's logo next to their name.
When none exists, show their initials on a colored background, with
text that meets the 4.5:1 contrast minimum.
Don't: leave a blank or generic silhouette for everyone, or let the
image replace the name. Screen readers read the name, not "image" or a
single letter.
Example: a list of messages, contacts or transactions, each with an
avatar or logo.
Source: uxpeak, top UI design tips part 2
