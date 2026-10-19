---
name: Medina's Airwork
description: A Philadelphia heating and cooling pro's site made of air you can touch and heat with a finger.
colors:
  navy: "#0c1f45"
  navy-2: "#13306a"
  blue: "#1d63ff"
  blue-bright: "#4a8dff"
  ice: "#a9dcff"
  flame: "#ff6b1a"
  flame-hi: "#ff8a3d"
  paper: "#eef3fa"
  paper-2: "#ffffff"
  ink: "#0c1f45"
  ink-soft: "#3c5079"
  on-dark: "#ffffff"
  on-dark-soft: "#c3d2ee"
  line-light: "#d3deef"
  error-ink: "#b4261a"
typography:
  display:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(2.7rem, 12.2vw, 5.6rem)"
    fontWeight: 900
    lineHeight: 0.98
    letterSpacing: "-0.02em"
  headline:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(2rem, 8.4vw, 3.4rem)"
    fontWeight: 900
    lineHeight: 0.98
    letterSpacing: "-0.02em"
  title:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "1.25rem"
    fontWeight: 800
    lineHeight: 1.3
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.55
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "1.125rem"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "0.875rem"
    fontWeight: 700
    lineHeight: 1.4
  button:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "1.05rem"
    fontWeight: 800
    lineHeight: 1.2
rounded:
  pill: "999px"
  card: "14px"
  control: "12px"
  inset: "10px"
  circle: "50%"
spacing:
  gutter: "20px"
  gutter-wide: "32px"
  container: "1180px"
  band-y: "56px"
  band-y-wide: "96px"
  stack: "22px"
  chip-gap: "10px"
  seam: "64px"
  seam-wide: "90px"
components:
  button-fire:
    backgroundColor: "{colors.flame}"
    textColor: "{colors.navy}"
    typography: "{typography.button}"
    rounded: "{rounded.pill}"
    padding: "0 1.4rem"
    height: "56px"
  button-fire-hover:
    backgroundColor: "{colors.flame-hi}"
    textColor: "{colors.navy}"
  button-line:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    typography: "{typography.button}"
    rounded: "{rounded.pill}"
    padding: "0 1.4rem"
    height: "56px"
  button-white:
    backgroundColor: "{colors.paper-2}"
    textColor: "{colors.navy}"
    typography: "{typography.button}"
    rounded: "{rounded.pill}"
    padding: "0 1.4rem"
    height: "56px"
  button-white-hover:
    backgroundColor: "{colors.ice}"
    textColor: "{colors.navy}"
  input-text:
    backgroundColor: "{colors.paper-2}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.control}"
    padding: "13px 15px"
    height: "54px"
  chip:
    backgroundColor: "{colors.paper-2}"
    textColor: "{colors.ink}"
    rounded: "{rounded.control}"
    padding: "0 16px"
    height: "46px"
  chip-selected:
    backgroundColor: "{colors.navy}"
    textColor: "{colors.on-dark}"
  step-number:
    backgroundColor: "{colors.navy}"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.circle}"
    size: "52px"
  photo-card:
    backgroundColor: "{colors.navy-2}"
    rounded: "{rounded.card}"
---

# Design System: Medina's Airwork

## Overview

**Creative North Star: "The Moving Air"**

Miguel's trade is moving warm and cool air, so the site is built from air. A deep navy ground (lifted straight from his flyer) carries fine streaming currents that run warm (flame orange) or cool (ice blue). In the hero you can touch the current and heat it with a finger. Between sections the edge is never a ruled line: it's a live seam of three wavering air lines with the next band's colour filling in under the middle one. Light paper bands sit between the dark ones like rooms the air moves through.

The voice is loud and local, never corporate. Display type is heavy italic uppercase, like the logo lettering on his van and flyer, set in the system font stack. This is the owner's pinned house style, not a placeholder. Everything else stays quiet and phone-first: big pill buttons at least 56px tall, list rows that read like a menu, and an estimate form that becomes a pre-written text. Density is generous on phones and opens into two-column splits on desktop.

Colour carries temperature. Orange means heat and action (the primary CTA, the warm word, warm particles). Ice and blue mean cool air and calm structure. The two never trade places.

