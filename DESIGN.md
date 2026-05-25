---
name: CARAVAN
description: The digital trade route for fresh produce. RFQ-based trading infrastructure for growers, exporters and buyers.
colors:
  caravan-amber: "#C8922A"
  amber-bright: "#E0A83A"
  midnight-navy: "#0B1220"
  navy-raised: "#111D30"
  navy-overlay: "#1A2A42"
  trade-cream: "#EEE8DC"
  text-muted: "#EEE8DC99"
  text-muted-strong: "#EEE8DCBF"
  faint: "#EEE8DC14"
  hairline: "#EEE8DC24"
  deal-green: "#0F6E56"
  deal-green-wash: "#E1F5EE"
  status-live: "#4ADE80"
  status-logged: "#1D9E75"
  status-demand: "#378ADD"
  alert-red: "#E24B4A"
typography:
  display:
    fontFamily: "Barlow Condensed, sans-serif"
    fontSize: "clamp(42px, 6vw, 80px)"
    fontWeight: 800
    lineHeight: 0.96
    letterSpacing: "0.01em"
  headline:
    fontFamily: "Barlow Condensed, sans-serif"
    fontSize: "clamp(38px, 5.5vw, 68px)"
    fontWeight: 800
    lineHeight: 1.02
    letterSpacing: "0.02em"
  title:
    fontFamily: "Barlow Condensed, sans-serif"
    fontSize: "26px"
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: "0.04em"
  body:
    fontFamily: "Barlow, sans-serif"
    fontSize: "clamp(15px, 1.4vw, 18px)"
    fontWeight: 300
    lineHeight: 1.65
    letterSpacing: "normal"
  label:
    fontFamily: "DM Mono, ui-monospace, monospace"
    fontSize: "10px"
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: "0.3em"
rounded:
  none: "0px"
  sm: "4px"
  md: "6px"
  panel: "10px"
spacing:
  xs: "6px"
  sm: "12px"
  md: "16px"
  lg: "24px"
  xl: "36px"
  gutter: "40px"
  section: "96px"
components:
  button-primary:
    backgroundColor: "{colors.caravan-amber}"
    textColor: "{colors.midnight-navy}"
    typography: "{typography.label}"
    rounded: "{rounded.none}"
    padding: "14px 24px"
  button-primary-hover:
    backgroundColor: "{colors.amber-bright}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.trade-cream}"
    typography: "{typography.label}"
    rounded: "{rounded.none}"
    padding: "14px 24px"
  button-ghost-hover:
    textColor: "{colors.caravan-amber}"
  input-field:
    backgroundColor: "#EEE8DC0A"
    textColor: "{colors.trade-cream}"
    rounded: "{rounded.none}"
    padding: "11px 14px"
  pill:
    textColor: "{colors.caravan-amber}"
    rounded: "{rounded.none}"
    padding: "4px 9px"
    typography: "{typography.label}"
  toggle-segment:
    backgroundColor: "{colors.navy-raised}"
    textColor: "{colors.text-muted}"
    rounded: "{rounded.sm}"
    padding: "8px 18px"
  toggle-segment-active:
    backgroundColor: "#C8922A1A"
    textColor: "{colors.caravan-amber}"
  usp-row:
    backgroundColor: "{colors.navy-raised}"
    textColor: "{colors.trade-cream}"
    rounded: "{rounded.sm}"
    padding: "24px 28px"
  usp-row-hover:
    backgroundColor: "{colors.navy-overlay}"
  nav-bar:
    backgroundColor: "#0B1220EB"
    textColor: "{colors.text-muted-strong}"
---

# Design System: CARAVAN

## 1. Overview

**Creative North Star: "The Digital Trade Route"**

CARAVAN is amber waypoints on a navy expanse. The brand's own origin story is the design brief: before roads, ports or exchanges there were caravans, merchants crossing fragmented terrain together, sharing intelligence, pooling trust, reaching markets none could reach alone. The interface is that route made legible. A dark, lantern-lit field (Midnight Navy) carries warm signal points (Caravan Amber) that mark where a deal is forming. Structure is imposed on chaos through hairline rules, ordered columns, and a live blotter you can trust.

