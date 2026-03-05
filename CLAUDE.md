# CLAUDE.md — Site Nyres Edim

Landing page + páginas internas para Nyres Edim, terapeuta Pathwork® (BH). Conversion-focused: cada seção direciona para WhatsApp. Static only, NO SSR.

**Goals:** Lighthouse 95+, mobile-first, accessibility AA, tom acolhedor e profissional.

## Stack

- Astro 5.18 (static) + `@astrojs/sitemap`
- Tailwind CSS v4 via `@tailwindcss/vite` (NOT `@astrojs/tailwind`)
- Deploy: Vercel (auto-deploy via GitHub)
- NO React/Vue/Svelte/islands

## Styling

ALL Tailwind config lives in `src/styles/global.css` via `@theme`. There is **NO `tailwind.config.js`**.

Color tokens: `teal-deep`, `teal`, `teal-light`, `teal-soft`, `brown`, `brown-light`, `sand`, `cream`, `warm`. Extracted from Nyres' real brand identity (logo, Instagram, professional photos).

Fonts: `font-serif` (Cormorant Garamond) for headings, `font-sans` (Lato) for body.

Rules:
- Inline Tailwind classes only — NO `@apply`
- Import global.css ONLY in `Layout.astro`
- Use only `@theme` color tokens — no hardcoded hex in components

## Components

All `.astro` files in `src/components/`. Most use inline data (no props). Props only when receiving external data.

Standard section pattern:
- `<section>` with `id`, `py-16 md:py-28`
- Container: `mx-auto px-6 max-w-6xl`
- Semantic HTML: `<section>`, `<nav>`, `<main>`, `<footer>`

Images: use Astro `<Image>` component with descriptive `alt` in Portuguese when possible. Photos in `public/images/`.

## Animations

CSS-only micro-animations defined in `global.css`:
- `reveal`, `reveal-left`, `reveal-right`, `reveal-scale` — scroll-triggered via Intersection Observer
- `stagger` — children appear sequentially (100ms delay)
- `photo-zoom` — 5% scale on hover
- `card-lift` — translateY(-6px) + teal shadow on hover
- `btn-glow` — light sweep on hover
- `pulse-cta` — subtle shadow pulse on main CTA
- `float` — gentle float animation (WhatsApp button)

**ALWAYS** respect `prefers-reduced-motion` — disable animations for users who prefer reduced motion.

## JS Policy

Client JS allowed ONLY for:
1. Intersection Observer (scroll-reveal animations)
2. Header scroll shadow effect
3. Mobile menu toggle

NO frameworks, NO heavy bundles. All JS in `<script>` tags inside .astro files.

## Accessibility

- Semantic HTML elements
- `aria-label` on icons/buttons
- Descriptive `alt` text (Portuguese)
- Focus rings: `focus:ring-2 ring-teal-deep`
- Keyboard navigable CTAs
- `prefers-reduced-motion` respected

## Performance

- Astro `<Image>` for optimized images
- `loading="lazy"` below the fold, `loading="eager"` for hero
- Preload critical fonts
- Static output only — no SSR, no client bundles

## SEO

- Portuguese meta tags + Open Graph in `Layout.astro`
- JSON-LD schema (therapist/local business)
- Canonical: `https://nyresedim.com.br`
- Sitemap via `@astrojs/sitemap`
- robots.txt in `public/`

## Conventions

Commits: `feat:` / `fix:` / `refactor:` prefix.

**NEVER:** create `tailwind.config.js` | use `@astrojs/tailwind` | add frameworks/islands | use `@apply` | hardcode colors outside `@theme`

**ALWAYS:** semantic HTML | Astro `<Image>` when possible | inline Tailwind | mobile-first (`sm:` up) | verify build: `npm run build`