**Key Characteristics:**
- Navy-and-paper alternating bands joined by animated air seams, never straight edges.
- Heavy italic uppercase display in the system stack, tight leading (0.98), slight negative tracking.
- Temperature palette: flame = heat and action, ice/blue = cool air and structure.
- Canvas particle fields (hero, proof band) are the imagery. There's no stock photography; the only photos are real install shots.
- Pill buttons, softly rounded controls, circular markers. No sharp corners anywhere.

## Colors

A temperature palette on a navy ground: one hot accent, one cool family, and blue-tinted neutrals.

### Primary
- **Flame Orange** (`flame`): Heat and action. The primary CTA fill ("Get a free estimate", "Text this to Miguel"), the word "Warm" in the hero, warm particles, the hot end of the hero's heat ramp, the third seam line, row-arrow hover, text selection, and the underline on inline call links. Text on flame is always navy.
- **Flame Light** (`flame-hi`): Hover state for flame fills. Also the warm drift particles in the proof band.

### Secondary
- **Electric Blue** (`blue`): The cool structural accent on light bands. Input/chip hover and focus borders with a translucent halo, focus outlines on light grounds, the service-area icons, the first seam line over light bands.
- **Bright Wordmark Blue** (`blue-bright`): The second word of the wordmark ("Airwork") and the first seam line over dark bands. Also a faint radial glow in the hero ground.

### Tertiary
- **Ice Blue** (`ice`): Cool air. The word "Cool" in the hero, cool particles, the focus outline on dark grounds, icons in the header and footer, link hover on dark, hover fill for the white Facebook button.

### Neutral
- **Flyer Navy** (`navy`): The ground. Body background, hero, dark bands, footer, step-number circles, selected chips. Doubles as `ink`, the primary text colour on light bands.
- **Deep Navy Lift** (`navy-2`): The fill behind photo cards while they load.
- **Soft Ink** (`ink-soft`): Secondary text on light bands: ledes, step copy, helper notes, the "(optional)" marker.
- **Cool Paper** (`paper`): The light band ground. Also the inset fill for the copied-message block.
- **White** (`paper-2` / `on-dark`): The alternate light band, input and chip fills, and primary text on dark.
- **Mist** (`on-dark-soft`): Secondary text on dark: the hero promise, dark-band ledes, the footer body, the drag hint.
- **Hairline** (`line-light`): 1px service-row rules and the resting 2px border of inputs, chips and the fallback panel.
- **Error Ink** (`error-ink`): Inline validation messages.

### Named Rules
**The Temperature Rule.** Orange is heat, blue and ice are cool. Flame marks the one primary action and anything warm. Never use it for neutral decoration, and never set the cool family on a warm meaning.

**The Navy Ink Rule.** Text on flame is navy, never white. The navy-on-orange pairing comes from the flyer, and it holds contrast.

**The Two Grounds Rule.** Surfaces are either the navy ground or a paper band (`paper` or `paper-2`). There are no grey or tinted mid-surfaces.

## Typography

**Display Font:** System stack (-apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif), at 900 italic uppercase
**Body Font:** The same system stack

**Character:** One family pushed to two extremes. Black italic capitals shout like van lettering, and plain system text speaks as Miguel in the first person. The stack is a pinned owner requirement. Its character comes from weight, slant and case, not from a typeface.

### Hierarchy
- **Display** (900 italic uppercase, clamp(2.7rem, 12.2vw, 5.6rem), 0.98, -0.02em): The hero headline only. Single words can be coloured flame (warm) or ice (cool).
- **Headline** (900 italic uppercase, clamp(2rem, 8.4vw, 3.4rem), 0.98, -0.02em, balanced wrap): One per section, as the section title.
- **Title** (800, 1.25rem): Service-row labels, step headings, the place list (at 700).
- **Body** (400, 17px rising to 18px at 1024px and up, 1.55): Running copy. Ledes run 1.125rem in soft ink, capped at 38ch. The hero promise caps at 34ch.
- **Label** (700, 0.875rem): The drag hint, validation errors, helper notes (helper notes at 400).
- **Button** (800, 1.05rem): All pill buttons and the header phone number (tabular numerals).

