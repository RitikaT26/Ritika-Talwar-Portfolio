---
name: Developer Portfolio System
colors:
  surface: '#131315'
  surface-dim: '#131315'
  surface-bright: '#39393b'
  surface-container-lowest: '#0e0e10'
  surface-container-low: '#1b1b1d'
  surface-container: '#201f21'
  surface-container-high: '#2a2a2c'
  surface-container-highest: '#353437'
  on-surface: '#e5e1e4'
  on-surface-variant: '#c2c6d8'
  inverse-surface: '#e5e1e4'
  inverse-on-surface: '#313032'
  outline: '#8c90a1'
  outline-variant: '#424656'
  surface-tint: '#b3c5ff'
  primary: '#b3c5ff'
  on-primary: '#002b75'
  primary-container: '#0066ff'
  on-primary-container: '#f8f7ff'
  inverse-primary: '#0054d6'
  secondary: '#ffffff'
  on-secondary: '#00382b'
  secondary-container: '#24ffcd'
  on-secondary-container: '#00725a'
  tertiary: '#abd600'
  on-tertiary: '#283500'
  tertiary-container: '#617b00'
  on-tertiary-container: '#f0ffbe'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#dae1ff'
  primary-fixed-dim: '#b3c5ff'
  on-primary-fixed: '#001849'
  on-primary-fixed-variant: '#003fa4'
  secondary-fixed: '#24ffcd'
  secondary-fixed-dim: '#00e0b3'
  on-secondary-fixed: '#002118'
  on-secondary-fixed-variant: '#00513f'
  tertiary-fixed: '#c3f400'
  tertiary-fixed-dim: '#abd600'
  on-tertiary-fixed: '#161e00'
  on-tertiary-fixed-variant: '#3c4d00'
  background: '#131315'
  on-background: '#e5e1e4'
  surface-variant: '#353437'
typography:
  display-xl:
    fontFamily: Space Grotesk
    fontSize: 72px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 48px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-md:
    fontFamily: Space Grotesk
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1'
    letterSpacing: 0.05em
  code:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1280px
  gutter: 32px
  margin-page: 64px
  section-gap: 128px
---

## Brand & Style

This design system is engineered for high-end developer portfolios, emphasizing technical precision, architectural clarity, and a "code-first" premium aesthetic. The brand personality is professional yet innovative, balancing the cold efficiency of a code editor with the polished sophistication of a luxury tech brand.

The visual direction combines **Minimalism** with **Glassmorphism**. It utilizes heavy whitespace to allow complex technical content to breathe, while employing semi-transparent surfaces and vibrant "electric" accents to signify cutting-edge capabilities. The emotional response is one of trust and high-performance engineering.

## Colors

The palette is anchored by a deep charcoal background that provides a "dark mode" environment preferred by the developer community. The **Electric Blue** acts as the primary driver for action and focus, representing energy and connectivity.

**Secondary Teal** and **Tertiary Lime** are used as high-utility signals—Teal for successful deployments or status indicators, and Lime for "Live" badges or critical highlights. Neutral slates and zinc grays are employed for metadata and secondary text to maintain a strict visual hierarchy. Contrast ratios must be strictly monitored to ensure accessibility against the dark backdrop.

## Typography

The typography strategy relies on **High Contrast**. **Space Grotesk** is used for headlines and labels to provide a geometric, technical feel that mirrors mathematical precision. Its bold weights at large scales create an editorial impact.

**Inter** is utilized for all body copy and technical descriptions. It was chosen for its exceptional legibility at small sizes and its neutral, utilitarian character which balances the more expressive display face. Font weights should jump significantly between levels (e.g., 400 for body to 700 for headlines) to ensure a clear information architecture.

## Layout & Spacing

This design system uses a **Fixed Grid** model for desktop views to maintain the integrity of complex code blocks and project showcases. The layout is centered on a 12-column grid with generous 32px gutters to prevent the "cluttered" feel often found in technical documentation.

Spacing follows a strict 8px base-unit scale. Vertical rhythm is driven by large section gaps (128px) to clearly differentiate between "Experience," "Projects," and "Contact" areas. Content should be grouped logically using varying scales of padding (24px for card internals, 48px for component groups).

## Elevation & Depth

Depth is achieved through **Glassmorphism** and subtle tonal layering rather than traditional heavy shadows. Surfaces are defined by:

1.  **Backdrop Blur:** Floating panels and navigation bars must use a `backdrop-blur` (20px-30px) to maintain context while isolating content.
2.  **Thin Borders:** Elements are defined by 1px solid borders at `white/10` opacity. This "ghost border" technique provides structure without adding visual bulk.
3.  **Tonal Stacking:** Background is `#0E0E10`. Elevated cards use a slightly lighter `#161618`.
4.  **Outer Glows:** Primary buttons and active states may utilize a soft, diffused blue outer glow (blur: 20px, spread: -5px) to simulate a light-emitting screen or terminal.

## Shapes

The shape language is modern and approachable, utilizing a consistent radius to soften the technical edges. Base components like buttons and input fields use a **0.5rem (8px)** radius. Larger structural elements, such as project cards and modal containers, use **1rem (16px)** for a more distinct "container" feel.

Strictly avoid sharp 0px corners, as they appear dated and overly aggressive. Circles are reserved exclusively for avatars and status indicators.

## Components

### Buttons
- **Primary:** Solid Electric Blue background with white text. High contrast. No shadow, or very subtle blue glow on hover.
- **Secondary:** Ghost style. `white/10` border, transparent background, white text. Transitions to `white/05` background on hover.

### Cards (Project Showcase)
- Semi-transparent background (Glassmorphism).
- 1px `white/10` border.
- 16px corner radius.
- Imagery inside cards should have a subtle inner glow to blend with the dark theme.

### Inputs & Text Areas
- Background: `#0B0E14` (darker than page).
- Border: 1px Zinc-800.
- Focus State: Border changes to Electric Blue with a minimal 2px outer glow.

### Chips & Tags
- Used for tech stacks (e.g., "React", "TypeScript").
- Small Space Grotesk text, uppercase.
- Subtle background: `rgba(0, 102, 255, 0.1)` with Electric Blue text.

### Navigation Bar
- Fixed top position.
- Full glassmorphism effect (blur + semi-transparent dark tint).
- Bottom border 1px `white/10`.