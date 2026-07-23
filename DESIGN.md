---
name: Industrial Precision
colors:
  surface: '#fef9ef'
  surface-dim: '#dedad0'
  surface-bright: '#fef9ef'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f8f3e9'
  surface-container: '#f2ede3'
  surface-container-high: '#ede8de'
  surface-container-highest: '#e7e2d8'
  on-surface: '#1d1c16'
  on-surface-variant: '#594238'
  inverse-surface: '#32302a'
  inverse-on-surface: '#f5f0e6'
  outline: '#8c7166'
  outline-variant: '#e0c0b3'
  surface-tint: '#a33e00'
  primary: '#a33e00'
  on-primary: '#ffffff'
  primary-container: '#ef6820'
  on-primary-container: '#4e1a00'
  inverse-primary: '#ffb596'
  secondary: '#5f5e5e'
  on-secondary: '#ffffff'
  secondary-container: '#e2dfde'
  on-secondary-container: '#636262'
  tertiary: '#655d51'
  on-tertiary: '#ffffff'
  tertiary-container: '#999082'
  on-tertiary-container: '#2f291f'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffdbcd'
  primary-fixed-dim: '#ffb596'
  on-primary-fixed: '#360f00'
  on-primary-fixed-variant: '#7c2e00'
  secondary-fixed: '#e5e2e1'
  secondary-fixed-dim: '#c8c6c5'
  on-secondary-fixed: '#1c1b1b'
  on-secondary-fixed-variant: '#474746'
  tertiary-fixed: '#ede1d1'
  tertiary-fixed-dim: '#d0c5b5'
  on-tertiary-fixed: '#201b11'
  on-tertiary-fixed-variant: '#4d463a'
  background: '#fef9ef'
  on-background: '#1d1c16'
  surface-variant: '#e7e2d8'
typography:
  display-lg:
    fontFamily: Hanken Grotesk
    fontSize: 64px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  display-md:
    fontFamily: Hanken Grotesk
    fontSize: 48px
    fontWeight: '600'
    lineHeight: '1.1'
  headline-sm:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.2'
  body-lg:
    fontFamily: Hanken Grotesk
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.5'
  body-md:
    fontFamily: Hanken Grotesk
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  label-md:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1.2'
    letterSpacing: 0.05em
  label-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.2'
  display-mobile:
    fontFamily: Hanken Grotesk
    fontSize: 40px
    fontWeight: '700'
    lineHeight: '1.1'
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  gutter: 1px
  margin-mobile: 24px
  margin-desktop: 48px
---

## Brand & Style

This design system is built for a high-utility calculator app that balances mechanical heritage with modern minimalism. The aesthetic is inspired by industrial engineering blueprints and mid-century laboratory equipment. 

The personality is **authoritative, precise, and utilitarian**. It avoids decorative flourishes in favor of clear structural hierarchy and functional clarity. The target audience includes engineers, designers, and professionals who value tools that feel robust and reliable. 

Visual style highlights:
- **Minimalism:** Use of generous negative space to prevent cognitive overload.
- **Industrial Layout:** Structured grid systems that echo physical hardware panels.
- **Precision Typography:** High legibility with a focus on data density and clear numerical separation.

## Colors

The palette is rooted in industrial "equipment beige" and high-visibility safety accents.

- **Primary (#EF6820):** An international orange used exclusively for action states, results, and critical operator functions. 
- **Neutral Background (#F5F0E6):** A warm, off-white/beige that reduces eye strain compared to pure white, providing a "paper-like" or "plastic-shell" tactile feel.
- **Secondary (#1A1A1A):** A deep charcoal for primary text and heavy structural lines.
- **Tertiary (#8C8375):** A muted taupe-grey for secondary labels, grid lines, and inactive states.

Color application should be disciplined: use the primary orange sparingly to ensure it maintains its "signal" status against the neutral backdrop.

## Typography

The typography system uses a pairing of a sharp Neo-grotesk and a technical Monospace font.

- **Hanken Grotesk** handles all primary interface elements and numerical displays. Its clean, geometric shapes reflect modern engineering.
- **JetBrains Mono** is utilized for metadata, scientific notations, and technical labels. The monospaced nature reinforces the feeling of a calculated, "under-the-hood" environment.

For the main calculator readout, use `display-lg` with tight tracking. Secondary technical data (like memory or history) should use `label-md`.

## Layout & Spacing

The layout is governed by a strict **1px hairline grid** system that separates different functional zones (Display, Basic Ops, Advanced Ops).

- **Grid:** Use a 4-column layout for mobile and an 8-column layout for desktop/tablet.
- **Margins:** Generous outer margins (`margin-mobile`) ensure the calculator feels like an object sitting in space.
- **Internal Spacing:** Components are separated by `gutter` (1px) lines in `tertiary_color`, creating a "segmented" physical button feel without relying on shadows.
- **Rhythm:** All vertical spacing should be multiples of the 4px base unit to maintain technical alignment.

## Elevation & Depth

This system avoids traditional shadows to maintain a flat, industrial aesthetic. Depth is achieved through **structural layering and tonal shifts**:

- **Hairline Borders:** Use 1px solid lines (#8C8375) to define areas.
- **Inverted Surfaces:** For high-priority areas like the main display or active buttons, invert the color scheme (Secondary background with Primary or Neutral text).
- **Tonal Stepping:** Use subtle variations of the neutral background to differentiate the "case" of the calculator from the "screen."
- **Interaction Depth:** On hover or press, do not use shadows. Instead, use a fill color change (e.g., Neutral to light Grey) or a 1px offset to simulate a mechanical button press.

## Shapes

The shape language is predominantly **rectilinear with micro-radii**.

- **Containers:** Main app container and primary functional blocks use 0px (Sharp) corners to emphasize the architectural structure.
- **Interactive Elements:** Buttons and input fields use `soft` roundedness (4px) to provide a subtle tactile hint that these elements are interactive.
- **Signals:** Indicators and mode-toggles use circular shapes (pill-shaped) to distinguish them from standard buttons.

## Components

### Buttons
- **Standard:** Neutral background, 1px border, charcoal text. `label-md` typography.
- **Operator:** Taupe-grey background, charcoal text.
- **Action (Enter/Equal):** Primary orange background, Neutral text. No border.
- **State:** Active buttons should switch to a solid Charcoal background with Neutral text.

### Input Fields / Display
- The main readout should be "inset" visually using a 1px border. 
- Use a slightly darker shade of the neutral background (#EDE8DE) for the display area to simulate an LCD panel.

### Chips / Indicators
- Small circular dots in Primary Orange or Charcoal used to indicate active modes (e.g., RAD vs DEG).

### Lists (History)
- Technical data should be displayed in `label-sm`.
- Items are separated by horizontal 1px hairlines.
- Right-aligned values for numerical consistency.

### Cards
- Used for grouping advanced functions (Trigonometry, Calculus). 
- Should have a 1px border and a distinct `label-sm` header pinned to the top-left corner.