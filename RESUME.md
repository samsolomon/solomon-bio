# Sam-as-a-Service — shelved homepage exploration

Checkpoint saved November 20, 2026 on `sam-as-a-service-home`.

## Resume

```sh
git switch sam-as-a-service-home
npm ci
npm run dev -- --port 4322
```

The new homepage is `src/pages/index.astro`. Its procedural Three.js hero animation is `src/components/HeroFlow.astro`. Product decisions and design notes are in PRODUCT.md and DESIGN.md.

## Direction

The Sam Solomon Company of Atlanta, presenting Sam-as-a-Service with deadpan SaaS humor. Paid work covers design leadership and sales-team technology. Coffee is free; Enterprise/full-time work is unavailable. Contact links use email until a booking URL is selected.

The current layout follows the spacious white-and-black structure of v7labs.com, replacing an earlier Califa-inspired exploration. Original Geist Serif Regular is self-hosted for headings; Inter Variable handles body and UI. Geist Serif's current file does not contain liga/dlig features, despite CSS enabling ligatures. Image slots are explicitly labeled placeholders.

The hero has compact 3D coil piles flowing left to center, then diamonds exiting right. Models are opaque with depth writing; the whole canvas is faded to avoid internal transparency artifacts. No pause/play control by user preference. Reduced motion renders a static scene; offscreen/hidden animation stops. The last change was the transparency fix; more sculpting of the coil/base may still be desirable.

## Publication

Nothing from this branch has been published. The root index.html is the original live static site. GitHub Pages currently publishes the root of main. The new Astro site requires a Pages build/deployment workflow before release; do not simply merge and assume it will serve Astro's output.

## Remaining work

- Review the last model/transparency iteration and finalize homepage copy.
- Replace placeholders with real assets and select project examples.
- Add booking destination if desired.
- Verify responsive layout, accessibility and reduced-motion behavior before release.
- Review Three.js bundle cost (build warns about a chunk above 500 kB).
- Configure Astro deployment and sitemap/canonical metadata before publishing.

The last production build passed. This is an exploratory checkpoint, not a launch-ready site.
