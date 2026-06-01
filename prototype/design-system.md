---
name: VUS Elite Portal
colors:
  surface: '#f9f9ff'
  surface-dim: '#cfdaf2'
  surface-bright: '#f9f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f0f3ff'
  surface-container: '#e7eeff'
  surface-container-high: '#dee8ff'
  surface-container-highest: '#d8e3fb'
  on-surface: '#111c2d'
  on-surface-variant: '#454650'
  inverse-surface: '#263143'
  inverse-on-surface: '#ecf1ff'
  outline: '#757681'
  outline-variant: '#c5c5d2'
  surface-tint: '#495a9e'
  primary: '#00185c'
  on-primary: '#ffffff'
  primary-container: '#1d3072'
  on-primary-container: '#899ae3'
  inverse-primary: '#b7c4ff'
  secondary: '#b91000'
  on-secondary: '#ffffff'
  secondary-container: '#e51f08'
  on-secondary-container: '#fffbff'
  tertiary: '#00242d'
  on-tertiary: '#ffffff'
  tertiary-container: '#003b48'
  on-tertiary-container: '#00accf'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dde1ff'
  primary-fixed-dim: '#b7c4ff'
  on-primary-fixed: '#001552'
  on-primary-fixed-variant: '#304285'
  secondary-fixed: '#ffdad4'
  secondary-fixed-dim: '#ffb4a7'
  on-secondary-fixed: '#400200'
  on-secondary-fixed-variant: '#910a00'
  tertiary-fixed: '#b3ebff'
  tertiary-fixed-dim: '#37d7ff'
  on-tertiary-fixed: '#001f27'
  on-tertiary-fixed-variant: '#004e5f'
  background: '#f9f9ff'
  on-background: '#111c2d'
  surface-variant: '#d8e3fb'
  background-main: '#f8fafc'
  surface-white: '#FFFFFF'
  status-success: '#10b981'
  status-warning: '#f9a825'
  gray-text-subtle: '#64748b'
  border-light: '#e2e8f0'
typography:
  display-lg:
    fontFamily: Bricolage Grotesque
    fontSize: 48px
    fontWeight: '800'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Bricolage Grotesque
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
  headline-md:
    fontFamily: Bricolage Grotesque
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-sm:
    fontFamily: Bricolage Grotesque
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-md:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  headline-lg-mobile:
    fontFamily: Bricolage Grotesque
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 36px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 4px
  xs: 8px
  sm: 16px
  md: 24px
  lg: 32px
  xl: 48px
  sidebar-width: 260px
  container-max: 1440px
---

## Brand & Style

The design system is engineered for a professional SaaS environment that balances educational authority with modern administrative efficiency. It targets educators, administrators, and students who require a focused, high-utility interface.

The aesthetic follows a **Corporate / Modern** direction. It prioritizes clarity through generous white space, a structured information hierarchy, and a refined color application that differentiates navigation from content. The atmosphere is serious and functional, ensuring that complex data remains legible and actionable without unnecessary visual noise.

## Colors

The palette is anchored by a deep navy (`#1D3072`) for primary branding and sidebar navigation, establishing a sense of stability. The brand red (`#E21D06`) is reserved for high-impact calls to action and critical alerts, while the cyan-blue (`#00C9F1`) serves as a secondary accent for interactive elements or data visualization.

The interface utilizes a "Cool Gray" scale for typography and borders to maintain a crisp, professional look. Backgrounds use a very light off-white (`#f8fafc`) to reduce eye strain during long work sessions, contrasting against pure white (`#FFFFFF`) surface cards.

## Typography

This design system uses a dual-font strategy optimized for Vietnamese diacritics. **Bricolage Grotesque** is employed for headlines and display text, providing a distinctive, modern character that sets the brand apart.

For all functional text, including body copy, data tables, and input labels, **Inter** is the standard. It provides exceptional legibility at small sizes and maintains a neutral, systematic feel. Hierarchies are established through consistent weight stepping and the use of uppercase letter-spacing for labels to distinguish them from standard body text.

## Layout & Spacing

The layout utilizes a **Fixed Grid** approach for the main content area, centered within the viewport, paired with a persistent sidebar navigation.

- **Desktop:** 12-column grid, 24px gutters, 32px margins. The sidebar remains fixed at 260px.
- **Tablet:** 8-column grid, 16px gutters, 24px margins. The sidebar may collapse into an icon-only rail or hide behind a hamburger menu.
- **Mobile:** 4-column fluid grid, 16px gutters and margins. All cards and containers reflow to full width.

Spacing follows a strict 4px/8px baseline grid to ensure mathematical harmony across all components.

## Elevation & Depth

Hierarchy is communicated through **Tonal Layers** and **Ambient Shadows**.

The background layer is the lowest (`#f8fafc`). Above this, content cards and containers sit on a white surface (`#FFFFFF`) with a subtle, highly-diffused shadow (0px 2px 4px rgba(30, 41, 59, 0.05)).

Interactive elements like dropdowns, modals, and hovered states use a more pronounced elevation (0px 10px 15px rgba(30, 41, 59, 0.1)) to indicate they are physically closer to the user. Borders are kept minimal, using `#e2e8f0` only when necessary to define boundaries within a single tonal layer.

## Shapes

The shape language is defined by **Rounded** geometry. A standard 8px (`0.5rem`) corner radius is applied to all primary containers, buttons, and input fields. This softened geometry prevents the "serious" tone from feeling cold or aggressive, making the portal feel approachable yet professional.

Badges and tags use a larger radius or a full "pill" shape to distinguish them from interactive buttons.

## Components

### Buttons
- **Primary:** Solid `#1D3072` with white text. High emphasis.
- **Outline:** 1px border of `#1D3072` or `#e2e8f0` with primary color text. Used for secondary actions.
- **Destructive:** Solid `#E21D06` for critical, irreversible actions.

### Form Fields
Inputs use a white background, 1px `#e2e8f0` border, and 8px radius. Active states transition the border to `#00C9F1` with a soft outer glow. Labels are positioned above the field in `label-md` style.

### Status Badges
Used for system statuses (e.g., "Active", "Pending"). They feature a light tinted background of the status color (10% opacity) with high-contrast text in the same hue.

### Cards
Cards are the primary container for dashboard modules. They feature a white background, 8px radius, and the standard ambient shadow. Headers within cards should use `headline-sm` with a bottom border divider.

### Sidebar
The sidebar uses the neutral dark navy (`#1e293b`). Nav items use white text at 70% opacity, transitioning to 100% opacity with a primary blue left-accent bar on active/hover states.
