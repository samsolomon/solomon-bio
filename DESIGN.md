# Sam-as-a-Service — V7 reference layout

User-selected reference https://www.v7labs.com/, inspected in Orca via DOM/computed styles and desktop/mobile screenshots. Replaces the prior Califa structure.

## Tokens and fonts
White #fff; ink #292929; secondary #737373; panel dividers #f4f4f4. Geist Serif original Regular self-hosted for display; Inter Variable for body/UI. Original font file lacks liga/dlig; CSS enables supported ligatures and kerning without synthetic styling.

## Reference measurements
1440px desktop: 52px horizontal gutters; 36px announcement; roughly 60px navigation; 54px hero heading; 48px section headings. Wide, airy centered hero followed by proof strip, three service panels, statement, two-column feature grid, resources and footer. Mobile reference uses 32px hero and 24px sections; implementation uses 36px/32px for the Sam copy and readable hierarchy.

## Implementation
Sticky navigation with native details menu on mobile. Pill buttons, fine borders, open white surfaces. Four explicitly labeled product-image placeholders and two resource-image placeholders. Sam's three pricing tiers retained. No borrowed customer claims, logos or testimonials. All actions lead to real email links, page anchors or solomon.io.

## Verification
Production build passes; desktop and 390px mobile inspected; no mobile horizontal overflow or broken fragment links. Geist Serif loads. Nothing published.

Global typography rendering uses `text-rendering: optimizeLegibility`, `-webkit-font-smoothing: antialiased` and `-moz-osx-font-smoothing: grayscale`.

## Hero transformation animation
Three.js orthographic canvas with a tapered helical coil mesh entering from the left and flat-faceted diamond geometry exiting right. 18 shared-geometry items, muted translucent materials, 23-second cycle, central convergence and fade preserve headline readability. Pixel ratio capped at 1.5. Pointer-transparent layer behind text; continuous playback with no controls (user preference), reduced-motion static composition, IntersectionObserver and visibility-based suspension. No downloaded model or raster asset. Three.js adds a sizeable client bundle; the HTML content remains independent of rendering.

Coil revision: broader tube, reduced vertical rise, buried starting end and short tapered tip. Adjacent turns overlap to create a squat pile instead of an open spring.

Transparency revision: meshes now render opaque with depth writing, hiding interior overlapping surfaces. The composed canvas fades to 24% desktop / 16% mobile opacity. A spatial mask fades near the center and edges; no per-mesh transparency. Coil material is softer and less metallic. Geometry unchanged in this pass to assess the transparency improvement independently.
