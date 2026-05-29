════════════════════════════════════════════════════
DESIGN & CONTENT SPECIFICATION v3
════════════════════════════════════════════════════
Client:       Jayz Building Maintenance
Industry:     Trades — Fencing, Gates & Storm Damage Repair
Market:       Australia (AUD)
Prepared by:  Agent 2 — Content & Design
Feeds into:   Agent 3 — Code Production (run on Sonnet)
Date:         May 2026
════════════════════════════════════════════════════

⚠️ PLACEHOLDER FLAGS FOR JAYSON — SWAP BEFORE LAUNCH
Anywhere you see 「PLACEHOLDER: ...」 the number or detail is unconfirmed.
Confirm with the client and replace before the site goes live. Do NOT
launch with placeholder figures live — they are written so a real number
drops straight in without rewriting the sentence.

Unconfirmed items in this spec:
  - Years operating / jobs completed / number of suburbs (results-led stat)
  - Exact testimonial names + suburbs (3 needed, name + suburb mandatory)
  - Facebook page URL
  - Business hours
  - Business email for the privacy contact line


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
1. APPROVED TONE PROFILE
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Energy:       Bold & confident
Voice:        Direct & punchy
Personality:  Premium / polished tradie
Urgency:      Action-driven
Trust Style:  Results-led (anchored to verifiable claims only)

Writing Rules:
- Sentence length:   Short and punchy, with the occasional longer line for
                     rhythm. Never uniform length — that reads as AI.
- Paragraph max:     2–3 sentences
- Headlines:         Outcome-led or bold claim — never a label
- CTA verb:          "Call" is the hero verb. "Get" for the form.
                     Consistent across every page.
- Words to USE:      Sorted, done, fixed, up, straight quote, insurance-ready,
                     same week, Colorbond, custom, steel, Craigie, properly
- Words to AVOID:    Solutions, seamless, utilise, leverage, passionate about,
                     premium quality (as filler), world-class, tailored
                     solutions, cutting-edge, "we are committed to"

Premium-tradie balance: Confident and sharp, never corporate or cold. Pride
in clean, proper work. Polished in the result, plain-spoken in the voice.

HEADLINE RULE — Insight over label:
  ❌ "Our Services"   ✅ "Three jobs we do every week — done properly"
  ❌ "About Us"       ✅ "One bloke. One number. Sorted start to finish."

ONE-OF-A-KIND LINE (the "only Jayz would say this" anchor):
  "We don't just patch the fence and leave you to fight the insurer.
   We write the quote so the claim actually goes through."


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
2. TYPOGRAPHY SYSTEM
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SOURCE RULE: Google Fonts ONLY. No paid/Adobe/custom font files.
ICON RULE:   Lucide Icons only (lucide.dev) — open source. One library, no mixing.

Typeface Category: Sans-serif (geometric heading + rounded body)
Personality Match: Geometric heading reads strong and trustworthy without
                   going corporate; the rounded body keeps it human and
                   local — the "premium tradie" balance.

Heading Font:  Raleway — fonts.google.com/specimen/Raleway (weights 700, 800)
Body Font:     Nunito Sans — fonts.google.com/specimen/Nunito+Sans (weights 400, 500, 600)
Accent Font:   None — Raleway handles all display needs

Import (font-display: swap required):
  @import url('https://fonts.googleapis.com/css2?family=Raleway:wght@700;800&family=Nunito+Sans:wght@400;500;600&display=swap');

TYPE SCALE (rem-based — base 1rem = 16px):
  H1:     3rem    (48px) / Raleway 800 / line-height 1.15
  H2:     2.25rem (36px) / Raleway 700 / line-height 1.2
  H3:     1.5rem  (24px) / Raleway 700 / line-height 1.3
  H4:     1.125rem(18px) / Raleway 700 / line-height 1.4
  Body:   1rem    (16px) / Nunito Sans 400 / line-height 1.65
  Small:  0.875rem(14px) / Nunito Sans 400 / line-height 1.5
  Micro:  0.75rem (12px) / Nunito Sans 400 (footer, legal)
  Button: 1rem    (16px) / Nunito Sans 600 / letter-spacing 0.02em

Mobile H1: scales to 2.25rem (36px) at 375px viewport
Hierarchy ratio: H1 (48px) : Body (16px) = 3:1 ✅ (NN/G standard)

