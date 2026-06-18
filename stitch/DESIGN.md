---
name: TaskPulse Mini
colors:
  surface: '#031427'
  surface-dim: '#031427'
  surface-bright: '#2a3a4f'
  surface-container-lowest: '#000f21'
  surface-container-low: '#0b1c30'
  surface-container: '#102034'
  surface-container-high: '#1b2b3f'
  surface-container-highest: '#26364a'
  on-surface: '#d3e4fe'
  on-surface-variant: '#c3c6d7'
  inverse-surface: '#d3e4fe'
  inverse-on-surface: '#213145'
  outline: '#8d90a0'
  outline-variant: '#434655'
  surface-tint: '#b4c5ff'
  primary: '#b4c5ff'
  on-primary: '#002a78'
  primary-container: '#2563eb'
  on-primary-container: '#eeefff'
  inverse-primary: '#0053db'
  secondary: '#ffb95f'
  on-secondary: '#472a00'
  secondary-container: '#ee9800'
  on-secondary-container: '#5b3800'
  tertiary: '#bec6e0'
  on-tertiary: '#283044'
  tertiary-container: '#656d84'
  on-tertiary-container: '#eef0ff'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#dbe1ff'
  primary-fixed-dim: '#b4c5ff'
  on-primary-fixed: '#00174b'
  on-primary-fixed-variant: '#003ea8'
  secondary-fixed: '#ffddb8'
  secondary-fixed-dim: '#ffb95f'
  on-secondary-fixed: '#2a1700'
  on-secondary-fixed-variant: '#653e00'
  tertiary-fixed: '#dae2fd'
  tertiary-fixed-dim: '#bec6e0'
  on-tertiary-fixed: '#131b2e'
  on-tertiary-fixed-variant: '#3f465c'
  background: '#031427'
  on-background: '#d3e4fe'
  surface-variant: '#26364a'
typography:
  display:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
    letterSpacing: -0.02em
  headline-sm:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
    letterSpacing: -0.01em
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
  label-caps:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
  mono-data:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 16px
  xl: 24px
  gutter: 12px
  margin: 16px
---

## Brand & Style

This design system is engineered for high-performance productivity and deep work. The brand personality is **Precise, Calm, and Functional**, designed to stay out of the user’s way while providing the structural integrity needed for complex task management. 

The aesthetic follows a **Modern Corporate/Minimalist** hybrid approach. It prioritizes information density and clarity over decorative elements. Visual noise is aggressively reduced to promote a state of "flow," utilizing a systematic arrangement of data, subtle transitions, and a rigorous adherence to a functional grid. The emotional response is one of organized control and professional reliability.

## Colors

The palette is anchored in a dark-mode foundation to reduce eye strain during extended focus sessions. 

- **Foundation (Tertiary):** Deep Navy (`#0F172A`) serves as the primary canvas, providing a stable, low-distraction environment.
- **Foundation (Slate):** Slate Grays (ranging from `#1E293B` to `#64748B`) define UI boundaries, surfaces, and secondary text.
- **Action (Pulse Blue):** Vibrant Blue (`#2563EB`) is reserved strictly for primary actions, progress indicators, and interactive highlights.
- **State (Focus Amber):** A warm, high-visibility Amber (`#F59E0B`) is utilized exclusively for active countdowns, high-priority alerts, and "Focus Mode" states to differentiate time-sensitive data from standard tasks.

## Typography

The system utilizes **Inter** as its primary typeface for its exceptional legibility at small sizes and high x-height. For data-heavy components like timers and IDs, **JetBrains Mono** is used to ensure character distinction and alignment.

- **Hierarchy:** We use tight line heights to maintain high information density.
- **Labels:** Small caps with tracking are used for section headers to provide structure without requiring large font sizes.
- **Data:** Numerical values in tables and countdowns should always use the `mono-data` style to prevent layout shifts during value updates.

## Layout & Spacing

This design system employs a **4px baseline grid** to achieve a high-density "utility" feel. The layout is optimized for desktop productivity.

- **Grid Model:** A 12-column fluid grid is used for the main dashboard, but individual modules (Sidebar, Task List, Inspector) use fixed widths to maximize the central work area.
- **Density:** Padding is intentionally compact (`8px` to `12px` for most containers) to allow as much data as possible to be visible above the fold.
- **Breakpoints:**
  - **Compact (<640px):** Single column, collapsible sidebar.
  - **Standard (1024px+):** Three-pane layout (Navigation | Task List | Details).

## Elevation & Depth

To maintain a "mini" and precise feel, the design system avoids heavy shadows. Instead, it uses **Tonal Layering** and **Low-Contrast Outlines**.

- **Surface 1 (Base):** Deep Navy (`#0F172A`).
- **Surface 2 (Containers):** Slate (`#1E293B`).
- **Borders:** Subtle `1px` solid borders in Slate (`#334155`) define edges. 
- **Interaction:** Active elements do not lift; instead, they receive a `1px` Pulse Blue border or a subtle background shift to a lighter slate. Shadows are only used for floating menus/dropdowns—sharp, small radius, 25% opacity black.

## Shapes

The shape language is **Soft (0.25rem)**. This provides enough rounding to feel modern and professional while maintaining the structural "grid-like" feel required for a high-density tool. 

- **Primary Radius:** `4px` for buttons, inputs, and small cards.
- **Large Radius:** `8px` for main container panels.
- **Exceptions:** Checkboxes use a `2px` radius for a crisp, technical appearance.

## Components

### Buttons & Inputs
- **Primary Action:** Solid Pulse Blue background, white text, `4px` radius.
- **Ghost Input:** Transparent background with a 1px border. On focus, the border transitions to Pulse Blue with no outer glow.
- **Density:** Button heights are capped at `32px` for standard and `28px` for "mini" variants.

### Task Cards
- Minimalist design: No shadows. 1px border. 
- Hover state: Background shifts from `#1E293B` to `#334155`.
- Active state: Left-edge accent of Pulse Blue (2px width).

### Data Tables
- Header: `label-caps` typography with a subtle background tint.
- Rows: `32px` fixed height. Zebra striping is not used; instead, 1px horizontal dividers in `#334155` separate entries.
- Numerical cells use `mono-data`.

### Focus Timer
- Uses **Focus Amber** for the digit display.
- Circular progress indicators use a `2px` stroke width for a technical, wireframe-inspired look.

### Chips & Tags
- Compact height (`20px`), using low-saturation backgrounds with high-contrast text for status labeling.