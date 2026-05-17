# Oldpainless CRT Shaders for WRGB WOLED Panels (v32.0)

These presets are engineered strictly for 4K self-emissive WRGB WOLED panels (tested on the Sony KD-55A85), bypassing sterile digital computer monitor rules to capture true analog light-field cavity rebound mechanics.

## Key Optimizations
* **Hard-Locked Subpixel Purity:** `smoothmask` is held tightly to preserve un-diluted color chemistry and first-glow volume.
* **Symmetric Phase Alignment:** `s_sharp` acts as a horizontal-only phase filter to crush non-integer aspect scaling waves (e.g., PC Engine 256px) inside the gun pass, keeping vertical scanline trenches perfectly dark and deep.
* **WRGB Gate Alignment:** Modified phase windows absorb the horizontal spatial offset caused by the panel's physical White subpixel gate, releasing massive 3D optical pop.
* **High-Fidelity Grid Alignment:** Uses custom viewport mapping to eliminate standard down-sampling, locking rendering to full resolution for pixel-perfect triad alignment.
* **Insulated Pipeline Processing:** Chains the multi-pass layout to protect color chemistry profiles from mid-stream compression, ensuring high-contrast scanlines.


## 🎨 3D Color LUT Chemistry Mapping
The included 1024x32 color stripe files handle the non-linear analog color spaces of the original monitors:
* `astro-nanao-chemical.png` translates the high-vibrancy, wide-gamut arcade P22 phosphor saturation of the Nanao MS9 board.
* `trinitron-lut.png` secures the tight, clinical D65 reference broadcast colors of the Sony XBR chassis.
* **Pipeline Protection:** These textures are loaded natively inside `Pass 5 (LinearizePass)`. By eliminating vertical gun defocus row-bleeding and digital sharpness overshoots downstream, the raw RGB vectors are protected from reverse-voltage back-pressure, allowing the panel to display pure, uncompromised color saturation.

## Included Profiles
1. **Sega Arcade Astro City (Nanao MS9-29):** Optimized for multi-sync arcade PCB resolution tracking under a 4K Honeycomb Dot-Mask.
2. **Sony Broadcast (KV-32XBR48):** Optimized for high-rigidity 1:1 Aperture Grille wire mesh definition.



