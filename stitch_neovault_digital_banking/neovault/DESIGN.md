---
name: NeoVault
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#393939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#20201f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353535'
  on-surface: '#e5e2e1'
  on-surface-variant: '#bac9cc'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#849396'
  outline-variant: '#3b494c'
  surface-tint: '#00daf3'
  primary: '#c3f5ff'
  on-primary: '#00363d'
  primary-container: '#00e5ff'
  on-primary-container: '#00626e'
  inverse-primary: '#006875'
  secondary: '#c8c6c5'
  on-secondary: '#313030'
  secondary-container: '#4a4949'
  on-secondary-container: '#bab8b7'
  tertiary: '#edecec'
  on-tertiary: '#2f3131'
  tertiary-container: '#d0d0d0'
  on-tertiary-container: '#585959'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#9cf0ff'
  primary-fixed-dim: '#00daf3'
  on-primary-fixed: '#001f24'
  on-primary-fixed-variant: '#004f58'
  secondary-fixed: '#e5e2e1'
  secondary-fixed-dim: '#c8c6c5'
  on-secondary-fixed: '#1c1b1b'
  on-secondary-fixed-variant: '#474646'
  tertiary-fixed: '#e3e2e2'
  tertiary-fixed-dim: '#c6c6c6'
  on-tertiary-fixed: '#1a1c1c'
  on-tertiary-fixed-variant: '#464747'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353535'
typography:
  headline-xl:
    fontFamily: Manrope
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Manrope
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  body-lg:
    fontFamily: Manrope
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: '0'
  body-md:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: '0'
  label-sm:
    fontFamily: Manrope
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  xs: 4px
  sm: 12px
  md: 24px
  lg: 48px
  xl: 80px
  gutter: 20px
  margin: 32px
---

## Brand & Style

This design system embodies "Digital-First Prestige." It is curated for a demographic that values technical precision and understated luxury. The brand personality is architectural, silent, and powerful—evoking the feeling of a private digital vault rather than a traditional retail bank.

The aesthetic blends **Minimalism** with **Glassmorphism**. High-density information is avoided in favor of "breathing" layouts that prioritize clarity and focus. The visual language uses deep tones to create a sense of security, while electric accents signal innovation and speed. Every interaction should feel intentional, mimicking the tactile satisfaction of high-end physical hardware.

## Colors

The palette is rooted in a "Deep Charcoal" base to provide a sophisticated, low-light environment that reduces eye strain and emphasizes premium hardware displays. 

- **Primary (Electric Blue):** Used sparingly for critical action points, active states, and data visualizations. It represents the "energy" of the digital transaction.
- **Secondary (Deep Charcoal):** The foundation of the UI, used for backgrounds and primary containers to create depth.
- **Silver Accents:** A gradient-based or metallic-matte silver is used for borders, icons, and secondary typography to provide a tactile, reflective quality.
- **High Contrast:** Pure white is reserved for primary body text to ensure maximum readability against the dark surfaces.

## Typography

The design system utilizes **Manrope** for its balance of geometric modernism and functional readability. The type hierarchy is strictly enforced to maintain a "luxe" editorial feel.

Headlines use tighter letter spacing and heavy weights to command attention, while body text is generously spaced to ensure a relaxed reading experience. Labels utilize uppercase styling with increased tracking to mimic the engraving found on high-end timepieces or debit cards. Silver tints should be applied to secondary text to create a clear visual hierarchy between "Value" (White) and "Context" (Silver).

## Layout & Spacing

The layout follows a **Fluid Grid** system with fixed-margin logic to ensure the UI feels anchored on all device sizes. We utilize an 8px rhythmic scale to maintain mathematical harmony across all components.

Generous white space (or "dark space") is the primary luxury signifier here. Content is grouped into logical modules with significant vertical padding (`xl`) to prevent the interface from feeling crowded. For mobile interfaces, a "Safe Zone" of 32px horizontal margin is maintained to ensure haptic navigation elements are easily reachable without visual clutter.

## Elevation & Depth

Depth is achieved through **Glassmorphism** and tonal layering rather than traditional heavy shadows. 

1.  **The Base:** The Deep Charcoal floor (`#121212`).
2.  **Surface Tiers:** Containers use a slightly lighter neutral (`#1A1A1A`) with 1px silver inner-borders (low opacity) to define edges.
3.  **Glass Elements:** Transaction cards and modals use a backdrop-blur (20px–40px) with a semi-transparent charcoal fill (60% opacity). This creates a "frosted obsidian" effect.
4.  **Electric Glow:** Active elements or "hot" zones emit a soft, diffused Electric Blue outer glow (blur: 24px, opacity: 15%) to simulate light emitting from within the glass.

## Shapes

The shape language is "Sophisticated-Rounded." We avoid sharp industrial corners to ensure the digital environment feels premium and approachable. 

Primary containers and buttons use a **0.5rem (8px)** base radius. For larger card elements (like virtual credit cards), we step up to **rounded-lg (16px)** to create a distinct visual container. This moderate roundedness communicates a modern, software-centric approach while remaining more "serious" than the pill-shaped aesthetics found in casual social apps.

## Components

**Buttons:** Primary actions are filled with an Electric Blue to Silver gradient, using black text for maximum contrast. Secondary actions utilize "Ghost" styling—a 1px silver border with a subtle backdrop blur.

**Glass Cards:** The centerpiece of this design system. These elements must feature a `backdrop-filter: blur()` and a hairline silver stroke. Information on cards should be set in high-contrast white with silver labels.

**Haptic Navigation:** The bottom navigation bar is floating and glassmorphic. Icons are "haptic-ready"—large touch targets (minimum 44x44px) that provide a subtle scale-down animation on press to simulate physical resistance.

**Input Fields:** Minimalist under-line inputs or very subtly filled containers. The focus state triggers a "glow" from the bottom border in Electric Blue.

**Progress Bars & Data:** Use thin, glowing lines of Electric Blue. Data visualizations should be stripped of axes and grids, favoring a clean, "heads-up display" (HUD) aesthetic.