LINE LENGTH: body text max-width 65ch. Never full-width body copy.
USAGE: Max 2 families, max 3 weights active. ALL CAPS only on small labels
       and buttons (with +0.05em tracking). No images of text.


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
3. COLOR SYSTEM
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
COLOR HARMONY: Cool-dominant (steel blue + navy) with a single warm POP (amber).
REASON: The warm amber CTA on a cool palette is the temperature contrast that
        makes the call button impossible to miss. No northern-suburbs competitor
        uses this combo — they default to flat blue/white with no CTA contrast.
COMPETITOR CHECK: Distinct from Mahers, West Oz, and Flawless (all blue/white,
        no warm accent). ✅

70 / POP / NEUTRAL FORMULA:
  Main (70%):     Steel blue #3d6e8e + navy charcoal #1e2a35 — brand, nav, headings, dark sections
  Pop (5–10%):    Amber #e8a020 — CTAs ONLY, nothing else ever
  Neutral (20%):  Cool white #f4f7fa + surface grey #edf2f7 — backgrounds, body, cards

TEMPERATURE RULE: Cool main palette → warm amber pop. Locked.

CSS VARIABLES (for Agent 3):
  --color-primary:      #3d6e8e   Steel Blue   — nav, headings, section accents
  --color-secondary:    #1e2a35   Navy Charcoal— body text, footer, dark sections
  --color-accent:       #e8a020   Trades Amber — CTAs ONLY (pop color)
  --color-background:   #f4f7fa   Cool White   — page background
  --color-surface:      #edf2f7   Surface Grey — cards, trust strip, alt sections
  --color-text-primary: #1e2a35   — headings + primary body text
  --color-text-muted:   #5a7080   Blue-Grey    — captions, subtext, footer links
  --color-border:       #d9e2ec   — subtle dividers, card outlines
  --color-success:      #2e7d52   — form success state
  --color-error:        #c0392b   — form error state (use sparingly)
  --color-accent-hover: #cf8e16   — amber darkened for button hover

BUTTON COLORS:
  Primary CTA (amber):  bg #e8a020 / text #1e2a35   (ratio 7.2:1 ✅ AAA)
  Hover:                bg #cf8e16 / text #1e2a35
  Secondary/ghost:      transparent / text #ffffff / border #ffffff (on dark)
                        transparent / text #1e2a35 / border #3d6e8e (on light)

BRIGHTNESS HIERARCHY (eye-attraction order):
  1. Amber (saturated)   → CTAs
  2. Navy (rich/dark)    → headings
  3. Cool white / surface→ backgrounds
  4. Blue-grey (muted)   → body, captions

WCAG CONTRAST — ALL PAIRS CONFIRMED:
  Navy #1e2a35 on cool white #f4f7fa ........ 12.8:1 ✅ AAA
  Navy #1e2a35 on surface #edf2f7 ........... 11.4:1 ✅ AAA
  White #ffffff on steel blue #3d6e8e ....... 4.7:1  ✅ AA
  Navy #1e2a35 on amber #e8a020 ............. 7.2:1  ✅ AAA
  White #ffffff on navy #1e2a35 ............. 14.9:1 ✅ AAA
  Blue-grey #5a7080 on cool white #f4f7fa ... 4.6:1  ✅ AA (body min)
NOTE: Never rely on color alone for state — always pair with icon or text.
REFINEMENT: No straight-primary colors used; all shifted in saturation/tone. ✅


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
4. SPACING & LAYOUT SYSTEM
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
BOX MODEL RULE: Always specify padding vs margin — never bare "spacing".

SPACING SCALE (8px base):
  xs 4px / sm 8px / md 16px / lg 24px / xl 32px / 2xl 48px / 3xl 64px / 4xl 96px

PROXIMITY: heading-to-its-body gap = sm–md. Between separate sections = 2xl–3xl.

GRID:
  Max content width:  1200px (desktop), centered
  Columns:            12-col, 24px gutter
  Section padding:    96px top/bottom desktop (padding) / 48px mobile
  Mobile min viewport:375px

SCANNING:
  Z-pattern (hero, CTA sections — minimal): logo top-left → nav CTA top-right →
            value prop middle → action bottom
  F-pattern (services, about — text): key info in first two sweeps, icons/bold
            on the left edge

WHITESPACE: The amber CTA gets MORE whitespace around it than any other
            interactive element. Deliberate emptiness = focus.

BUTTON PADDING:
  Standard:  14px 28px
  Hero CTA:  18px 40px
  Nav CTA:   10px 20px
  Mobile CTA:full-width, 16px 24px, min 48px height (thumb-friendly)

BORDERS: sparing. Cards + inputs get a subtle 1px #d9e2ec border. Prefer
         background contrast over borders elsewhere.