The voice is precise, warm, and institutional. Quant-grade rigor shows up as sharp 0px corners, 1px hairline dividers, and monospace tracked labels, the grammar of a trading desk. The warmth comes from the palette: cream text instead of stark white, gold instead of clinical green, a night canvas that reads considered rather than cold. Density is editorial, not cramped: 96px section rhythm, generous gutters, one dominant idea per fold, long deliberate scroll. The page is bilingual (English and Dutch) and every motion respects `prefers-reduced-motion`.

This system explicitly rejects four reflexes. It is not cold bank-fintech navy-and-gold (the warmth and the condensed display type pull it elsewhere). It is not sterile SaaS with rounded cards and icon-title-subtitle grids. It is not leafy agri-tech green (green is reserved strictly for "deal done"). And it is never startup-purple gradients or decorative glassmorphism.

**Key Characteristics:**
- Dark, warm canvas: Midnight Navy ground, Trade Cream type, never pure black or white.
- One committed accent: Caravan Amber carries identity, signal, and call-to-action.
- Square by default: 0px corners, 1px hairlines, tonal navy layering instead of shadows.
- Monospace tracked labels (DM Mono, uppercase, 0.2em+) as connective tissue, prefixed by a 28px amber rule.
- Condensed display type (Barlow Condensed 800) at large fluid sizes for headline drama.
- Motion is purposeful and reversible: staggered entrance, press feedback, live pulses, full reduced-motion support.

## 2. Colors

A nocturnal, warm palette: one gold accent and one green outcome color carried across a layered navy ground, with cream as the only "light."

