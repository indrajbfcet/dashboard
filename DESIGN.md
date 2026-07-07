---
name: Insightful Management
colors:
  surface: '#fbf8ff'
  surface-dim: '#dbd9e2'
  surface-bright: '#fbf8ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f4f2fc'
  surface-container: '#efedf6'
  surface-container-high: '#e9e7f0'
  surface-container-highest: '#e3e1ea'
  on-surface: '#1a1b22'
  on-surface-variant: '#454652'
  inverse-surface: '#2f3037'
  inverse-on-surface: '#f2eff9'
  outline: '#757684'
  outline-variant: '#c5c5d4'
  surface-tint: '#4355b9'
  primary: '#24389c'
  on-primary: '#ffffff'
  primary-container: '#3f51b5'
  on-primary-container: '#cacfff'
  inverse-primary: '#bac3ff'
  secondary: '#006c49'
  on-secondary: '#ffffff'
  secondary-container: '#6cf8bb'
  on-secondary-container: '#00714d'
  tertiary: '#603b00'
  on-tertiary: '#ffffff'
  tertiary-container: '#805000'
  on-tertiary-container: '#ffc988'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dee0ff'
  primary-fixed-dim: '#bac3ff'
  on-primary-fixed: '#00105c'
  on-primary-fixed-variant: '#293ca0'
  secondary-fixed: '#6ffbbe'
  secondary-fixed-dim: '#4edea3'
  on-secondary-fixed: '#002113'
  on-secondary-fixed-variant: '#005236'
  tertiary-fixed: '#ffddb8'
  tertiary-fixed-dim: '#ffb95f'
  on-tertiary-fixed: '#2a1700'
  on-tertiary-fixed-variant: '#653e00'
  background: '#fbf8ff'
  on-background: '#1a1b22'
  surface-variant: '#e3e1ea'
typography:
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  data-mono:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  container-margin: 16px
  gutter: 16px
---

## Brand & Style
The brand personality is authoritative yet approachable, designed for high-efficiency environments where clarity of data is paramount. The target audience includes project coordinators, educators, and team leads who require a "glanceable" interface to track progress and deadlines.

The design style is **Corporate Modern with Minimalist influences**. It prioritizes high whitespace to reduce cognitive load and uses a systematic approach to color and elevation. The goal is to evoke a sense of organized calm and professional reliability, ensuring that critical data points—like overdue tasks or pending approvals—surface naturally without visual clutter.

## Colors
The palette is functional and status-driven. 
- **Primary (Deep Indigo):** Reserved for brand moments, primary action buttons, and active navigation states.
- **Success (Emerald Green):** Used exclusively for "Completed" or "Paid" statuses to provide positive reinforcement.
- **Warning (Amber):** Signals "Pending" or "In Progress" items that require attention but are not yet critical.
- **Danger (Rose):** Highlights "Overdue," "Cancelled," or "High Priority" errors.
- **Neutral (Slate Grays):** A stepped scale from `#F8FAFC` for backgrounds to `#1E293B` for primary headings, ensuring deep contrast and accessibility.

## Typography
The system uses **Inter** for its exceptional legibility and neutral, professional tone. 
- **Headlines:** Use tighter letter spacing and heavier weights to establish a strong hierarchy.
- **Body Text:** Standard weight for readability; `body-sm` is the workhorse for dashboard metadata and table rows.
- **Labels:** Uppercase styles are used for table headers and section overviews to differentiate from interactive content.
- **Data Display:** For IDs or numerical values that require alignment (like assignment codes), a monospaced font is used to ensure clarity.

## Layout & Spacing
The design system employs a **12-column fluid grid** for desktop and a **single-column stack** for mobile. 

- **Desktop:** 24px margins with 16px gutters. Sidebars are fixed at 280px.
- **Mobile:** 16px horizontal safe-area margins.
- **Rhythm:** All spacing (padding, margins) follows an 8px scale. Use 16px (`md`) for standard card padding and 8px (`sm`) for tight component internal spacing.

## Elevation & Depth
Depth is conveyed through **Tonal Layers** supplemented by **Ambient Shadows**. 
- **Level 0 (Background):** `#F8FAFC` (Slate 50).
- **Level 1 (Cards/Surface):** White background with a subtle 1px border (`#E2E8F0`) and a soft shadow (0 1px 3px rgba(0,0,0,0.1)).
- **Level 2 (Modals/Dropdowns):** Increased shadow depth (0 10px 15px rgba(0,0,0,0.1)) to indicate a clear break from the canvas.

Shadows should be "clean," utilizing a slight indigo tint in the shadow color (`rgba(63, 81, 181, 0.05)`) to maintain brand harmony.

## Shapes
The design system adopts a **Rounded** aesthetic. 
- Standard components (Buttons, Inputs, Cards) use a **0.5rem (8px)** corner radius.
- Larger containers or empty state illustrations use **1rem (16px)**.
- Status chips and tags use a **Pill-shape (999px)** to distinguish them from interactive buttons.

## Components
- **Buttons:** Primary buttons are solid Deep Indigo with white text. Secondary buttons use a ghost style (border only) or a light slate background.
- **Status Chips:** High-contrast text on a low-opacity background of the status color (e.g., Emerald Green text on 10% opacity Emerald background).
- **Input Fields:** 8px rounded corners with a 1px Slate-200 border. Focus state moves the border to Primary Indigo with a 2px outer glow.
- **Cards:** White surfaces, 8px radius, used to group assignment details. Title and "Action" (Edit/View) should be clearly separated at the top and bottom.
- **Progress Bars:** Use a thick 8px track height with Success or Warning colors to indicate completion percentage.
- **Data Tables:** Row-based layouts with subtle separators. On mobile, tables reflow into "Stacked Cards" to maintain readability.