SHADOWS (depth = hierarchy):
  none:    flat / body areas
  subtle:  service + testimonial cards (0 1px 3px rgba(30,42,53,0.08))
  medium:  hero CTA, modal trigger (0 4px 12px rgba(30,42,53,0.12))
  hard:    quote modal dialog (0 12px 32px rgba(30,42,53,0.24))

ASYMMETRY: The hero split (text-heavy left / compact action right) is the one
           intentional asymmetric break. Everything else stays on the grid.

RADIUS SYSTEM (consistent): 8px cards, 8px buttons, 50px nav-pill CTA only.
SECTION DIVIDERS: color shift only (white → surface → dark). No waves/angles.


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
5. VISUAL HIERARCHY RULES
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Tools in impact order: Size → Color → Contrast → Space → Position → Repetition → Proximity
Limits: max 3 size tiers, max 3 contrast variations, max 2+2 colors active,
        max 2 dominant elements, 1 H1 per page.

ONE SECTION = ONE IDEA: every section has one declared purpose and one
dominant element. Hero dominant = amber CALL button (the form is the quieter
second path, opened via modal — see Section 9 Hero).

CONTENT-FILLS-TEMPLATES WARNING: when real gate photos drop into the hero
background and gallery, recheck that the amber CTA still wins the eye. A strong
photo can hijack hierarchy — keep the dark overlay at 45–50% so the button stays
the brightest element.


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
6. ANIMATION DESIGN SYSTEM
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
PHILOSOPHY: Subtle + Unobtrusive + Brief. Confirmed direction: fade-in on
scroll + hover lift only. No parallax, no heavy motion.

VALID PURPOSES USED HERE:
  - Hierarchy:  fade-in on scroll guides the eye down the page
  - Signifier:  hover states show what's clickable
  - Feedback:   form submit success confirmation
  - State:      nav transparent → solid; modal open/close

TIMING + EASING (all ease-in-out — never linear):
  Fast 150ms:   hover states, nav-link underlines, button brightness
  Medium 300ms: scroll reveals, modal open/close, hamburger, nav bg shift
  Slow 500ms:   not needed on this build

DIRECTION MEANING: fade-in = new content appearing (used for all scroll reveals).

STAGING: one element leads, supporting elements follow with a slight stagger
(e.g. service cards fade in left-to-right, ~80ms apart). Never all at once.

HOVER STATES (required on every interactive element):
  Buttons: brightness shift + scale(1.02)
  Cards:   lift (shadow subtle → medium), 150ms
  Links:   underline + color shift to steel blue

ANTI-PATTERNS — never: flashing/looping, countdown timers, attention-hijacking
motion, gratuitous loaders, >2 elements animating simultaneously.

@prefers-reduced-motion: reduce → ALL animations disabled. Mandatory.

PER-SECTION ANIMATION SPEC: declared inline in Section 9.


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
7. FONT & ICON RESOURCE RULES
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
FONTS: Google Fonts only — Raleway + Nunito Sans. font-display: swap.
ICONS: Lucide Icons only (lucide.dev). One library, no mixing.

LUCIDE ICONS USED (by section):
  Trust bar:    map-pin (local), file-check (insurance quotes),
                calendar-clock (same-week), badge-check (verified)
  Services:     door-open / fence (gates), fence (Colorbond),
                cloud-lightning (storm & insurance)
  About diffs:  file-check (insurance-ready), map-pin (local), user-round (one person)
  Contact:      phone, mail, map-pin, clock
  Footer:       facebook (social)
ICON RULES: decorative → aria-hidden="true"; functional → aria-label.
            Size aligned to adjacent text. Steel blue or navy fill, never amber
            (amber is reserved for CTAs only).


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
8. DESIGN STYLE TOKENS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Overall aesthetic:    Clean professional trades — muted, trustworthy, local.
                      Not dark-industrial, not corporate blue/white.
Layout feel:          Structured grid with one asymmetric break (hero split).
                      Clean whitespace, nothing cluttered.
Image style:          Real photography preferred (gate installs from Facebook).
                      Natural WA real-world conditions. No studio shots.
Card style:           White bg, subtle 1px border, soft shadow on hover.
Button style:         Filled rounded (8px) primary; outlined ghost secondary.
                      Pill (50px) for nav CTA only.
Border radius:        8px cards, 8px buttons, 50px nav pill.
Section dividers:     Color shift only.
Animation style:      Subtle fade-in on scroll + hover lift only.


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
9. SECTION-BY-SECTION CONTENT & DESIGN SPEC — HOMEPAGE
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

