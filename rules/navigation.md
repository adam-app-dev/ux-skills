# Navigation

**Memory hook:** the backbone, not a toolbox.

The bottom navigation bar (iOS calls it a tab bar) shows the app's
top-level structure and is one of the most-tapped areas of any app.
Sizes, colors, borders and shadows come from the design system.
These rules say what the bar must do.

## The bar holds the top sections, by how often they're used
Why: the bar tells users what matters in the app and lets them move
between core sections in one tap. Every slot is valuable.
Do: include only the main destinations people use often (home, search,
the main list, messages, profile).
Don't: put rarely used things in the bar (help, log out, legal pages,
settings details). They belong in the profile or settings screen.
Don't repeat a tab's destination elsewhere on the same screen (a search
icon in the top bar and a Search tab, a profile avatar and a Profile
tab): each duplicate is one more thing to scan and wonder about.
Sources: uxpeak, bottom navigation guide; How to Design Better UI
Components 3.0 (book)

## Familiar beats clever
Why: people spend most of their time in other apps and expect yours to
work the same way. Moving well-known controls to unusual places makes
them hunt.
Do: keep back buttons, titles and logos in the top bar, where people
expect them. A creative bar shape or layout is fine only if it is still
instantly usable.
Don't: put back/forward buttons or a logo in the bottom bar, or trade
usability for a striking look.
Source: uxpeak, bottom navigation guide

## Three to five tabs
Why: more tabs mean smaller targets, more mis-taps and more choices to
scan.
Do: use 3 to 5 tabs, chosen from the app's core functions.
Don't: squeeze in a sixth tab. If more sections exist, group them inside
one of the tabs.
Note: the source allows up to six. This repo follows the platform
guidelines (iOS and Android's Material Design both say five at most).
Source: uxpeak, bottom navigation guide; platform guidelines

## Places in the bar, actions outside it (default)
Why: tabs take you somewhere; an action (create, post, add) does
something. Mixing them in one row makes it unclear what a tap will do.
Do: by default, put the main "create" action in a floating action button
above the content, not in the bar.
Don't: put actions in the bar just to make them visible.
Variant (use only when a project's design calls for it): a centered
"Create" button inside the bar. Use it only when creating is the app's
core activity, and make it clearly look like an action (a different
shape, not just another tab). Tapping it opens the create flow (often a
sheet) instead of switching tabs.
Note: the source recommends the centered button as a default. This repo
keeps it as a variant because both platform guidelines reserve the bar
for destinations.
Source: uxpeak, bottom navigation guide; platform guidelines

## Every tab has a label
Why: icons alone are guesswork for many people, and screen readers need
a name for each tab anyway.
Do: show a short text label under every icon. Labels must grow with the
phone's text size setting.
Don't: ship an icon-only bar, or set labels so small they're hard to read.
Note: the source says icon-only bars can work for young, tech-savvy
audiences. This repo always labels, for accessibility.
Source: uxpeak, bottom navigation guide

## Labels are one short word
Why: long labels wrap to two lines, make the bar taller and slow down
scanning.
Do: use one short word per tab, and check it in long languages
(Italian, German).
Don't: let labels wrap or shrink the font to fit. Pick a shorter word.
Source: uxpeak, bottom navigation guide

## The current tab is obvious, in at least two ways
Why: users must see instantly where they are. A single small change
(only the label, or only the color) is easy to miss, and color alone
fails colorblind users.
Do: change at least two things on the active tab, for example the icon
goes from outlined to filled and the color changes, or the color changes
and the label gets bolder. Make screen readers announce the selected
tab (in Compose, the navigation item's selected state).
Don't: change only the text, or only the color.
Source: uxpeak, bottom navigation guide

## Inactive tabs are softer but still readable
Why: inactive tabs must step back without disappearing, especially for
users with low vision.
Do: soften inactive tabs (for example lower opacity), and check the
contrast: at least 3:1 for icons, at least 4.5:1 for label text.
Don't: fade inactive tabs until they're hard to see.
Note: the source cites 3:1 for everything. That's the minimum for icons
and shapes; text labels need 4.5:1.
Source: uxpeak, bottom navigation guide

## The bar stays calm
Why: the bar is part of the frame, not the content. A loud bar pulls
attention from what users came for and from the screen's main action.
Do: use neutral colors for the bar, consistent with the top bar, and
save bright color for key actions on the screen. A brand color is fine
if it doesn't overpower the content.
Don't: give the top and bottom bars unrelated color schemes.
See also: hierarchy.md (few things compete for attention, color is
intentional).
Source: uxpeak, bottom navigation guide

## The bar is visibly separate from the content
Why: without separation, content scrolling under the bar blends into it
and the bar stops reading as navigation.
Do: separate it with one subtle cue: a thin line, a slightly different
background, or a soft shadow.
Don't: use heavy lines or big, harsh shadows.
See also: hierarchy.md (separators stay subtle).
Source: uxpeak, bottom navigation guide

## Badges are rare and readable
Why: a badge is useful only while it means "something important is
waiting". Badges on everything get ignored.
Do: use badges only for updates the user truly needs to see (a dot, or
a count when the number matters), placed consistently on the icon, with
a readable count. Screen readers announce it ("Messages, 3 unread").
Don't: badge every minor update, or use a tiny or decorative font for
the count.
Source: uxpeak, bottom navigation guide

## Every tap gets feedback
Why: a tap with no visible response feels broken; small motion makes
navigation feel connected instead of jumping.
Do: respond instantly to a tap (color change, ripple), move the
active-tab indicator smoothly, and use gentle transitions between
screens.
Don't: add long or flashy animations. Always respect the phone's
"reduce motion" setting.
Source: uxpeak, bottom navigation guide

## On wide screens, the bar moves to the side
Why: on tablets, desktop windows and landscape, a bottom bar stretches
across a wide screen and sits far from the content.
Do: switch to a side navigation rail (or a side menu) on wide screens,
with the same destinations in the same order. In Kotlin Multiplatform,
plan for this from the start.
Don't: stretch the phone bottom bar across a wide window.
Note: this rule is from the platform guidelines (Material Design's
adaptive navigation), not the source video. The repo added it because
apps built once for phone, tablet and desktop need it.
Source: platform guidelines (Material Design, adaptive layouts)
