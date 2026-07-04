---
name: Marine E-Commerce System
colors:
  surface: '#f4faff'
  surface-dim: '#d2dbe1'
  surface-bright: '#f4faff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#ecf5fb'
  surface-container: '#e6eff5'
  surface-container-high: '#e0e9ef'
  surface-container-highest: '#dbe4ea'
  on-surface: '#141d21'
  on-surface-variant: '#42474e'
  inverse-surface: '#293236'
  inverse-on-surface: '#e9f2f8'
  outline: '#72777f'
  outline-variant: '#c2c7cf'
  surface-tint: '#31628d'
  primary: '#002a48'
  on-primary: '#ffffff'
  primary-container: '#00416a'
  on-primary-container: '#7faddc'
  inverse-primary: '#9ccbfb'
  secondary: '#006879'
  on-secondary: '#ffffff'
  secondary-container: '#1fdcfe'
  on-secondary-container: '#005d6d'
  tertiary: '#262829'
  on-tertiary: '#ffffff'
  tertiary-container: '#3c3e3e'
  on-tertiary-container: '#a8a9a9'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#cfe5ff'
  primary-fixed-dim: '#9ccbfb'
  on-primary-fixed: '#001d33'
  on-primary-fixed-variant: '#114a73'
  secondary-fixed: '#aaedff'
  secondary-fixed-dim: '#16d9fb'
  on-secondary-fixed: '#001f26'
  on-secondary-fixed-variant: '#004e5c'
  tertiary-fixed: '#e2e2e2'
  tertiary-fixed-dim: '#c6c6c7'
  on-tertiary-fixed: '#1a1c1c'
  on-tertiary-fixed-variant: '#454747'
  background: '#f4faff'
  on-background: '#141d21'
  surface-variant: '#dbe4ea'
typography:
  display-lg:
    fontFamily: Montserrat
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Montserrat
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
  headline-lg-mobile:
    fontFamily: Montserrat
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
  headline-md:
    fontFamily: Montserrat
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
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
  price-display:
    fontFamily: Montserrat
    fontSize: 22px
    fontWeight: '700'
    lineHeight: 24px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  container-margin: 24px
  gutter: 16px
  stack-sm: 8px
  stack-md: 16px
  stack-lg: 32px
---

## Brand & Style

The visual identity of this design system is anchored in the concept of "Oceanic Freshness." It captures the clarity of shallow coastal waters and the depth of the open sea to evoke feelings of quality, trust, and premium service.

The design style is a sophisticated blend of **Corporate Modern** and **Glassmorphism**. We utilize translucent layers and soft-focus background blurs to mimic the refractive properties of water. This approach creates a "glossy" aesthetic that feels clean and hygienic—essential for a food delivery platform—while maintaining the professional rigor of a high-end e-commerce experience. The interface should feel fluid, approachable, and highly responsive, guiding users through the "catch of the day" with effortless navigation.

## Colors

The color palette is derived from marine environments. 
- **Deep Ocean Blue (#00416A)** serves as the primary anchor, used for headers, primary text, and high-level navigation to establish authority and trust.
- **Bright Sea Blue (#12D8FA)** acts as the functional highlight. This high-energy hue is reserved for primary actions, progress indicators, and "fresh" badges.
- **Neutral Backgrounds** utilize a very soft blue-tinted white (#F0F9FF) rather than pure grey, maintaining the oceanic theme even in negative space.

Gradients are used sparingly but strategically on primary call-to-action buttons and feature banners to reinforce the "glossy" marine aesthetic.

## Typography

This design system employs a dual-font strategy to balance personality with utility. 
- **Montserrat** is used for all headlines and price displays. Its geometric construction feels modern and friendly, while its bolder weights provide the necessary impact for product names and promotional headers.
- **Inter** is the workhorse for body copy, descriptions, and technical UI labels. Its high legibility at small sizes ensures that nutritional information and delivery details remain clear and accessible.

Line heights are generous to prevent the UI from feeling "cramped," reinforcing the open, airy feel of a premium marketplace.

## Layout & Spacing

The layout follows a **Fluid Grid** model with a base unit of 8px. This ensures a consistent rhythm across all components. 

- **Mobile:** A 4-column grid with 24px side margins. 
- **Desktop:** A 12-column grid centered in a 1280px max-width container.

Spacing is intentionally generous. We utilize "Safe Zones" around product images to emphasize the freshness of the photography. Vertical rhythm should prioritize white space to maintain a clean, uncluttered appearance, reminiscent of a high-end boutique fish market.

## Elevation & Depth

To achieve the "glossy" look, depth is created through a combination of **Ambient Shadows** and **Glassmorphism**:

1.  **The Base Layer:** A soft, blue-tinted background.
2.  **Surface Layer:** White cards use a very soft, diffused shadow (Blur: 20px, Y: 8px, Opacity: 6% of Deep Ocean Blue) rather than black. This keeps the shadows "cool" and integrated into the palette.
3.  **Floating Elements:** Floating Action Buttons (FABs) and active navigation items use a multi-layered shadow to appear as if they are floating on water.
4.  **Glass Layers:** Overlays (like bottom sheets or sticky headers) utilize a `backdrop-filter: blur(12px)` with a 70% opaque white background and a subtle 1px white border to simulate polished glass or sea mist.

## Shapes

The shape language is defined by extreme softness and fluidity. All primary containers (Product Cards, Search Bars, Modals) utilize a **2xl corner radius (1.5rem/24px)**. 

This high degree of roundedness removes "sharp edges," making the app feel safer, more organic, and more friendly. 
- **Small elements** (Chips, Badges): Use full pill-shaped rounding.
- **Medium elements** (Buttons, Inputs): Use 12px to 16px rounding.
- **Large elements** (Cards, Bottom Sheets): Use the signature 24px rounding.

## Components

### Buttons
Primary buttons should use the `gradient_oceanic` with white text. They should have a slight "inner glow" (a 1px semi-transparent white top border) to enhance the glossy effect.

### Product Cards
Cards are the heart of the experience. They must be pure white with a subtle 1px border (#E0F2FE) and the signature soft oceanic shadow. Images should be high-resolution with background removal to make the products "pop" off the card.

### Inputs & Search
The search bar should be a pill-shaped element with a soft inner shadow, giving it a slightly recessed "etched" look, or a glassmorphic blur when placed over a header image.

### Chips & Badges
Use Bright Sea Blue (#12D8FA) at 10-15% opacity for chip backgrounds, with the text in Deep Ocean Blue (#00416A). This creates a "watery" tag that is legible but light.

### Bottom Navigation
The navigation bar should be a floating glassmorphic element with a subtle backdrop blur. Active states are indicated by the primary Deep Ocean Blue with a soft glow underneath the icon.