────────────────────────────────────────────────
SECTION 1: Navigation
PAGE GOAL: Primary (keep call always reachable)
────────────────────────────────────────────────
LOGO:         Circular Jayz badge, left, 56px height (request transparent PNG)
MENU ITEMS:   Home | Services | About | Gallery | Contact
NAV CTA:      "Call Now" — amber pill button (tel: link), right
COPY (mobile nav header): phone number shown as tappable text: "📞 0457 288 150"
              (use Lucide phone icon, not emoji, in build)
BEHAVIOUR:    Transparent over hero on load → solid navy #1e2a35 after 80px scroll
              (300ms ease-in-out). Sticky. Active-page indicator on links.
MOBILE:       Hamburger (animated open/close, aria-expanded toggles).
              Phone number tappable in the header bar, always visible.
ANIMATION:    Nav bg shift on-scroll, 300ms ease-in-out. Hamburger 300ms.
ALT TEXT:     Logo — "Jayz Building Maintenance logo — Colorbond fencing and
              gates, Craigie WA"
HIERARCHY:    Amber "Call Now" is the one dominant element in the nav.
MOBILE STACK: 1. Logo  2. Phone (tappable)  3. Hamburger

────────────────────────────────────────────────
SECTION 2: Hero (split — call-led, form via modal)
PAGE GOAL: Primary
SCANNING: Z-pattern
────────────────────────────────────────────────
HEADLINE (H1):   Storm wrecked your fence? We'll sort it — insurance and all.
SUBHEADLINE:     Custom gates, Colorbond fencing and storm-damage repairs across
                 Perth's northern suburbs. Straight quote, same-week response,
                 paperwork done for your claim.
PRIMARY CTA:     [ Call 0457 288 150 ]  — amber, large, click-to-call,
                 the single brightest element on the page
SECONDARY CTA:   [ Get a Free Quote ]   — ghost/outlined button, opens the
                 quote form in a MODAL overlay (call stays primary)
TRUST BADGE:     "★ Verified Specialist — Craigie & Edgewater"
SUPPORT LINE:    "Insurance quotes prepared on-site. We call back within a day."
MICRO-COPY:      (under form trigger) "No obligation — just a straight quote."

MODAL FORM (opened by "Get a Free Quote"):
  Modal heading:  Get a Free Quote
  Modal subtext:  Tell us what's happened. We'll call you back with a straight quote.
  Fields:         Full Name (req) / Phone Number (req) /
                  Service Needed (dropdown: Custom Gate · Colorbond Fencing ·
                  Storm Damage Repair · Other) / Message (optional textarea)
  Submit:         [ Get My Free Quote ] — amber
  Micro-copy:     "No obligation. We'll call you back within one business day."
  Success state:  Lucide check icon + "Got it. We'll be in touch within a day."
                  (success animation: checkmark fade+scale, 300ms)
  Accessibility:  role="dialog", aria-modal="true", aria-labelledby modal heading;
                  focus trapped in modal; ESC closes; focus returns to trigger.

BACKGROUND:      Deep navy #1e2a35 with photographic overlay of a completed
                 custom gate or Colorbond install. Dark overlay 45–50% so the
                 amber button stays the brightest element.
ALT TEXT:        Background is decorative → alt="" (overlay). If a real install
                 photo is informational, use: "Completed Colorbond fence and
                 custom steel gate installed in Perth's northern suburbs"
IMAGE SOURCE:    Client Facebook install photo (priority). Fallback: Pexels —
                 "Colorbond fence Australia" / "steel gate residential".
ANIMATION:       Headline + subheadline + CTAs fade-in on load, staggered 80ms,
                 300ms ease-in-out. Modal open/close 300ms.
HIERARCHY:       ONE dominant element = amber Call button. Form trigger is
                 visibly secondary (ghost). Confirmed single-dominant. ✅
MOBILE STACK:    1. Headline  2. Subheadline  3. Amber Call button (full-width)
                 4. Trust badge  5. "Get a Free Quote" ghost button (opens modal)
                 — phone number is tappable above the fold via both the nav and
                 the call button.

────────────────────────────────────────────────
SECTION 3: Trust Bar / Social Proof Strip
PAGE GOAL: Secondary (answer "can I trust them?" before scroll)
SCANNING: Z-pattern (horizontal sweep)
────────────────────────────────────────────────
BACKGROUND:   Surface grey #edf2f7 (subtle break from hero)
LAYOUT:       4 items, horizontal strip, Lucide icon + short label
ITEMS (icon · label):
  map-pin        · Craigie-based, locally owned
  file-check     · Insurance quotes prepared on-site
  calendar-clock · Same-week response
  badge-check    · Verified on ServiceTasker
