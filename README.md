# Articulink Brand Guidelines

The cleaned-up, canonical written brand guidelines for Articulink. Everything
here is expressed in code by the
[`@articulink/brand`](https://github.com/jordyhunsaker/articulink-brand)
package on GitHub Packages — install that in your project rather than
copy-pasting values from these pages. The interactive version of this guide
is the [Articulink/brand](https://github.com/Articulink/brand) site
(design.articulink.com).

## The brand in one paragraph

Articulink connects families with speech-language therapy that feels warm,
clear, and encouraging. The visual identity is an "ocean journey": a blue
scale from Cloud and Breeze down to Abyss and Trench, led by **Tide**
(#037DE4), accented sparingly with **Sunshine** (#FCDE1E), set in **Nunito**
for headings and **Poppins** for everything else, with playful rounded
shapes and gentle motion. Light mode is the preferred style; dark mode is a
user preference.

## Guide

| Section | Contents |
|---|---|
| [Color](guide/color.md) | Core palette, Ocean Journey blue scale, accents, UI feedback, dark mode, contrast rules |
| [Typography](guide/typography.md) | Nunito / Poppins / Caveat, weights, type scale, usage |
| [Logo](guide/logo.md) | Wordmark usage, clear space, minimum sizes, don'ts, asset files |
| [Voice & writing](guide/voice.md) | Voice traits, tone by audience, writing tips |
| [Foundations](guide/foundations.md) | Spacing, radius, breakpoints, motion, accessibility |
| [UI components](guide/components.md) | The component inventory and CSS-only classes the package ships |

## Using the brand in a project

```bash
npm install @articulink/brand
```

```css
@import "@articulink/brand/css/index.css";      /* tokens + base + components + animations */
@import "@articulink/brand/css/tailwind.css";   /* Tailwind v4 apps only */
```

```ts
import { colors, typeScale, motion } from "@articulink/brand";
```

See the [package README](https://github.com/jordyhunsaker/articulink-brand#readme)
for registry auth setup (GitHub Packages needs a `read:packages` token) and
full usage.

## Changing the guidelines

Values (a hex, a duration, a font) change in
[`tokens/tokens.json`](https://github.com/jordyhunsaker/articulink-brand/blob/main/tokens/tokens.json)
in the package repo — these pages describe *how* to use them, and should only
need editing when the rules themselves change. When a rule changes, update
both this guide and the brand site.