### Named Rules
**The Van Lettering Rule.** Only the hero headline, section headlines, the wordmark and the step numerals use 900 italic. Everything else stays upright.

**The One Voice Rule.** Copy is set as Miguel speaking. Strong weight (700 to 800) marks his commitments ("I'm Miguel.", "Licensed & insured."), not decoration.

## Layout

Single column on phones inside a 1180px container with 20px gutters (32px from 700px up). Section bands pad 56px top / 64px bottom, rising to 96px / 104px at 1024px. At 1024px most bands become a two-column split (1fr / 1.1fr, 72px gap): the headline and lede on the left, a list or action on the right. Steps go to three equal columns (36px gap). The estimate form goes to two columns (28px column gap), with the chip groups, notes and submit spanning the full width. Form fields stack at 22px. The proof band uses a work grid, with copy and the Facebook button on the left and an asymmetric pair of photos (one tall, one wide, bottom-aligned) on the right.

The hero is phone-first. The headline, promise and two stacked full-width CTAs come first, then a 230 to 320px touch field (the "air pad") underneath. On desktop the hero grows to min(92svh, 860px), the copy centres vertically, and the air pad covers the whole hero. Tap targets are at least 44px; primary buttons are 56px.

**The Bands-and-Seams Rule.** The page is a vertical run of full-bleed bands alternating navy and paper. Every band boundary is an air seam (64px tall, 90px at 1024px), never a hard edge.

## Elevation & Depth

Mostly flat, with depth coming from the air. Particle canvases sit behind the content, and radial blue glows tint the hero ground. There are only two shadows, both soft and diffuse, and both go on objects sitting over the navy ground.

### Shadow Vocabulary
- **CTA lift** (`box-shadow: 0 8px 18px -8px rgba(4,12,32,.55)`): Under flame buttons only.
- **Photo float** (`box-shadow: 0 22px 40px -18px rgba(0,0,0,.6)`): Under install photos in the dark proof band.
- **Focus halo** (`box-shadow: 0 0 0 3px rgba(29,99,255,.18)`): A blue glow on input, chip and copy-button hover/focus. It's a state ring, not elevation.

### Named Rules
**The Air Is The Depth Rule.** Layering comes from streaming air behind the content, not stacked cards. On light bands, controls stay flat and get only the focus halo.

## Shapes

Everything is rounded and nothing is sharp. Buttons are full pills (999px). Inputs, chips and the copy button share a 12px control radius. Photo cards and the fallback panel use 14px. Inset blocks and the skip link use 10px. Step numerals and row arrows are perfect circles. Borders are 2px on interactive controls, and 1px hairlines only between service rows. The signature silhouette is the wave. Seam edges are sine-summed curves drawn across a 1440-wide viewBox, and the wordmark carries a stroked roofline glyph with a chimney.

## Components

### Buttons
Big, round-ended and confident. They're built for thumbs.
- **Shape:** Full pill (999px), 56px minimum height, 2px border, icon gap 0.6rem, 22px inline SVG icons. Full width on phones, auto width from 700px.
- **Fire (primary):** Flame fill, navy text, CTA lift shadow. Hover goes to flame light. Inside the form, hover/focus adds a 3px blue outline.
- **Line (secondary, dark grounds):** Transparent with white text and a 75% white border. Hover goes to a solid white border plus an 8% white wash.
- **White (dark grounds, external link):** White fill and navy text, ice on hover. Used for the Facebook link, with the icon in Facebook blue.
- **Press:** scale(.98). Transitions run 0.2s on colour and 0.15s on transform. They're removed under reduced motion.

### Chips
- **Style:** White fill, 2px hairline border, 12px radius, 46px tall, 16px inline padding, 700 weight. A visually hidden native checkbox or radio drives each chip.
- **State:** Hover and keyboard focus give a blue border plus the focus halo. Selected is a navy fill with white text. Selected + hover/focus keeps navy and adds a blue border.

