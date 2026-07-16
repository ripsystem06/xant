---
name: Kinetic Precision
colors:
  surface: '#131314'
  surface-dim: '#131314'
  surface-bright: '#3a393a'
  surface-container-lowest: '#0e0e0f'
  surface-container-low: '#1c1b1c'
  surface-container: '#201f20'
  surface-container-high: '#2a2a2b'
  surface-container-highest: '#353436'
  on-surface: '#e5e2e3'
  on-surface-variant: '#c2c6d8'
  inverse-surface: '#e5e2e3'
  inverse-on-surface: '#313031'
  outline: '#8c90a1'
  outline-variant: '#424656'
  surface-tint: '#b3c5ff'
  primary: '#b3c5ff'
  on-primary: '#002b75'
  primary-container: '#0066ff'
  on-primary-container: '#f8f7ff'
  inverse-primary: '#0054d6'
  secondary: '#a2e7ff'
  on-secondary: '#003642'
  secondary-container: '#00d2fd'
  on-secondary-container: '#005669'
  tertiary: '#ffb59d'
  on-tertiary: '#5d1900'
  tertiary-container: '#cc4204'
  on-tertiary-container: '#fff6f4'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#dae1ff'
  primary-fixed-dim: '#b3c5ff'
  on-primary-fixed: '#001849'
  on-primary-fixed-variant: '#003fa4'
  secondary-fixed: '#b4ebff'
  secondary-fixed-dim: '#3cd7ff'
  on-secondary-fixed: '#001f27'
  on-secondary-fixed-variant: '#004e5f'
  tertiary-fixed: '#ffdbd0'
  tertiary-fixed-dim: '#ffb59d'
  on-tertiary-fixed: '#390c00'
  on-tertiary-fixed-variant: '#832600'
  background: '#131314'
  on-background: '#e5e2e3'
  surface-variant: '#353436'
typography:
  display-lg:
    fontFamily: Hanken Grotesk
    fontSize: 48px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-sm:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Geist
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Geist
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  label-mono:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1'
    letterSpacing: 0.05em
  label-mono-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1'
    letterSpacing: 0.1em
  headline-md-mobile:
    fontFamily: Hanken Grotesk
    fontSize: 28px
    fontWeight: '700'
    lineHeight: '1.2'
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 48px
  container-max: 1440px
---

## Brand & Style

This design system targets high-stakes environments—fintech trading floors, automotive telemetry, and developer infrastructure. The aesthetic is "Tech-Motorsport," blending the precision of a dashboard with the aggressive performance of a racing engine.

The style is **Modern-Brutalist Minimalism**. It uses high-contrast surfaces, razor-sharp typography, and a "dark mode first" philosophy. The interface should feel incredibly fast, utilizing thin borders, monospaced data points, and a restricted color palette to minimize cognitive load while maximizing the impact of critical data.

## Colors

The palette is anchored in deep blacks and "Oil-Slick" grays to provide a void-like backdrop for the electric blue accents. 

- **Primary Blue (#0066FF):** Used for core actions, branding, and active states. It represents stability and technical depth.
- **Vibrant Cyan (#00D4FF):** Used sparingly for "live" data, highlights, and secondary interactive elements to provide a sense of velocity.
- **Neutral Core:** Grays are strictly neutral (0% saturation) to ensure the blue hues pop without visual vibration.
- **Success/Warning/Error:** Use high-chroma emerald, amber, and crimson, but tint them with 10% of the primary blue to maintain system harmony.

## Typography

Typography is a tool for information density. 

- **Display & Headlines:** Use Hanken Grotesk with tight tracking. It provides a sharp, contemporary "Neo-Grotesque" look that feels engineered.
- **Body:** Geist provides exceptional clarity for long-form technical documentation and financial reports.
- **Data & UI Labels:** JetBrains Mono is mandatory for all numerical data, code snippets, and status labels. This reinforces the "Developer/Tech" aesthetic and ensures tabular data aligns perfectly.

## Layout & Spacing

This design system utilizes a **Fixed Grid** model for desktop and a **Fluid Fluid** model for mobile.

- **Grid:** 12-column structure with 24px gutters. Elements should align strictly to the grid to maintain a "blueprint" feel.
- **Rhythm:** An 8px base unit is used for component sizing, but a 4px "micro-step" is allowed for dense data displays.
- **Density:** High-density layouts are preferred. Padding inside containers should be tight (16px or 20px) to keep information proximal.

## Elevation & Depth

Depth is conveyed through **Tonal Layering** and **Subtle Outlines** rather than traditional shadows.

- **Z-Index Strategy:** Higher elevation elements use a lighter gray surface (e.g., #1A1A1C) compared to the base background (#050505).
- **Borders:** All containers must have a 1px solid border. Use a low-opacity white (10-15%) for inactive states and the primary electric blue for active/focused states.
- **Glow:** Only the most critical interactive elements (like a "Commit Trade" button) may use a subtle, 8px-blur outer glow in the primary blue to simulate an illuminated physical switch.

## Shapes

The shape language is "Soft-Industrial." 

- **Radius:** Standard components use a 4px (0.25rem) radius. This is enough to prevent the UI from feeling "hostile" while maintaining the precision of a hard-edged technical instrument.
- **Buttons:** Keep corners consistent with containers. Never use pill-shaped buttons; they are too organic for this aesthetic.

## Components

- **Buttons:** Primary buttons use a solid #0066FF fill with white JetBrains Mono text. On hover, they transition to #00D4FF. Secondary buttons are "Ghost" style: 1px blue border, no fill.
- **Inputs:** Dark backgrounds (#0A0A0B) with 1px gray borders. On focus, the border turns electric blue and the label (monospaced) shifts to the primary blue.
- **Status Chips:** Use a "dot" indicator (Primary Blue for active, Neutral Gray for idle) with monospaced uppercase text.
- **Data Cards:** No shadows. Use a 1px border (#1A1A1C). The card header should have a subtle 2px blue "accent bar" on the left side to denote focus.
- **Progress Bars:** Use a 2px height for a sleek, high-speed telemetry look. The track should be nearly black, the indicator the vibrant #00D4FF cyan.