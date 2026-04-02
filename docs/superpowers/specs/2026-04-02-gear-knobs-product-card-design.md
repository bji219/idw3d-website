# Design: Automation Gear Knobs Product Card

## Summary

Add a new product card to the IDW3D website for the "Automation Gear Knobs for OP-1 Field" Etsy listing. Follows the existing product card pattern with a minor enhancement: two distinct lists (package contents + features) to reflect the product's natural structure.

## Scope

Single file change: `index.html`. No new CSS required — existing `.product-card`, `.product-gallery`, `.product-features`, and `.product-link` styles cover everything needed. A small inline label (`<strong>In the box:</strong>`) distinguishes the two lists without new CSS classes.

## Image Assets

HEIC source files converted to JPEG:
- `images/products/gears/gears-1.jpg`
- `images/products/gears/gears-2.jpg`
- `images/products/gears/gears-3.jpg`
- `images/products/gears/gears-4.jpg`

## Card Structure

```
product-card
  product-tag:       "OP-1 Field"
  product-name:      "Automation Gear Knobs for OP-1 Field"
  product-gallery:   data-gallery="gears", 4 slides (gears-1..4.jpg), 4 dots
  product-description:
    "Experiment with sound design and live performance by mixing and
     matching gear ratios to connect synthesizer parameters and effects."
  "In the box:" label + ul.product-features:
    - Set of 4 hex-knobs (one complete set for your OP-1 Field)
    - Set of 16 interchangeable automation linking gears (10, 12, 15, 18, and 20 teeth)
    - Set of 4 offset collars (for compound gear trains)
  "Details:" label + ul.product-features:
    - Over 100 possible gear configurations
    - Designed specifically for the OP-1 Field
    - 3D printed from durable PLA filament, built for daily use
    - Link effects and synth parameters for hands-free performance
    - Tweak multiple parameters simultaneously and change rates with the gears
  product-link:
    href: https://www.etsy.com/listing/4482086859/op-1-field-gear-knobs-3d-printed
    text: "View on Etsy →"
```

## Placement

Inserted after the existing "Retro Analog Synth Knobs for OP-1" card (line ~900 in index.html), before the "OP-1 x Korg SV-Series Synth Riser" card. Both are OP-1 accessories so grouping them together is logical.

## Gallery JS

The existing gallery JavaScript uses `data-gallery` attribute for initialization — no changes needed. Adding `data-gallery="gears"` on the new card is sufficient.