### Primary
- **Caravan Amber** (#C8922A): The brand's single voice. Carries the logo, eyebrows and section kickers, primary buttons, the live-market pulse, RFQ highlights, prices, and the focus ring. It is signal and identity at once.
- **Amber Bright** (#E0A83A): The lit state. Used only on hover of amber surfaces (primary button, submit) and on the "best quote" price. A half-step brighter, never a second accent.

### Secondary
- **Deal Green** (#0F6E56): Outcome, not decoration. Reserved for a confirmed, logged deal and the buyer-initiated flow in the protocol diagram. Its rarity is what makes "green" mean "done."
- **Deal Green Wash** (#E1F5EE): The pale green fill behind a completed-deal node in the SVG diagrams.

### Tertiary
Status vocabulary for the live blotter only. These are functional state colors, never brand colors, and must not leak into page chrome.
- **Status Live** (#4ADE80): Available supply, a live/new RFQ row.
- **Status Logged** (#1D9E75): A recorded deal price in history.
- **Status Demand** (#378ADD): "Open demand" counterparties.
- **Alert Red** (#E24B4A): Urgent countdown under 30 seconds, and form errors. The only red in the system.

### Neutral
- **Midnight Navy** (#0B1220): The page ground and the theme color. Everything sits on this.
- **Navy Raised** (#111D30): The first layer up: cards, USP rows, the demo panel body, inputs.
- **Navy Overlay** (#1A2A42): The second layer up: table chrome, the mock browser title bar, USP row hover.
- **Trade Cream** (#EEE8DC): The only light. All primary text. Never `#ffffff`.
- **Text Muted** (#EEE8DC99, cream at 0.6) and **Text Muted Strong** (#EEE8DCBF, cream at 0.75): Secondary copy, leads, captions, nav links at rest.
- **Hairline** (#EEE8DC24, cream at 0.14) and **Faint** (#EEE8DC14, cream at 0.08): Borders and the 1px grid gaps that draw dividers. The structural ink of the whole system.

### Named Rules
**The One Voice Rule.** Caravan Amber is the only accent. It may appear often, but it is never joined by a second decorative hue. Green and the status colors are outcomes and states, not accents; they earn their place by meaning something.

**The Warm Neutral Rule.** Pure `#000` and `#fff` are forbidden. The ground is Midnight Navy, the light is Trade Cream, and every grey is cream at reduced alpha. If a neutral looks blue-grey or stark white, it is wrong.

**The Green-Means-Done Rule.** Green is reserved for a confirmed, logged, or accepted trade. Never use it for navigation, emphasis, or general "success" chrome.

## 3. Typography

**Display Font:** Barlow Condensed (sans-serif fallback), weights 300 to 800.
**Body Font:** Barlow (sans-serif fallback), weights 300 to 600, body set at 300.
**Label / Mono Font:** DM Mono (ui-monospace fallback), weights 300 to 500.

**Character:** A condensed grotesque carries the drama, a humanist sans carries the argument, and a mono carries the machinery. The pairing reads as a confident trading desk: big tight headlines, light readable prose, and tracked monospace labels that feel like terminal output. The one expressive move is the hero subhead: Barlow Condensed italic in Caravan Amber.

### Hierarchy
- **Display** (Barlow Condensed 800, clamp(42px, 6vw, 80px), line-height 0.96, tracking 0.01em): The hero headline and the contact headline (which scales to clamp(48px, 7vw, 88px)). One per fold, maximum.
- **Subhead** (Barlow Condensed 400 italic, clamp(24px, 3vw, 40px), amber): The single italic flourish, directly under the hero headline. Used sparingly.
- **Headline** (Barlow Condensed 800, clamp(38px, 5.5vw, 68px), line-height 1.02, tracking 0.02em): Section titles.
- **Title** (Barlow Condensed 700, 26px, tracking 0.04em; founder names at 34px/800): Problem tiles, USP rows, founder cards.
- **Body** (Barlow 300, clamp(15px, 1.4vw, 18px) for leads, 13px to 16px for copy, line-height 1.65): All prose. Capped at roughly 65 to 75ch via `max-width` 560px to 640px.
- **Label** (DM Mono 400, 9px to 11px, tracking 0.15em to 0.3em, UPPERCASE): Eyebrows, section kickers, nav links, meta, pills, table headers, button text.

### Named Rules
**The Tracked Kicker Rule.** Section and hero kickers are DM Mono, uppercase, tracked 0.3em, in Caravan Amber, and prefixed by a 28px x 1px amber rule via `::before`. This is the system's signature label, deliberate and consistent, not scattered decoration.

**The Condensed-Display Rule.** Large headings are always Barlow Condensed at weight 800 with tight line-height (under 1.02). A flat scale or a non-condensed display face breaks the voice. Steps stay at a 1.25+ ratio; no timid sizing.

**The Light-Body Rule.** Body copy is weight 300 on the dark ground. Light type on dark needs the air, hence line-height 1.65 and capped measure. Do not bump body to 400+ to "fix" legibility; fix contrast and measure instead.

## 4. Elevation

The system is flat by default and builds depth through tonal layering, not shadow. Surfaces step up by hue (Midnight Navy to Navy Raised to Navy Overlay) and are separated by 1px hairlines. The one exception is the floating product demo, which earns a single dramatic shadow to read as a screen lifted above the page. Glassmorphism is forbidden as decoration; the one blur in the system is the sticky nav's functional backdrop-filter.

### Shadow Vocabulary
- **Floating panel** (`box-shadow: 0 32px 72px -20px rgba(0,0,0,0.7)`): The animated RFQ demo browser only. A deep, soft, downward shadow that lifts the product mock off the navy ground.
- **Toast** (`box-shadow: 0 8px 24px rgba(0,0,0,0.5)`): The Outlook-style notification that slides in inside the demo. Tighter and shallower than the panel.
- **Nav backdrop** (`backdrop-filter: blur(16px)` over `#0B1220EB`): Functional, not decorative. Keeps content legible as it scrolls under the sticky bar.

### Named Rules
**The Flat-By-Default Rule.** Page surfaces are flat. Depth comes from the three-step navy tonal ramp and 1px hairlines. Shadow is reserved for elements that are literally floating (the demo, the toast). If a card has a drop shadow at rest, it is wrong.

**The Hairline Grid Rule.** Dividers are drawn by 1px gaps, not borders on each child: a grid with `gap: 1px` over a hairline background, with each tile painted in the ground color. This is how the problem grid and founders grid get their clean rules.

## 5. Components

### Buttons
- **Shape:** Hard rectangles (0px radius). Mono uppercase label, tracking 0.2em, with an inline `→` arrow that slides 3px right on hover.
- **Primary:** Caravan Amber fill, Midnight Navy text, padding 14px 24px. Hover lightens to Amber Bright (#E0A83A).
- **Ghost:** Transparent fill, Trade Cream text, 1px hairline border. Hover shifts border and text to Caravan Amber.
- **Press:** All pressables scale to 0.97 on `:active` for tactile feedback.
- **Focus:** A 2px Amber Bright `:focus-visible` outline, offset 3px. Never removed without this replacement.

### Chips and Tags
- **Pills (founder credentials):** Mono uppercase 9px, Caravan Amber text, 1px amber border at 0.4 alpha, square. No fill.
- **Status badges (blotter):** Mono uppercase, tiny, tinted background plus a matching 1px border, color-keyed to the Tertiary status palette. Live, Quoted, Logged, Future, Open demand each have a fixed color.

### Cards and Containers
- **Corner style:** USP rows and the demo panel use small radii (4px to 10px); problem tiles and founder cards are square (0px) and separated by the hairline grid.
- **Background:** Navy Raised (#111D30) for cards on the navy ground.
- **Shadow strategy:** None at rest (see Elevation). USP rows respond to hover by stepping to Navy Overlay (#1A2A42).
- **Border:** 1px hairline.
- **Internal padding:** 24px to 40px depending on density (USP rows 24px 28px, founder cards 40px 36px).

### Inputs and Fields
- **Style:** Cream-at-0.04 fill, 1px cream-at-0.1 border, 0px radius, Barlow 300 at 14px. Placeholder is cream at 0.42.
- **Focus:** Border shifts to amber at 0.5 alpha, plus the system focus ring on keyboard focus (offset 0 on inputs so the ring hugs the field).
- **Labels:** Mono uppercase amber kicker above each field; required marked with an amber asterisk, optional marked with a quiet mono note.
- **States:** Submit shows a sending label and disables; success swaps the form for a confirmation block; errors render in Alert Red with a recovery email address.

### Navigation
- **Style:** Sticky top bar, `#0B1220EB` with a 16px backdrop blur, 1px faint bottom border.
- **Typography:** DM Mono uppercase 10px links, tracking 0.18em, Text Muted Strong at rest, Caravan Amber on hover (pointer devices only).
- **Language toggle:** A segmented EN / NL control; the active segment is Caravan Amber fill with Midnight Navy text.
- **Mobile:** Links collapse into a burger that opens a full-width dropdown; hover effects are gated behind `(hover: hover)` so taps do not stick.

### Signature: The RFQ Demo and Protocol Diagrams
- **Animated demo browser:** A macOS-style window (10px radius, floating-panel shadow) running a scripted, perspective-switchable (sell side / buy side) walkthrough of the platform: upload, counterparty select, live countdown, streaming quotes, confirmed deal, email toast. It includes a simulated cursor and click rings. It is marked `aria-hidden`; its narrative lives in the visible step captions, and it pauses when scrolled out of view and under reduced motion.
- **Protocol diagrams:** Two inline SVGs (grower-initiated in amber, buyer-initiated in green) that loop through send, collect, and execute phases with animated dashed flow lines and pulsing origin nodes.

## 6. Do's and Don'ts

### Do:
- **Do** keep Caravan Amber (#C8922A) as the only accent. Promote to Amber Bright (#E0A83A) for hover, never for a new role.
- **Do** build depth with the three-step navy ramp and 1px hairlines. Draw dividers with `gap: 1px` over a hairline background.
- **Do** use sharp 0px corners on buttons, inputs, tiles, and pills. Reserve the small 4px to 10px radii for USP rows and the demo panel only.
- **Do** prefix section and hero kickers with the 28px amber rule and set them in DM Mono uppercase, tracked 0.3em.
- **Do** reserve green for a confirmed or logged deal, and red only for sub-30-second urgency and form errors.
- **Do** keep the 2px Amber Bright `:focus-visible` ring on every interactive element, and keep all motion behind `prefers-reduced-motion`.
- **Do** cap body measure at 65 to 75ch and keep body weight at 300 on the dark ground.

### Don't:
- **Don't** drift into cold bank-fintech navy-and-gold, sterile SaaS card grids, or leafy agri-tech green. Green is an outcome, not a brand color.
- **Don't** introduce startup-purple gradients, gradient text (`background-clip: text`), or decorative glassmorphism. The only blur is the nav backdrop.
- **Don't** use `#000` or `#fff`. Ground is Midnight Navy, light is Trade Cream, greys are cream at reduced alpha.
- **Don't** put drop shadows on resting cards. Shadow belongs only to elements that are literally floating (the demo panel, the toast).
- **Don't** use a colored `border-left` or `border-right` over 1px as a stripe accent on page chrome. (Inside the faithful Outlook mock, the blue accent is a reproduction of a real product, not a CARAVAN pattern.)
- **Don't** soften the geometry with rounded cards or set large headings in a non-condensed face. Condensed Barlow at 800 is the headline voice.
- **Don't** scatter mono tracked labels as generic decoration. The amber-ruled kicker is a deliberate, single system, not a stamp for every block.