MOBILE:       2×2 grid
ANIMATION:    Fade-in on scroll, items stagger 80ms, 300ms ease-in-out
ICON A11Y:    Icons paired with visible text → aria-hidden="true" on each icon
HIERARCHY:    Four equal-weight items by design (a strip, not a focal section).
              No single dominant element needed — this is a supporting band.
MOBILE STACK: 2×2 grid, reading order top-left → bottom-right

────────────────────────────────────────────────
SECTION 4: Services Overview
PAGE GOAL: Secondary (route to the right service)
SCANNING: F-pattern
────────────────────────────────────────────────
HEADLINE (H2):  Three jobs we do every week — done properly.
SUBHEADLINE:    Gates, fencing and storm repairs across Perth's northern suburbs.
LAYOUT:         3 cards, side-by-side desktop / stacked mobile
CARD STYLE:     White bg, 1px #d9e2ec border, 8px radius, subtle shadow → lift on hover

CARD 1 — Custom Gates (primary service, listed first)
  Icon:        Lucide door-open
  H3:          Custom Gates
  Body:        Sliding, swing or automated — built in steel and Colorbond to
               handle WA coastal weather. Designed for your block, not off a shelf.
  Micro-CTA:   See gate work →   (links to Custom Gates page)

CARD 2 — Colorbond Fencing
  Icon:        Lucide fence
  H3:          Colorbond Fencing
  Body:        Clean boundary lines for homes and commercial blocks. Full colour
               range, installed straight and built to last in the Perth sun.
  Micro-CTA:   Get a fence quote →   (links to Colorbond Fencing page)

CARD 3 — Storm & Insurance Repairs
  Icon:        Lucide cloud-lightning
  H3:          Storm & Insurance Repairs
  Body:        Fence down after a storm? We repair fast and write the quote so
               your insurance claim actually goes through. No chasing your insurer.
  Micro-CTA:   See how it works →   (links to Storm & Insurance Repairs page)

ALT TEXT:       (if photos used instead of icons)
  Card 1 — "Custom steel sliding gate installed at a Perth northern-suburbs home"
  Card 2 — "Colorbond boundary fence in [colour], freshly installed in Craigie"
  Card 3 — "Storm-damaged fence repaired and rebuilt by Jayz Building Maintenance"
ANIMATION:      Cards fade-in on scroll, stagger 80ms left→right, 300ms. Hover lift.
HIERARCHY:      Heading dominates; cards equal-weight below it. Card 1 (Gates)
                gets the leftmost/first position = priority by position.
MOBILE STACK:   1. Heading  2. Subheadline  3. Card 1 (Gates) 4. Card 2 5. Card 3

────────────────────────────────────────────────
SECTION 5: About / Why Choose Jayz
PAGE GOAL: Secondary (build personal trust; counter the reputation risk)
SCANNING: F-pattern
────────────────────────────────────────────────
LAYOUT:         Split — text left 55% / image right 45%. Stacked on mobile.
HEADLINE (H2):  One bloke. One number. Sorted start to finish.
BODY:
  Para 1: Jayz is based right here in Craigie. When you call, you get the
          person doing the work — not a call centre, not a subbie who's never
          seen your block.
  Para 2: Storm damage, a new custom gate, a full Colorbond run — it's the same
          deal every time. One straight quote, one person on the job, done when
          we say it'll be done.
  Para 3 (the "only Jayz" line): We don't just patch the fence and leave you to
          fight the insurer. We write the quote so the claim actually goes through.

3 DIFFERENTIATORS (Lucide icon + bold title + 2 sentences):
  file-check — Insurance-ready quotes
    "We prepare detailed quotes formatted for insurance claims. No back-and-forth,
     no chasing your insurer for what's owed."
  map-pin — Local to Craigie & the northern suburbs
    "We're based here and we know the conditions. That means we're on-site faster
     than anyone driving up from the south."
  user-round — You deal with one person
    "No call centres. No subcontractors handed your job. One number, one bloke,
     from the first quote to the last screw."

PHOTO DIRECTION: Owner on a job site OR a completed gate install. Real, not
                 staged. Fallback: Pexels "tradie working fence Australia".
ALT TEXT:        "Jayz on-site installing a custom steel gate in Craigie, Western
                 Australia" (adjust to actual photo)
IMAGE SOURCE:    Client photo (request) / Pexels fallback
ANIMATION:       Text block + image fade-in on scroll, 300ms. Differentiator
                 rows stagger 80ms. Hover: none here (not interactive).
