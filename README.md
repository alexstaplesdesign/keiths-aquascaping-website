# Keith's Aquascaping Services

Website for a local aquascaping business serving the NY/NJ/CT tri-state area.
Services include custom tank design, routine maintenance, koi pond construction,
and natural water restoration.

Live demo: https://alexstaplesdesign.github.io/keiths-aquascaping-website/

## Stack

HTML5 · CSS3 · JavaScript (vanilla) · Gabriel Sans (self-hosted custom font)

## Running it

No build step — open `index.html` in a browser.

## Pages

The homepage (`index.html`) is fully built. The inner pages (`about.html`,
`services.html`, `contact.html`) are currently stubs.

**Homepage sections:**
- Header with desktop nav and hamburger mobile nav
- Hero with background image
- Business overview
- Services preview — Aquascaping Design, Tank Maintenance, Pond & Water Features
  (alternating image/text rows with scroll-triggered fade-in)
- Contact/CTA

## CSS

Self-hosted Gabriel Sans font loaded via `@font-face` with `font-display: swap`.
Color palette uses CSS custom properties:

```css
--color-bg: #F6F1F1;
--color-light-blue: #577BC1;
--color-dark-blue: #344CB7;
--color-yellow: #FFEB00;
```

## JavaScript (`js/main.js`)

- Hamburger nav opens/closes mobile menu; closes on outside click
- Scroll-triggered fade-up animation on `.wwd-fade` elements using
  `IntersectionObserver` — text sections animate as a group when they
  enter the viewport