### Inputs / Fields
- **Style:** White, 2px hairline border, 12px radius, 54px minimum height (textarea 110px, resize vertical), 17px text. Labels sit above at 800 weight.
- **Focus:** Blue border plus the focus halo, with no outline. Hover gets the same treatment.
- **Error:** The message appears below in error ink (0.875rem, 700), the border turns red, and aria-invalid is set. Errors use Miguel's voice ("Add your name so I know who's texting.").

### Service Rows
A menu, not cards. Rows of 1.25rem/800 navy labels, 64px tall, separated by 1px hairlines, each with a 40px circular arrow chip on the right (pale blue fill). On hover/focus the arrow fills flame with a white glyph, and focus adds a flame outline around the arrow. Tapping a row pre-ticks the matching chip in the estimate form.

### Step Markers
52px navy circles holding a white 900 italic numeral, next to an 800 title and soft-ink copy. Stacked on phones, three columns on desktop.

### Navigation
There's no nav menu. The header sits over the hero: the wordmark on the left (stroked roof glyph, "MEDINA'S" in white over "AIRWORK" in bright blue, 900 italic uppercase, line-height 0.86), and the phone number on the right (800, tabular numerals, ice phone icon that turns flame on hover). The footer repeats the wordmark, the tagline, and 44px-tall contact links with ice icons.

### Hero Air Field (signature)
A full-bleed canvas of streaming particle trails over the navy ground, drifting left to right like air leaving a register. Dragging a finger adds heat to an 18px grid. Particles passing through warm cells shift colour along a five-stop ramp (ice to pale ice to warm white to orange to flame), get thicker and brighter, and rise. Heat cools back and drifts up. After 3.5s of idle an invisible heater wanders the lower air so the page keeps playing by itself. Soft elliptical "still air" masks keep trails out from behind the headline, wordmark, phone and hint. Tuning constants: 700 particles on phones and 1150 on desktop, speed 1.35, drift 0.55, trail fade 0.068, heat radius 80px, push radius 95px. A "Drag to turn up the heat" hint (flame hand icon) fades on first touch. Rendering is capped at 1.5x DPR, pauses offscreen, and under reduced motion shows a pre-rendered still frame.

### Air Seam (signature)
The section divider. An SVG band (viewBox 1440x90, stretched) is filled with the previous band's colour. The next band's colour fills up to the middle of three wavering lines. Over dark the lines are bright blue / ice / flame, over light they're blue / bright blue / flame, at 1.6 / 2.6 / 1.6 stroke widths and 0.7 to 0.8 opacity. Each seam has its own phase, animates only while visible, and stays static under reduced motion.

### Proof Drift
A quiet, non-interactive canvas behind the dark proof band. Around 160 particles (60% on phones) stream left to right at speed 0.6. About 22% are warm (flame light) and the rest ice, with long trails. It keeps the air present behind the real install photos without competing with them.

## Do's and Don'ts

### Do:
- **Do** join every pair of bands with an air seam, filled with the outgoing band's colour and the incoming band's colour.
- **Do** set section headlines in 900 italic uppercase at clamp(2rem, 8.4vw, 3.4rem) with 0.98 leading, in the system stack.
- **Do** keep flame for the single primary action per view and for anything warm. Put navy text on it.
- **Do** use ice for focus on dark grounds and electric blue for focus on light grounds (3px outline, 3px offset).
- **Do** keep tap targets at 44px or more and primary buttons at 56px, full width on phones.
- **Do** let canvases pause offscreen and fall back to a still frame under prefers-reduced-motion.
- **Do** keep moving air out from behind text, using soft masks rather than hard boxes.

### Don't:
- **Don't** separate bands with straight edges or ruled lines. Hairlines belong only between list rows.
- **Don't** use flame for decoration, borders on neutral controls, or cool meanings.
- **Don't** introduce a webfont or a second family. The system stack at extreme weights is the owner's house style.
- **Don't** add stock photography or icon-card grids. The imagery is the air and Miguel's real install photos.
- **Don't** add sharp corners. Every shape is a pill, a 10 to 14px round, or a circle.
- **Don't** add shadows on light bands beyond the focus halo.
