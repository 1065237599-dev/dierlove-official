# Technical Implementation Plan: Dierlove B2B Portal

This plan outlines the technical stack and architecture for building the Dierlove brand-led B2B website using Next.js.

## 1. Core Technology Stack
- **Frontend**: Next.js 14+ (App Router)
- **Styling**: Tailwind CSS (for rapid, responsive UI development)
- **Animation**: Framer Motion (for subtle, high-end transitions)
- **CMS (Optional but recommended)**: Strapi or Contentful (for product management)
- **Deployment**: Vercel (for global edge performance) + Cloudflare (Security/DNS)
- **Analytics**: Google Analytics 4 + Microsoft Clarity (to track heatmaps)

## 2. Information Architecture (Sitemap)
- **`/`**: Home (Hero, Categories, Trust, Reviews)
- **`/solutions`**:
  - `OEM/ODM Service`: Process details
  - `Low MOQ Program`: Targeting startups/boutiques
- **`/products`**:
  - Index: Grid of categories
  - Category Pages: `/products/lingerie`, `/products/swimwear`
  - Detail Pages: Technical specs, MOQ, fabric info (No pricing, lead to inquiry)
- **`/factory`**: Video tours, certification downloads, production capacity
- **`/contact`**: Interactive form, WhatsApp widget, global location map

## 3. SEO Strategy for Lingerie B2B
- **Meta Tags**: Target "Lingerie Manufacturer", "Swimwear OEM China", "Custom Underwear Factory".
- **Structured Data**: JSON-LD for `ManufacturingBusiness` and `Product`.
- **Image SEO**: WebP format with descriptive Alt text.

## 4. Proposed Folder Structure (Next.js)
```bash
/src
  /app
    /layout.tsx       # Global fonts & styles
    /page.tsx         # Homepage
    /products
      /[slug]/page.tsx # Product Dynamic Routes
    /contact
      /page.tsx
  /components
    /ui               # Reusable buttons, inputs
    /sections         # Hero, FactoryGrid, Footer
  /lib
    /cms.ts           # CMS fetching logic
  /styles
    /globals.css      # Custom Playfair/Montserrat imports
```

## 5. Deployment Checklist
1. SSL Certificate configuration.
2. Sitemap.xml and Robots.txt generation.
3. Fast-loading WhatsApp floating button integration.
4. CDN optimization for high-res model images.
