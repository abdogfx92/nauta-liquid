# NAUTA: Liquid Reveal Hero

By @abdomahrous.design on Instagram.

**Live demo:** https://abdogfx92.github.io/nauta-liquid/

Or download `index.html` and open it in your browser, then move the cursor (or touch on mobile).

## The prompt

```
Build a single-file landing page (one index.html, no libraries, all CSS and JS inline) for a freedive club called NAUTA.

HERO
- Full-screen hero with two pixel-aligned photos of the same person, same pose, same light:
  Layer 1 (top): [DIVER IN SCUBA GEAR: hood, mask, regulator]
  Layer 2 (underneath): [SAME DIVER, NO GEAR: face visible, wet hair]
- Run a real-time WebGL2 Navier–Stokes fluid simulation driven by the cursor (and touch on mobile):
  velocity + dye fields, curl and vorticity confinement, divergence, a 20-iteration pressure solve, gradient subtract, advection with slow dissipation.
- Use the dye as a soft mask: where the fluid is, reveal Layer 2 through Layer 1. Smoothstep the edges so the reveal looks like water washing the mask away, not a hard brush.
- Add thin specular streaks from the dye gradient and a slight refraction offset so it reads as water on glass. Keep it subtle and photographic, not white or milky.
- Gentle values: low curl (~12), moderate splat force, small splat radius (slightly larger on mobile), velocity dissipation ~0.9.
- Canvas2D fallback when WebGL2 is not available: a soft blurred trail mask composited with source-in, plus faint sheen streaks. Pause the loop when idle.

LAYOUT (desktop)
- Top nav: wave logo + "NAUTA", links (Club, Divers, Depths, Training, Logbook), blue pill "Book a dive".
- Huge split headline across the face: "DEEP" left in cobalt #1f3fd1, "BLUE" right in near-black, extra-bold wide grotesk.
- Under it: "One breath. All the way down." + pill "Join the club" + "▶ Watch the descent" + a small mono hint "Move to clear the mask".
- Bottom-right card: small underwater thumbnail + mono stats (DIVER 07 / CALLSIGN // COBALT / RECORD // −92 M CWT / SITE // DAHAB BLUE HOLE).

LAYOUT (mobile, under 700px)
- Hide the links and the card. Anchor the headline, the line and the buttons to the bottom, below the face, with a soft dark gradient behind them so the light text stays readable.

Images: inline both photos as base64 so the file works offline by double-click. Flip Y when uploading the textures.
```