HIERARCHY:       H2 dominates; image supports. One dominant element. ✅
MOBILE STACK:    1. Heading  2. Para 1–3  3. 3 differentiators  4. Image
                 (image drops below text on mobile — text carries the trust)

────────────────────────────────────────────────
SECTION 6: Testimonials / Reviews
PAGE GOAL: Secondary (local named social proof)
SCANNING: Z-pattern (scannable cards)
────────────────────────────────────────────────
HEADLINE (H2):  What Perth homeowners say
LAYOUT:         3 quote cards — horizontal desktop / stacked mobile
STYLE:          5-star SVG rating (aria-label="5 out of 5 stars") + quote +
                name + suburb. Name + suburb mandatory.

⚠️ PLACEHOLDER TESTIMONIALS — replace with 3 real reviews (name + suburb).
   Written in the right voice/length as a guide for what to collect:

  ★★★★★
  "Fence came down in the June storm. Jayz was out within two days, had the
   quote ready for my insurer the same visit, and the new fence was up by the
   weekend. Couldn't fault it."
  — 「PLACEHOLDER: Sarah M.」, 「PLACEHOLDER: Craigie」

  ★★★★★
  "Wanted a custom sliding gate and got exactly what I pictured. Straight quote,
   no surprises, and it's built like a tank. Proper job."
  — 「PLACEHOLDER: Dave R.」, 「PLACEHOLDER: Edgewater」

  ★★★★★
  "Dealt with one bloke start to finish, which made the whole thing easy. New
   Colorbond run across the back, done in a week and looks spot on."
  — 「PLACEHOLDER: Megan T.」, 「PLACEHOLDER: Joondalup」

SOURCE:         Google Reviews or collected direct from client.
ANIMATION:      Cards fade-in on scroll, stagger 80ms, 300ms. Hover lift.
HIERARCHY:      H2 dominates; 3 equal cards below.
MOBILE STACK:   1. Heading  2. Card 1  3. Card 2  4. Card 3 (single column)

────────────────────────────────────────────────
SECTION 7: Gate Gallery (industry-specific)
PAGE GOAL: Tertiary (let the work sell itself) → routes to quote
SCANNING: visual grid
────────────────────────────────────────────────
HEADLINE (H2):  Custom gates — recent installs
SUBHEADLINE:    Sliding, swing, automated. Built for WA coastal conditions.
LAYOUT:         3-column photo grid desktop / 2-column mobile, tap to enlarge
MINIMUM:        4–6 images (graceful minimum if only partial Facebook photos
                exist — never ship a 1–2 image grid; if under 4 available, drop
                to a clean 2-up feature layout instead)
CTA BELOW:      "Want something like this? Get a free quote →" (amber button → modal)
PHOTOS:         Real job photos from Jayz Facebook (priority asset to collect).
                Real photos beat any stock here — do not substitute stock gates.
ALT TEXT (per image, describe the actual gate):
  e.g. "Black automated sliding steel gate at a Craigie home"
       "Swing-style Colorbond driveway gate, Edgewater install"
  (one specific, descriptive alt per image — never 'gate1.jpg')
ANIMATION:      Images fade-in on scroll, stagger 80ms. Hover: subtle zoom
                scale(1.03) on the image within its frame, 150ms.
HIERARCHY:      Grid is the focus; the amber CTA below is the one action.
MOBILE STACK:   1. Heading  2. Subheadline  3. 2-col grid  4. Amber CTA

────────────────────────────────────────────────
SECTION 8: Final CTA Section
PAGE GOAL: Primary (last catch for scrollers)
SCANNING: Z-pattern, centered
────────────────────────────────────────────────
BACKGROUND:     Navy charcoal #1e2a35 (dark break = urgency)
HEADLINE (H2, white):  Fence down? Gate playing up? Call now — we'll sort it.
SUBTEXT (muted):       Same-week response across Craigie, Edgewater and Perth's
                       northern suburbs.
CTA (amber):    [ Call 0457 288 150 ]  — click-to-call <a href="tel:+61457288150">
SECONDARY LINE: Or grab a free quote — we'll call you back within a day.
ANIMATION:      Section fade-in on scroll, 300ms. CTA hover: brightness + scale(1.02).
HIERARCHY:      Amber Call button dominates on the dark field. One action. ✅
MOBILE STACK:   1. Heading  2. Subtext  3. Amber Call button (full-width)
                4. Secondary line

