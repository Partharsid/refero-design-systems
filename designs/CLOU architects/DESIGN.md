# CLOU architects — Style Reference
> ink on cream paper

**Theme:** light

CLOU architects operates in a radical two-color universe: warm cream (#fffffc) and absolute black (#000000). Nothing else is allowed in the interface — every other hue comes from architectural photography bleeding into the layout. The system is built on one geometric sans-serif (Circular Std) pushed to extremes: headlines reach 200px+, letter-spacing tightens aggressively at scale, and line-heights compress to 0.80 for display copy. The cream background is deliberately off-white (not #ffffff), which prevents harshness against the dominant black typography and gives the page a paper-like, gallery-wall warmth. Navigation is a dense black bar; the body is expansive cream; the only &quot;decoration&quot; is the photography itself — full-bleed, unframed, the actual project. This is a design system that says almost nothing visually so the architecture can say everything.

## Tokens — Colors

| Name | Value | Token | Role |
|------|-------|-------|------|
| Cream Paper | `#fffffc` | `--color-cream-paper` | Page canvas, card surfaces, button fills — the slightly warm off-white prevents stark contrast against black ink, giving the entire site a printed-paper warmth rather than a digital-screen feel |
| Ink Black | `#000000` | `--color-ink-black` | All text, borders, navigation background, button borders, icon strokes — the only foreground color in the system, used at full saturation with no opacity reductions |

## Tokens — Typography

### Circular Std — Sole typeface for all UI and editorial text. Used at 400 for body, nav, and captions; 700 for emphasis and display-level statements. The display sizes (109–201px) with tightened tracking and 0.80 line-height create headlines that function as architectural objects — each word occupies physical space, almost like load-bearing elements. · `--font-circular-std`
- **Substitute:** Inter, Geist, General Sans
- **Weights:** 400, 700
- **Sizes:** 13, 17, 20, 25, 32, 34, 50, 109, 134, 166, 201px
- **Line height:** 0.80, 1.00, 1.06, 1.10, 1.15, 1.50
- **Letter spacing:** -0.07em at 201px, -0.05em at 166px, -0.03em at 109–134px, -0.012em at 50px, -0.01em at 32–34px
- **Role:** Sole typeface for all UI and editorial text. Used at 400 for body, nav, and captions; 700 for emphasis and display-level statements. The display sizes (109–201px) with tightened tracking and 0.80 line-height create headlines that function as architectural objects — each word occupies physical space, almost like load-bearing elements.

### Type Scale

| Role | Size | Line Height | Letter Spacing | Token |
|------|------|-------------|----------------|-------|
| caption | 13px | 1.5 | — | `--text-caption` |
| body-sm | 17px | 1.5 | — | `--text-body-sm` |
| body | 20px | 1.5 | — | `--text-body` |
| subheading | 25px | 1.15 | — | `--text-subheading` |
| heading-sm | 34px | 1.1 | -0.34px | `--text-heading-sm` |
| heading | 50px | 1.06 | -0.6px | `--text-heading` |
| heading-lg | 109px | 1 | -3.27px | `--text-heading-lg` |
| display | 134px | 1 | -4.02px | `--text-display` |
| display-lg | 166px | 0.8 | -8.3px | `--text-display-lg` |
| display-xl | 201px | 0.8 | -14.07px | `--text-display-xl` |

## Tokens — Spacing &amp; Shapes

**Density:** comfortable

### Spacing Scale

| Name | Value | Token |
|------|-------|-------|
| 5 | 5px | `--spacing-5` |
| 8 | 8px | `--spacing-8` |
| 10 | 10px | `--spacing-10` |
| 11 | 11px | `--spacing-11` |
| 13 | 13px | `--spacing-13` |
| 17 | 17px | `--spacing-17` |
| 25 | 25px | `--spacing-25` |
| 50 | 50px | `--spacing-50` |
| 59 | 59px | `--spacing-59` |
| 84 | 84px | `--spacing-84` |
| 101 | 101px | `--spacing-101` |
| 134 | 134px | `--spacing-134` |
| 168 | 168px | `--spacing-168` |
| 174 | 174px | `--spacing-174` |

### Border Radius

| Element | Value |
|---------|-------|
| tags | 0px |
| cards | 0px |
| inputs | 0px |
| buttons | 0px |

### Shadows

| Name | Value | Token |
|------|-------|-------|
| subtle | `rgb(0, 0, 0) 0px 0px 0px 1px` | `--shadow-subtle` |

### Layout

- **Page max-width:** 1440px
- **Section gap:** 84px
- **Card padding:** 25px
- **Element gap:** 17px

## Components

### Black Navigation Bar
**Role:** Top-level site navigation

Full-bleed black bar (#000000) with cream text (#fffffc). Logo on far left, nav links left-aligned beside it, language switcher right-aligned. Padding approximately 17px vertical, 25px horizontal. Links use 17px Circular Std at weight 400; active/hovered links get a 1px cream underline (visible on &#x27;Info&#x27; in screenshots). Height tight — no generous padding, the bar is a strip not a panel.

### Display Headline
**Role:** Hero and section-opening statements

Circular Std weight 400 at 134–201px, line-height 0.80–1.00, letter-spacing -3 to -14px depending on size. Color #000000 on cream. No italic, no all-caps, no decoration — the size and weight contrast do all the work. Period at the end is a signature punctuation choice (e.g. &#x27;We do social space.&#x27;).

### Body Text Block
**Role:** Paragraphs and descriptive copy

Circular Std weight 400 at 20px, line-height 1.50, color #000000 on cream. Left-aligned, no first-line indent, no hyphenation. Generous left margin (up to 59px) to create a text column that doesn&#x27;t stretch full-width. Line-length is intentionally short to feel like editorial print rather than web copy.

### Underlined Nav Link
**Role:** Active or hovered navigation item

17px Circular Std weight 400, cream (#fffffc) on black nav bar, with a 1px cream underline directly beneath the text. Underline is flush with baseline, no gap, no offset — a printer&#x27;s mark rather than a CSS border.

### Outlined Action Button
**Role:** Primary or secondary actions (no filled variant exists)

Circular Std weight 400 at 17px, text #000000, 1px solid #000000 border, background #fffffc. Padding 17px horizontal by ~8px vertical. Radius 0px — no rounding. No fill state, no shadow, no gradient. The button is a frame, not a block.

### Full-Bleed Project Image
**Role:** Architectural photography display

No frame, no border, no caption, no background card. The image extends edge-to-edge within its container, with only its inherent content providing color. No rounded corners (radius 0). Aspect ratio varies by project but is always wide (landscape). The image carries the entire emotional and chromatic weight of the page.

### Language Switcher
**Role:** Localized language toggle

Top-right of nav bar, 13px Circular Std weight 400, cream on black. Format: &#x27;En / 中文&#x27; with a forward slash separator. No dropdown — always visible as a flat text toggle.

### Logo Mark
**Role:** Brand identifier in nav

&#x27;CLOU&#x27; wordmark, 17px Circular Std weight 700, cream on black nav. No icon mark — pure typography, uppercase, tight tracking.

### Section Divider
**Role:** Visual separation between content blocks

No explicit divider. Separation is achieved by the 84px vertical gap between blocks and the alternating image/text rhythm. The cream background is continuous — no background color changes between sections.

## Do&#x27;s and Don&#x27;ts

### Do
- Use #fffffc for all page backgrounds and #000000 for all text, borders, and icons — the system is strictly two-color
- Set display headlines at 109px+ with letter-spacing between -0.03em and -0.07em and line-height 0.80–1.00 to match the architectural-typography attitude
- Use weight 400 for body and display alike; reserve weight 700 only for the logo and strong emphasis
- Let photographs run full-bleed with no borders, rounded corners, or background cards — radius must be 0 across all components
- Maintain 84px vertical rhythm between major sections and 17–25px for inline element spacing
- End display statements with a period for a declarative, finished tone (&#x27;We do social space.&#x27;)
- Use the outlined button (1px #000000 border on #fffffc fill) for any clickable action — never add a filled black button

### Don&#x27;t
- Never introduce a third color into the interface — all chromatic content must come from project photography
- Don&#x27;t use pure #ffffff for backgrounds — the slight warmth of #fffffc is the entire mood
- Don&#x27;t apply border-radius to any element; the system is strictly orthogonal
- Don&#x27;t reduce opacity on black to create gray tones — use the real black or don&#x27;t use the color at all
- Don&#x27;t set display headlines at smaller than 109px — sub-display sizes (50–90px) break the editorial scale
- Don&#x27;t add drop shadows beyond the occasional 1px solid border — the design is flat, not elevated
- Don&#x27;t use all-caps for body or display text; sentence case with terminal period is the system&#x27;s voice

## Surfaces

| Level | Name | Value | Purpose |
|-------|------|-------|---------|
| 1 | Cream Paper | `#fffffc` | Page canvas, the default background for all body content |
| 2 | Ink Black | `#000000` | Navigation bar and any inverted surface — the only dark surface in the system |

## Imagery

Photography is the only color in the system and occupies the dominant visual space. All imagery is real architectural photography — interiors, exteriors, and building details — shot in available light with no post-production color grading or filter treatment. Images run full-bleed edge-to-edge with zero border, no rounded corners, and no background card. There are no illustrations, no abstract graphics, no icons beyond a minimal set of small UI glyphs (arrow, close), and no decorative elements. The only &#x27;imagery style&#x27; is documentary architectural photography at the highest possible resolution, allowed to fill the viewport and introduce its own palette of reds, blues, greens, and warm light into an otherwise monochrome page.

## Layout

Max-width 1440px centered, though hero and full-bleed images escape the constraint. The page follows a vertical-scroll editorial model: black nav strip at top, a display-headline hero, then a repeating rhythm of full-bleed image followed by short body-text block followed by next image. Text columns are narrow (left-aligned, max ~600px) and sit to the left, while images span the full width. No card grids, no multi-column feature blocks, no pricing tables. Sections are separated by whitespace (84px) rather than dividers or alternating backgrounds. The layout reads like a printed architecture monograph — one statement, one image, one statement, one image.

## Agent Prompt Guide

**Quick Color Reference**
- text: #000000
- background: #fffffc
- border: #000000
- accent: none
- primary action: no distinct CTA color

**Example Component Prompts**
1. *Display headline*: &#x27;Build bold spaces.&#x27; in Circular Std weight 400, size 166px, line-height 0.80, letter-spacing -8.3px, color #000000 on #fffffc canvas. End with a period.
2. *Outlined button*: Text &#x27;View Project&#x27; in Circular Std weight 400, 17px, #000000, inside a 1px solid #000000 border on #fffffc fill, padding 8px 17px, radius 0px.
3. *Navigation bar*: Full-bleed #000000 bar, 17px vertical padding, 25px horizontal. Left: &#x27;CLOU&#x27; in Circular Std weight 700, 17px, #fffffc. Beside it: &#x27;Projects  Info  Contact&#x27; in weight 400, 17px, #fffffc, with the active item underlined 1px. Right: &#x27;En / 中文&#x27; in 13px, #fffffc.
4. *Body paragraph*: &#x27;Combining smart creativity with commercial savvy, we take our clients&#x27; challenges and transform them into exceptionally innovative design.&#x27; in Circular Std weight 400, 20px, line-height 1.50, #000000, max-width ~480px, left-aligned with 59px left margin.
5. *Full-bleed project image*: A landscape architectural photograph, no border, no radius, no caption, spanning the full viewport width at its native aspect ratio.

## Typography Philosophy

Circular Std is the entire voice of the system. The type scale is not gradual — it is editorial: body lives at 17–25px, then jumps directly to 50px for secondary headings, and then leaps to 109–201px for display. This is a scale designed for a magazine spread, not a dashboard. The very tight letter-spacing at large sizes (-0.07em at 201px) is what makes a 201px headline not feel like a logo — the letters pull toward each other to create a solid mass of ink. The 0.80 line-height at display sizes allows lines to almost touch, creating dense typographic blocks. Weight is binary: 400 is the default, 700 is used only for the wordmark and rare emphasis. This restraint means when 700 appears, it carries disproportionate weight.

## Similar Brands

- **Herzog &amp; de Meuron** — Same radical two-color editorial layout with massive display sans-serif headlines and full-bleed architectural photography as the sole source of color
- **Pentagram** — Same monochrome (often black-on-white) page architecture where typography carries the entire brand and photography is left unframed
- **OMA / Rem Koolhaes** — Same typographic maximalism — oversized display headlines with tight tracking, zero border-radius, and large white-space between sparse content blocks
- **Snøhetta** — Same quiet cream/off-white canvas with full-bleed project photography and minimal navigation chrome

## Quick Start

### CSS Custom Properties

```css
:root {
  /* Colors */
  --color-cream-paper: #fffffc;
  --color-ink-black: #000000;

  /* Typography — Font Families */
  --font-circular-std: &#x27;Circular Std&#x27;, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, &quot;Segoe UI&quot;, Roboto, sans-serif;

  /* Typography — Scale */
  --text-caption: 13px;
  --leading-caption: 1.5;
  --text-body-sm: 17px;
  --leading-body-sm: 1.5;
  --text-body: 20px;
  --leading-body: 1.5;
  --text-subheading: 25px;
  --leading-subheading: 1.15;
  --text-heading-sm: 34px;
  --leading-heading-sm: 1.1;
  --tracking-heading-sm: -0.34px;
  --text-heading: 50px;
  --leading-heading: 1.06;
  --tracking-heading: -0.6px;
  --text-heading-lg: 109px;
  --leading-heading-lg: 1;
  --tracking-heading-lg: -3.27px;
  --text-display: 134px;
  --leading-display: 1;
  --tracking-display: -4.02px;
  --text-display-lg: 166px;
  --leading-display-lg: 0.8;
  --tracking-display-lg: -8.3px;
  --text-display-xl: 201px;
  --leading-display-xl: 0.8;
  --tracking-display-xl: -14.07px;

  /* Typography — Weights */
  --font-weight-regular: 400;
  --font-weight-bold: 700;

  /* Spacing */
  --spacing-5: 5px;
  --spacing-8: 8px;
  --spacing-10: 10px;
  --spacing-11: 11px;
  --spacing-13: 13px;
  --spacing-17: 17px;
  --spacing-25: 25px;
  --spacing-50: 50px;
  --spacing-59: 59px;
  --spacing-84: 84px;
  --spacing-101: 101px;
  --spacing-134: 134px;
  --spacing-168: 168px;
  --spacing-174: 174px;

  /* Layout */
  --page-max-width: 1440px;
  --section-gap: 84px;
  --card-padding: 25px;
  --element-gap: 17px;

  /* Named Radii */
  --radius-tags: 0px;
  --radius-cards: 0px;
  --radius-inputs: 0px;
  --radius-buttons: 0px;

  /* Shadows */
  --shadow-subtle: rgb(0, 0, 0) 0px 0px 0px 1px;

  /* Surfaces */
  --surface-cream-paper: #fffffc;
  --surface-ink-black: #000000;
}
```

### Tailwind v4

```css
@theme {
  /* Colors */
  --color-cream-paper: #fffffc;
  --color-ink-black: #000000;

  /* Typography */
  --font-circular-std: &#x27;Circular Std&#x27;, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, &quot;Segoe UI&quot;, Roboto, sans-serif;

  /* Typography — Scale */
  --text-caption: 13px;
  --leading-caption: 1.5;
  --text-body-sm: 17px;
  --leading-body-sm: 1.5;
  --text-body: 20px;
  --leading-body: 1.5;
  --text-subheading: 25px;
  --leading-subheading: 1.15;
  --text-heading-sm: 34px;
  --leading-heading-sm: 1.1;
  --tracking-heading-sm: -0.34px;
  --text-heading: 50px;
  --leading-heading: 1.06;
  --tracking-heading: -0.6px;
  --text-heading-lg: 109px;
  --leading-heading-lg: 1;
  --tracking-heading-lg: -3.27px;
  --text-display: 134px;
  --leading-display: 1;
  --tracking-display: -4.02px;
  --text-display-lg: 166px;
  --leading-display-lg: 0.8;
  --tracking-display-lg: -8.3px;
  --text-display-xl: 201px;
  --leading-display-xl: 0.8;
  --tracking-display-xl: -14.07px;

  /* Spacing */
  --spacing-5: 5px;
  --spacing-8: 8px;
  --spacing-10: 10px;
  --spacing-11: 11px;
  --spacing-13: 13px;
  --spacing-17: 17px;
  --spacing-25: 25px;
  --spacing-50: 50px;
  --spacing-59: 59px;
  --spacing-84: 84px;
  --spacing-101: 101px;
  --spacing-134: 134px;
  --spacing-168: 168px;
  --spacing-174: 174px;

  /* Shadows */
  --shadow-subtle: rgb(0, 0, 0) 0px 0px 0px 1px;
}
```
</code></pre></div></div></div></div></div></main></div><script>$RS=function(a,b){a=document.getElementById(a);b=document.getElementById(b);for(a.parentNode.removeChild(a);a.firstChild;)b.parentNode.insertBefore(a.firstChild,b);b.parentNode.removeChild(b)};$RS(