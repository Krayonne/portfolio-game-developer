---
name: Thanadul Suanma Portfolio
description: A Unity Developer's portfolio blending technical systems with mechanical elegance.
colors:
  primary: "#e8829a"
  primary-soft: "#f4b8c8"
  primary-light: "#fce8f0"
  primary-dark: "#c4516a"
  neutral-bg: "#fdf0f5"
  neutral-surface: "#ffffff"
  neutral-text: "#4a2d35"
  neutral-text-soft: "#9e6b7a"
typography:
  display:
    fontFamily: "Nunito, Prompt, sans-serif"
    fontSize: "clamp(2rem, 4vw, 3.2rem)"
    fontWeight: 800
    lineHeight: 1.2
  body:
    fontFamily: "Nunito, Prompt, sans-serif"
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.6
rounded:
  sm: "10px"
  md: "16px"
  lg: "24px"
  full: "999px"
spacing:
  xs: "8px"
  sm: "16px"
  md: "24px"
  lg: "48px"
  xl: "80px"
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "#ffffff"
    rounded: "{rounded.full}"
    padding: "10px 28px"
  card-base:
    backgroundColor: "{colors.neutral-surface}"
    rounded: "{rounded.lg}"
    padding: "20px"
---

# Design System: Thanadul Suanma Portfolio

## 1. Overview

**Creative North Star: "Mechanical Elegance"**

The design system for Thanadul Suanma's portfolio balances the precise, systematic nature of game development with a soft, inviting aesthetic. It reflects the persona of a developer who cares about performance and systems ("Mechanical") but delivers them with high-quality polish and a human touch ("Elegance").

This system rejects the "generic SaaS" look and instead embraces a "Plush Technical" vibe. It uses soft colors, generous rounded corners, and subtle motion to create a responsive, tactile environment that feels as good as a well-optimized Unity game.

**Key Characteristics:**
- Tactile surfaces with "lifted" shadows.
- Precise alignment and systematic spacing.
- Soft, rose-tinted palette (Identity preserved).
- Fluid, responsive typography.

## 2. Colors

The palette is a sophisticated "Rose Petal" range that avoids the oversaturation of typical "gamer" or "tech" sites.

### Primary
- **Blossom** (#e8829a): The main accent used for buttons, highlights, and primary icons. It is the heart of the brand.

### Neutral
- **Petal White** (#ffffff): Used for card surfaces to provide clarity and breathability.
- **Dusty Rose** (#fdf0f5): The page background that keeps the site feeling warm and unique compared to pure white.
- **Dark Bark** (#4a2d35): The primary ink for text, providing high contrast without the harshness of pure black.

**The Blossom Rule.** Blossom is used for interaction and emphasis. It should be the first thing a user's eye goes to when looking for an action.

## 3. Typography

**Display Font:** Nunito (with Prompt fallback)
**Body Font:** Nunito (with Prompt fallback)

**Character:** The pairing is clean, friendly, and highly legible. Nunito's rounded terminals complement the soft UI elements, while its bold weights provide a professional, structural anchor.

### Hierarchy
- **Display** (800, clamp(2rem, 4vw, 3.2rem), 1.2): Hero headlines and large section titles.
- **Headline** (800, 1.4rem, 1.4): Sub-headlines and card titles.
- **Body** (400, 1rem, 1.6): General prose and descriptions.
- **Label** (700, 0.85rem, normal): Tags, pills, and metadata.

## 4. Elevation

The system uses a "Lifted" philosophy. Depth is conveyed through soft, wide shadows and a slight vertical lift on hover, making the interface feel tactile and responsive.

### Shadow Vocabulary
- **Card Shadow** (`0 4px 24px rgba(220,100,130,0.12)`): Used for all main content containers.
- **Nav Shadow** (`0 8px 32px rgba(220, 100, 130, 0.08)`): A deeper, more ambient shadow for the floating navigation bar.

**The Response Rule.** Surfaces are never static. Every interactable card or button must respond to hover with a vertical lift or a shadow intensification.

## 5. Components

### Buttons
- **Shape:** Full pill (999px)
- **Primary:** Blossom background with white text. High prominence.
- **Outline:** Transparent background with Blossom border and text. Secondary prominence.

### Cards
- **Corner Style:** Large (24px radius)
- **Background:** Petal White (#ffffff)
- **Shadow Strategy:** Lifted with Card Shadow.
- **Border:** Subtle Blossom-light border (1.5px) to define edges on the warm background.

### Navigation
- **Style:** Floating pill with blur (16px) and subtle border.
- **Links:** Soft text with a Blossom underline reveal on active/hover states.

## 6. Do's and Don'ts

### Do:
- **Do** use `clamp()` for all major headlines to ensure responsiveness.
- **Do** maintain the 24px corner radius for all main containers to keep the "soft" brand consistent.
- **Do** use Blossom sparingly for maximum impact.

### Don't:
- **Don't** use pure black (#000000) for text; use Dark Bark (#4a2d35).
- **Don't** use side-stripe borders as colored accents; use full borders or background tints.
- **Don't** use sharp corners; even small elements should have at least a 10px radius.
- **Don't** use generic SaaS blue; stay within the Rose Petal palette.