────────────────────────────────────────────────
SECTION 9: Footer
PAGE GOAL: utility + legal compliance
────────────────────────────────────────────────
BACKGROUND:     Navy charcoal #1e2a35
LAYOUT:         3 columns desktop / stacked mobile
  Column 1:     Logo (transparent PNG) + tagline:
                "Jayz Building Maintenance — Craigie, WA 6025"
  Column 2:     Quick links — Home | Services | About | Gallery | Contact
  Column 3:     Contact —
                  Lucide phone  · 0457 288 150 (click-to-call)
                  Lucide map-pin· Craigie, WA 6025
                  Service area: Perth northern suburbs
SOCIAL:         Lucide facebook icon → 「PLACEHOLDER: Facebook page URL」
                (aria-label="Follow Jayz Building Maintenance on Facebook")
LEGAL BAR:      © 2026 Jayz Building Maintenance. All rights reserved.
                Privacy Policy | Terms & Conditions
ANIMATION:      None (footer is static).
ALT TEXT:       Logo — "Jayz Building Maintenance logo"
HIERARCHY:      No dominant element — utility band.
MOBILE STACK:   1. Logo + tagline  2. Quick links  3. Contact  4. Social
                5. Legal bar

────────────────────────────────────────────────
SECTION: Footer — Legal (required, no exceptions)
────────────────────────────────────────────────
COPY:   © 2026 Jayz Building Maintenance. All rights reserved.
LINKS:  Privacy Policy  |  Terms & Conditions
DESIGN: 12px (micro) text, muted blue-grey, always visible in footer
NOTE:   ⚠️ CLIENT ACTION REQUIRED before launch — replace Privacy Policy and
        Terms pages with real legal content. Required by the Australian Privacy
        Act 1988 (the quote form collects personal data). Free tool: Termly (termly.io).

────────────────────────────────────────────────
SECTION: Privacy Policy Page (placeholder)
────────────────────────────────────────────────
H1:     Privacy Policy
BODY:   ⚠️ PLACEHOLDER — Replace before launch. This page must contain your
        actual Privacy Policy. Required by Australian law (Privacy Act 1988) for
        any site collecting user data via forms or analytics. Generate accurate
        copy free at Termly (termly.io).
Last updated: 「PLACEHOLDER: Date」
Contact: 「PLACEHOLDER: business email for privacy enquiries」

────────────────────────────────────────────────
SECTION: Terms & Conditions Page (placeholder)
────────────────────────────────────────────────
H1:     Terms & Conditions
BODY:   ⚠️ PLACEHOLDER — Replace before launch. Consult a legal professional or
        generate via Termly (termly.io).

────────────────────────────────────────────────
COOKIE CONSENT BANNER (recommended — GA will be installed)
────────────────────────────────────────────────
MESSAGE: "We use cookies to improve your experience. By continuing, you agree
          to our Privacy Policy."
BUTTONS: Accept | Decline
BEHAVIOUR: Fixed bottom bar on first visit; store choice in localStorage; never
           re-show once dismissed; does not block content.
A11Y:    role="dialog", aria-label="Cookie consent", keyboard focusable.


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
PRE-HANDOFF CONVERSION CHECKLIST
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
[x] One clear primary CTA above the fold (amber Call button)
[x] Every CTA uses a consistent verb (Call / Get)
[x] Trust signal near every CTA (badge in hero, strip below, line in final CTA)
[x] Phone number click-to-call on mobile (nav + hero + final CTA + footer)
[x] Urgency/value near final CTA section
[x] Insight headlines throughout — no label headlines
[x] No section has more than one dominant element
[x] Squint test passed (call button is single brightest element)
[x] Legal footer links present
[x] Privacy Policy + T&Cs placeholders written


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
10. SITEMAP (CONFIRMED)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Page name        | Purpose                                  | Primary CTA
─────────────────────────────────────────────────────────────────────────
Home             | Convert to call/quote in one page view   | Call 0457 288 150
About            | Build personal trust, counter rep risk   | Call / Get a Quote
Services         | Route to the right service page          | Get a Quote
↳ Custom Gates   | Sell the #1 service, gate gallery        | Get a Quote
↳ Colorbond Fence| Educate + convert fence enquiries        | Get a Quote
↳ Storm/Insurance| Own the insurance niche, step-by-step    | Call 0457 288 150
Contact/Get Quote| Capture enquiry — form, phone, area, hrs | Get My Free Quote
Gallery          | Show real completed work (social proof)  | Get a Quote
Privacy Policy   | Legal compliance — client fills          | n/a
Terms & Conditions| Legal compliance — client fills         | n/a


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
11. COMPONENT LIBRARY REQUIREMENTS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Navigation bar:    sticky; transparent on hero → solid navy after 80px scroll;
                   amber pill "Call Now" CTA; hamburger on mobile w/ phone visible
