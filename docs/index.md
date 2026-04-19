# Pocket Scion External NeoPixels

A beginner-friendly guide to driving an external 9-LED NeoPixel strip from an [Instruo Pocket Scion](https://www.instruomodular.com/product/pocket-scion/).

<!-- TODO: replace with the actual demo recording -->
<video autoplay loop muted playsinline controls preload="metadata" width="100%">
  <source src="assets/demo.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

## The build at a glance

```
                    ┌──────────────┐
 USB ──────────────▶│ Pocket Scion ├─── DATA ───┐
                    └──────────────┘            │
                                                ▼
                                       ┌──────────────────┐
 USB ───┬── V+ ──[DIODE]──────────────▶│                  │
        │                              │   9 NeoPixels    │
        └── GND ──────────────────────▶│   daisy chained  │
                                       └──────────────────┘
```

## Pages

1. [Overview](overview.md) — what you're building, parts, tools
2. [Building the strip](building-the-strip.md) — soldering the 9-LED chain
3. [Tapping the Scion](tapping-the-scion.md) — exposing and soldering to the data trace
4. [Powering the strip](powering-the-strip.md) — USB cable, diode, final wiring
5. [Troubleshooting](troubleshooting.md) — common failures and further reading

Estimated build time: 2-3 hours if you are comfortable with a soldering iron.
