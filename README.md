# oto One

A scroll-driven 3D product page for **oto One**, a set of fictional wireless headphones. Everything is in one file, [`index.html`](index.html), and the headphones are modelled in code with Three.js, with no 3D assets.

## What happens as you scroll

1. **Hero:** ember-orange headphones over a giant "silence".
2. **Close-ups:** the camera flies to the swap-in badge (which flips to show its other design), the 24 air ports and the headband, with leader-line callouts.
3. **Colourways:** each new colour sweeps across the object with a glowing seam. Cobalt comes with clouds, bubblegum with floating bubbles, lime zest with outline type and ultraviolet with orbit rings.
4. **Exploded view:** the shells, PCB, battery, magnet, driver and cushions separate, with callouts on the internals.
5. **"six colors. one sound.":** six models fan out.
6. **After dark:** onyx shells, gold hardware, moody lighting and a macro shot of the slider.
7. **Gallery:** cards rendered from the same 3D model.
8. **Configurator:** pick a colour, badge and finish, drag to spin, add to bag.
9. **Footer:** a giant wordmark.

## Stack

- [Three.js](https://threejs.org) 0.160: a procedural model, plus a custom `onBeforeCompile` shader for the colour wipe.
- [GSAP](https://gsap.com) 3.12 + ScrollTrigger: a single scrubbed master timeline.
- [Lenis](https://lenis.darkroom.engineering) 1.1: smooth scrolling.

All libraries load from public CDNs, so there's no build step.

## Run locally

```bash
python -m http.server 8768
```

Then open http://localhost:8768.
