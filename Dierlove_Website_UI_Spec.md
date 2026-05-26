# Dierlove Website UI Visual Specification

This document defines the visual identity for the Dierlove high-end B2B brand website.

## 1. Brand Concept: "The Silent Strength of Luxury"
- **Keywords**: Editorial, Sophisticated, Trustworthy, Minimalist.
- **Visual Goal**: To look like a premium European brand's official supply chain partner, moving away from "Wholesale/Alibaba" aesthetics.

## 2. Color Palette (Tailwind CSS Codes)

| Role | Color Name | Hex Code | Purpose |
| :--- | :--- | :--- | :--- |
| **Primary BG** | Cream White | `#F7F3EE` | Main page background, provides a "soft luxury" feel. |
| **Secondary BG** | Soft Beige | `#D8C7B5` | Sections, hover states, and card backgrounds. |
| **Text (Heading)** | Deep Charcoal | `#1A1A1A` | All titles and primary text for high readability. |
| **Accent** | Muted Gold | `#C8A27A` | CTAs, icons, and small decorative elements. |
| **Body Text** | Slate Gray | `#7A7A7A` | Descriptions, footer text, and meta information. |

## 3. Typography System

### Heading Font: **Playfair Display** (Serif)
- **Use Case**: Hero headlines, Section titles.
- **Vibe**: Fashion editorial, high-end magazine style.
- **Weight**: Bold (700) or Regular (400) for a classic look.

### Body Font: **Montserrat** or **Inter** (Sans-serif)
- **Use Case**: Navigation, Body text, Buttons.
- **Vibe**: Clean, modern, professional, highly readable on mobile.
- **Weight**: Regular (400), Medium (500).

## 4. UI Components Guidelines

### Buttons
- **Primary**: Black background, white text, sharp corners or very slight rounding (2px), heavy tracking (letter-spacing).
- **Secondary**: Transparent with black border (outline), or Gold text with no border.

### Image Style
- **Model Shots**: High-key lighting, soft shadows, neutral backgrounds. No busy/messy backgrounds.
- **Factory Shots**: Black and white or desaturated tones to emphasize "Expertise" over "Mass Production."

## 5. Tailwind Configuration Snippet
```javascript
module.exports = {
  theme: {
    extend: {
      colors: {
        dierlove: {
          bg: '#F7F3EE',
          beige: '#D8C7B5',
          black: '#1A1A1A',
          gold: '#C8A27A',
          gray: '#7A7A7A',
        }
      },
      fontFamily: {
        serif: ['"Playfair Display"', 'serif'],
        sans: ['Montserrat', 'sans-serif'],
      },
      letterSpacing: {
        widest: '.2em',
      }
    }
  }
}
```
