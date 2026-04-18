# Troubleshooting

## Quick diagnosis

**Nothing lights up.** Diode is almost certainly backwards, or the USB cable isn't plugged in. Check the band direction first (it must face the LEDs), then check the cable.

**LEDs flicker or show wrong colors.** Both USB cables aren't on the same dual-port power source. Fix that and retest. If the problem persists, measure V+ on the LED strip — it should read ~4.3V. If it reads ~5V, the diode is bypassed or shorted.

**Some LEDs work, others are dark.** Broken chain. The failure point is the joint right after the last working LED. Reflow the V+, GND, or DOUT-to-DIN connection there.

**Red and green work but no blue, or LEDs dim after a while.** Undervoltage. Measure V+ under load — if it's significantly below 4.3V, the diode or the USB power source is underspec'd. Try a known-good 1A+ USB source.

**LEDs stay dark even though the Scion is powered.** They have power but no data arriving. Either the DATA wire is broken, the Scion isn't powered, or the scraped trace isn't actually the data trace.

## Further reading

- [Adafruit NeoPixel Überguide](https://learn.adafruit.com/adafruit-neopixel-uberguide) — everything about NeoPixels
- [Tips for Troubleshooting NeoPixel Glitches](https://blog.adafruit.com/2016/10/28/tips-for-troubleshooting-neopixel-glitches/) — the blog post that explains the voltage rule behind the diode
- [Adafruit's Guide to Excellent Soldering](https://learn.adafruit.com/adafruit-guide-excellent-soldering) — if you need to brush up before you start