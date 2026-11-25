# KHAN: Drag-the-queue lookbook hero

By @abdomahrous.design on Instagram.

**Live demo:** https://abdogfx92.github.io/nauta-liquid/khan/

Or download `index.html` and open it in your browser, then drag the queue.

## The prompt

```
KHAN: Depth Queue Lookbook (full prompt)

Build a single-file lookbook hero (one index.html, no libraries, all CSS and JS inline, images inlined as base64) for a Cairo streetwear brand called KHAN, "Cairo Drop 01".

THE QUEUE
- Six full-body models shot with the same camera, backdrop and light: [MODEL 1] … [MODEL 6]. Cut out the backgrounds, align every figure's feet to the same baseline, keep their real relative heights.
- Stand them in a queue that recedes into depth: the front model large and sharp at about 30% of the stage width; each one behind is ~0.74× the size of the one in front, its feet sit closer to a horizon line, it drifts up and to the right, and it gets softer: CSS blur growing ~2.6px per step, slightly desaturated and lighter. Fade the fifth one out so the queue seems to go on.
- Drag (mouse, touch), wheel or arrow keys move the queue as one continuous value with momentum; on release, snap to the nearest look. The queue loops forever.
- The front model exits to the left: it grows to ~1.38×, slides off, fades, with a horizontal motion blur (SVG feGaussianBlur with stdDeviation "x 0") that peaks mid-exit.
- Soft contact shadow under every figure, a warm concrete-grey backdrop (#E7E3DC) with a light pool top-left and a subtle film grain.

THE PAGE
- Top bar: links (Drop 01, Archive, Stores) on the left, the KHAN wordmark in a wide grotesk in the centre, Sign in / Search / Bag (0) on the right.
- Left rail (23% wide): product cards, two per look (ghost-mannequin garments and shoes on white, name + EGP price, ♡ and +). The rail scrolls in lockstep with the queue: one look of drag = two cards.
- Top right: "Shubra · Cairo", a big wide "CAIRO DROP 01" and two lines of copy.
- Bottom right: the look name in an italic serif and "LOOK 01" in wide caps. Both roll up to the next value on every change. Then "Shop the look" and six progress ticks.
- A custom pill cursor "‹ ›" over the stage that widens while dragging.

MOBILE (under 760px)
- Hide the rail and the links, make the stage full width, put the title top-left and the look block bottom-left, and drive the queue with swipes.
```
