# pocket-scion-neopixels

Guide for externalizing the NeoPixel output of the [Instruo Pocket Scion](https://www.instruomodular.com/product/pocket-scion/) to drive an off-board LED strip.

**Read the guide:** <https://ucodia.github.io/pocket-scion-neopixels/>

## What this is

The Pocket Scion has onboard NeoPixels that respond to bioelectric input. This guide shows how to tap the NeoPixel data line and extend the visualization to a separate 9-LED strip, powered via a second USB cable with an inline silicon diode to drop 5V to ~4.3V (required for reliable 3.3V data transmission).

## Local development

This site is built with [Zensical](https://zensical.org/) and deployed to GitHub Pages via the workflow in `.github/workflows/docs.yml`.

```bash
uv sync
uv run zensical serve    # live preview at http://127.0.0.1:8000
uv run zensical build    # outputs to ./site
```

## License

This documentation is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

You are free to share and adapt the material for any purpose, as long as you give appropriate credit.

## Disclaimer

This guide describes a modification that involves permanent changes to your Pocket Scion hardware (scraping conformal coating, soldering to traces). Proceed at your own risk. Not endorsed by or affiliated with Instruo.
