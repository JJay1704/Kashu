---
name: Kashu Design System
colors:
  surface: '#f8f9ff'
  surface-dim: '#cbdbf5'
  surface-bright: '#f8f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eff4ff'
  surface-container: '#e5eeff'
  surface-container-high: '#dce9ff'
  surface-container-highest: '#d3e4fe'
  on-surface: '#0b1c30'
  on-surface-variant: '#45464d'
  inverse-surface: '#213145'
  inverse-on-surface: '#eaf1ff'
  outline: '#76777d'
  outline-variant: '#c6c6cd'
  surface-tint: '#565e74'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#131b2e'
  on-primary-container: '#7c839b'
  inverse-primary: '#bec6e0'
  secondary: '#006c49'
  on-secondary: '#ffffff'
  secondary-container: '#6cf8bb'
  on-secondary-container: '#00714d'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#40000d'
  on-tertiary-container: '#f23d5c'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae2fd'
  primary-fixed-dim: '#bec6e0'
  on-primary-fixed: '#131b2e'
  on-primary-fixed-variant: '#3f465c'
  secondary-fixed: '#6ffbbe'
  secondary-fixed-dim: '#4edea3'
  on-secondary-fixed: '#002113'
  on-secondary-fixed-variant: '#005236'
  tertiary-fixed: '#ffdadb'
  tertiary-fixed-dim: '#ffb2b7'
  on-tertiary-fixed: '#40000d'
  on-tertiary-fixed-variant: '#92002a'
  background: '#f8f9ff'
  on-background: '#0b1c30'
  surface-variant: '#d3e4fe'
typography:
  display-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 20px
    fontWeight: '600'
    lineHeight: '1.4'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
  label-md:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.05em
  numeric-xl:
    fontFamily: Plus Jakarta Sans
    fontSize: 36px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: -0.01em
  numeric-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '600'
    lineHeight: '1'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  container-max-width: 1200px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 40px
  stack-sm: 8px
  stack-md: 16px
  stack-lg: 32px
---

## Brand & Style
The design system for this personal finance application is rooted in **Minimalism** with a focus on high-clarity data visualization. The brand personality is dependable, precise, and encouraging, aiming to transform the often-stressful task of money management into a calm, controlled experience.

The visual direction prioritizes whitespace and structural alignment to reduce cognitive load. By utilizing a "Content-First" approach, the UI recedes into the background, allowing the user's financial data to take center stage. The aesthetic is modern and professional, leveraging crisp edges and subtle depth to establish a sense of institutional security.

## Colors
The palette is engineered for financial clarity:
- **Primary (Deep Navy):** Used for core navigation, primary actions, and "Stable" branding elements to project security.
- **Secondary (Emerald Green):** Representing income and growth. This is the "Success" token.
- **Tertiary (Soft Coral):** Representing expenses and outflows. This is the "Error" token.
- **Neutral (Slate):** Used for secondary text and balanced states.

Use the background color (#F8FAFC) for the main canvas and the surface color (#FFFFFF) for cards and containers to create a subtle layered effect.

## Typography
This design system utilizes **Plus Jakarta Sans** for headings and large currency displays to provide a modern, friendly character. **Inter** is used for body text and functional labels due to its exceptional legibility at small sizes.

**Tabular Figures:** Always use `tabular-nums` for transaction lists and balance sheets to ensure decimal points and currency symbols align vertically for easy scanning.

## Layout & Spacing
The layout follows a **12-column fluid grid** on desktop and a **4-column grid** on mobile. 

- **Padding:** High-density financial data should be balanced with generous "Safe Areas." Cards should never have less than 24px of internal padding.
- **Rhythm:** An 8px linear scale is used for all spatial relationships. 
- **Alignment:** Use a fixed-width container for dashboard views on large screens to prevent data points from becoming too far apart, which can hinder eye-tracking across rows.

## Elevation & Depth
Depth is conveyed through **Tonal Layering** supplemented by **Ambient Shadows**. 

- **Level 0 (Background):** #F8FAFC. The lowest layer.
- **Level 1 (Cards):** #FFFFFF with a 1px border (#E2E8F0) and a soft, diffused shadow: `0px 4px 6px -1px rgba(15, 23, 42, 0.05)`.
- **Level 2 (Interactive/Floating):** Higher elevation used for active inputs or dropdowns, with a more pronounced shadow: `0px 10px 15px -3px rgba(15, 23, 42, 0.1)`.

Avoid heavy blacks in shadows; always tint shadows with the primary navy color at very low opacities (5-10%).

## Shapes
A "Rounded" shape language (0.5rem base) is applied across the system to soften the "hard" nature of financial data.

- **Standard Buttons & Inputs:** 0.5rem (8px).
- **Cards:** 1rem (16px) to create a clear container identity.
- **Charts:** Use rounded caps on bar charts and soft corners on line graph data points.
- **Pills/Chips:** Fully rounded (9999px) to distinguish them from interactive buttons.

## Components
- **Buttons:** Primary buttons use the Deep Navy background with white text. Secondary buttons use a Slate-100 background. Interactive states should use a subtle opacity shift (90%) rather than a color change.
- **Transaction Cards:** Use a three-column layout: Icon (left), Description/Category (center), and Amount (right, right-aligned). Amounts should be color-coded (Emerald for positive, Coral for negative).
- **Inputs:** Use a 1px border (#CBD5E1) that thickens and changes to Deep Navy (#0F172A) on focus. Labels should always be visible above the input, never hidden as placeholders.
- **Progress Bars:** Use Emerald Green for savings goals and Soft Coral for budget limits to provide immediate visual feedback.
- **Empty States:** Use light slate illustrations and clear "Call to Action" buttons to guide users when no data is present.