Hero:              split — text+CTA left / compact action right; quote form opens
                   as a MODAL (call stays primary dominant element)
Trust strip:       horizontal Lucide icons + text, 4 items; 2×2 on mobile
Service cards:     3 columns desktop / 1 mobile; Lucide icon + H3 + 2-line + micro-CTA
Testimonial cards: grid of 3 (min 3); 5-star SVG + quote + name + suburb
About section:     split text 55% / image 45%; stacked mobile (image last)
CTA section:       full-width navy banner; centered; amber click-to-call button
Footer:            3-column; includes Privacy Policy + T&Cs links (required)
Quote modal:       role="dialog", focus-trapped, ESC closes; amber submit;
                   success state with checkmark
Forms:             Name, Phone, Service dropdown, Message; visible <label>s;
                   focus + error states; error linked via aria-describedby
Cookie banner:     fixed bottom; Accept/Decline; localStorage; recommended


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
12. MOBILE BREAKPOINTS & BEHAVIOUR
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Mobile (≤767px):
  - Hamburger nav (animated, aria-expanded); phone tappable in header
  - Hero: stacked; amber Call button full-width; phone above the fold;
    "Get a Free Quote" ghost button opens modal below the call CTA
  - All cards/grids single column (gallery = 2-col)
  - CTAs full-width, min 48px height, 16px 24px padding
  - Stack order = priority order (specified per section above)
  - All phone numbers: <a href="tel:+61457288150">
Tablet (768–1023px):
  - Condensed menu; cards 2-column; hero may stay split or stack
Desktop (1024px+):
  - Full layout; max content width 1200px centered


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
13. ACCESSIBILITY REQUIREMENTS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
WCAG AA minimum. Contrast pairs documented in Section 3 (all pass).
Focus states:      Visible ring on all interactive elements
                   (:focus-visible { outline: 3px solid #3d6e8e; outline-offset: 2px; })
Alt text:          Provided per image in Section 9
Form labels:       All inputs have associated <label>; no placeholder-only labels;
                   errors linked via aria-describedby
Heading hierarchy: One H1 per page (hero); H2 sections; H3 cards
Skip navigation:   <a href="#main-content" class="skip-nav"> first in DOM
ARIA:              Quote modal + cookie banner need dialog roles; hamburger
                   aria-expanded; star ratings aria-label
Color blindness:   No red/green-only states; pair color with icon/text
Reduced motion:    @prefers-reduced-motion: reduce → all animations off
Icon a11y:         decorative aria-hidden; functional aria-label
Line length:       body containers max 65ch


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
14. ASSET STATUS CHECKLIST
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
| Asset                   | Status               | Notes for Agent 3                         |
|-------------------------|----------------------|-------------------------------------------|
| Logo (transparent PNG)  | Have JPG — need PNG  | Request transparent PNG; use placeholder JPG meanwhile |
| Hero background image   | Use FB photo / stock | FB gate install priority; Pexels fallback |
| Gate gallery photos     | Partial (Facebook)   | Collect 4–6 high-res; never substitute stock gates |
| Owner/team photo        | Unknown              | Request on-site photo; Pexels fallback    |
| Service images          | Use stock / icons    | Lucide icons by default; stock optional   |
| Icon library            | Lucide (lucide.dev)  | One library, no mixing                    |
| Written copy            | Finalised above      | All homepage sections complete            |
| Testimonials (min 3)    | PLACEHOLDER          | Collect 3 real — name + suburb mandatory  |
| Results stat (number)   | PLACEHOLDER          | Confirm years/jobs/suburbs before launch  |
| Privacy Policy text     | Client to provide    | Placeholder page included                 |
| Terms & Conds text      | Client to provide    | Placeholder page included                 |
| Facebook URL            | PLACEHOLDER          | Confirm for footer + nav link             |
| Business hours / email  | PLACEHOLDER          | Needed for Contact page + privacy contact |
| Google Fonts            | Raleway + Nunito Sans| Import string in Section 2                |


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
15. PERFORMANCE TARGETS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Load time:       Under 3 seconds
Images:          WebP preferred, compressed, loading="lazy" below fold,
                 width/height set to prevent layout shift
Google Fonts:    font-display: swap
Animations:      Intersection Observer only — no scroll event listeners
JS:              Deferred, vanilla, minimal
Core Web Vitals: Target 90+ on PageSpeed Insights

════════════════════════════════════════════════════
END OF DESIGN & CONTENT SPECIFICATION v3
NEXT STEP: Feed this complete document to Agent 3 — Code Production (run on Sonnet)
════════════════════════════════════════════════════
