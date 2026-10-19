# Medina's Airwork — handoff at ~60%

**Live:** https://10elizabethbell.github.io/medinasAirwork/ · **Repo:** https://github.com/10elizabethbell/medinasAirwork · **Built:** 2026-10-19 from Muse brief (run 2026-10-19, Facebook group "HVAC Business Owners & Contractors" post 1869884327698443)

## What's built
- Single page `index.html` (inline CSS/JS, system fonts, no tracking), photos in `img/`, `favicon.svg`, `apple-touch-icon.png`, `og.jpg` (1200x630, the real hero).
- **World: airflow currents.** Deep navy from Miguel's flyer, electric-blue wordmark, flame orange for heat, ice blue for cool air, heavy italic uppercase like his logo.
- **Signature element:** the hero is a field of moving air (canvas, ~700 streaks on phones, 1,700 on desktop). Drag a finger or mouse through it and the air warms from ice blue to flame orange, gets pushed aside, rises, then cools back. When nobody touches it, an invisible heater wanders the lower air so it plays by itself. On phones the area under the buttons takes drags in every direction (no scrolling there). The text, logo, phone number and hint have clear zones, so no air runs through them.
- Section dividers are moving air seams (three lines plus a fill that follows the middle one). Slow drifting air sits behind the install photos.
- Sections: header (wordmark, top-right `tel:` number) → hero (WARM WINTERS. COOL SUMMERS., Miguel's promise, "Get a free estimate" + "Contractor? Work with me") → What I work on (6 service rows; tapping one pre-ticks it in the form) → How it works (3 steps + "Licensed & insured. Estimates are always free.") → Recent installs (2 photos + "Click to see more of my work" to Facebook) → Where I work → Contractors (text button) → Free estimate form (composes an SMS to 215-839-2766, with a copy fallback if texting doesn't open) → footer (phone, email, Facebook).
- Tunable constants are at the top of each script block (`CFG` in hero air: speed, particle counts, heat radius, cooling rate, idle delay; `SPEED/AMP` for seams; `COUNT/SPEED` for the proof drift).

## Assumptions I made
- **Colours** come from the flyer (navy, royal blue, flame orange, ice blue).
- **No logo file exists** (the flyer's lettering sits on a busy background). The wordmark is set in the site's own lettering with a roofline drawn after the flyer's house. The favicon is that roof plus an italic "M".
- **"Delaware" on the flyer is read as Delaware County, PA**, because it's listed with Bucks and Montgomery County. It could mean the state of Delaware.
- **The two photos are assumed to be Miguel's installs** (air handler from his profile image, condenser from the flyer). The "Recent installs" heading and the alt text claim this. Neither is confirmed.
- **The page speaks as "I"** (Miguel posted as the owner). Whether he has a crew is unknown.
- **The services list is shortened to 6 rows** (furnaces, heat pumps, mini splits, central air, air handlers, water heaters). The lede covers installs/replacements/repairs/maintenance.
- **Headline:** "Warm winters. Cool summers." is mine (benefit, heating-season lead). His flyer tagline "Heating & cooling solutions you can trust" is in the footer.

## Placeholders and gaps
- **Texts: unknown.** The estimate form, the contractor button and step 1 all assume 215-839-2766 takes texts. If it doesn't, switch the form to a call or change the copy.
- **"Licensed & insured" is the owner's own flyer claim, not verified.**
- **The photos are low resolution** (cropped from the flyer: 254px and 516px wide), so they're soft on 2x/3x phones. They're shown at or below native size on desktop.
- No hours, prices, reviews, years in business, surname or address. None appear on the page.
- The Carrier units in the photos imply nothing on the page (no affiliation claim).

## Questions for the owner
1. Does 215-839-2766 take texts?
2. Can you send the original install photos (and more jobs, before/afters)?
3. Licensed & insured: license number or insurer to confirm?
4. Delaware County, or the state of Delaware too?
5. Is it just you, or a crew ("I" vs "we")?
6. Hours / emergency calls? Brands you install?
7. Which jobs do you want more of: installs, repairs, contractor work?

## Ideas not built (yours to pick)
- **Runner-up world: duct blueprint.** A white-line mechanical drawing of a house section on navy, with air traced through the ducts. Impeccable's roll actually assigned this one; Ellie's pick rule (fluid, touchable, on-brand) chose airflow.
- Bring in the flyer's snowflake and flame: e.g. a tiny flame appears where you heat, frost where air is coldest.
- A thermostat readout in the hero that climbs (62° → 72°) as you warm the air.
- A warm flare across the page when "Text this to Miguel" is tapped.
- Let the proof-band air lap the base of the photos more (photos still look a bit placed on desktop).
- Desktop services: the left column under the heading is empty; a still of the air field or the condenser photo could fill it.
- Make the air broader and wispier if it reads as "starfield" rather than air to you (`TRAIL`, line widths in `CFG`). The finish reviewer raised this as a taste call.
- A separate contractors page if that side of the business grows.

## Not verified
- Real-device touch (iOS Safari, Android Chrome, Facebook in-app browser): drag-to-heat, no pull-to-refresh, scroll still works outside the air pad.
- The real SMS handoff on iOS and Android (`sms:+12158392766?&body=`), and how the copy fallback behaves in the FB in-app browser.
- Frame rate on older phones.
- Headless Chrome doesn't capture canvas in top-level screenshots; all review shots were taken inside an iframe.

## Review status
Impeccable: detector run (system-font finding suppressed as house style; flat-type-scale finding left standing, sizes separated by weight). All 16 modes swept by an agent (no live/onboard); finish reviewer ran 2 rounds, disposition **fix**. Resolved: duplicate call link, photo shapes, HANDOFF, desktop composition, recapture. Fixed after the last verdict and not re-scored: county names wrapping mid-name, the rectangular clear zones behind text (now feathered ellipses). **Still open, yours to call:** the photos still sit as plain cards on the drifting air (not wrapped by it), and the reviewer felt the dense desktop air can read as "combed fur" rather than air; I thinned it (`COUNT_DESK` 1150, `TRAIL` .068) but it needs your eye.
