# AURAL INSTRUMENTS

**Deterministic procedural sound systems for the browser.**

AURAL INSTRUMENTS is a collection of self-contained generative instruments and soundscapes built with the Web Audio API. Each instrument is its own themed sonic environment, with its own controls, behavior, visual identity, and seeded procedural logic.

The complete collection is packaged inside a single HTML cabinet. Launch an instrument as its own complete experience in a separate tab, extract an individual standalone HTML file, or export all twelve standalone instruments in a ZIP archive.

## What is AURAL?

AURAL is less a conventional synthesizer collection than a set of small procedural worlds.

Instead of loading a song or a fixed audio file, each instrument generates an evolving soundscape from rules: oscillators, noise, filtering, modulation, rhythm, spatial movement, events, drones, and deterministic pseudo-random variation.

Most of the collection uses an experimental **SplitMix1024** system to turn a seed into a repeatable sonic identity. The same seed can reconstruct the same underlying procedural character, while the exact rendering may still vary slightly between browsers and audio systems.

SplitMix1024 is used here as a creative deterministic generator, **not as a cryptographic algorithm**.

## The Collection

| Model | Instrument | Character |
|---|---|---|
| **C-1** | **Continuum** | A synthetic-consciousness soundscape of resonant substrate, uneven clock pulses, bright FM packets, melodic memory, harmonic thoughts, restrained glitches, and seeded long-form evolution. |
| **D-9** | **Wyrm** | A dragon soundscape of cavern wind, dripping stone, shifting hoard, embers, flame, storm pressure, subterranean pulse, and a many-voiced creature that bellows, purrs, hisses, and shrieks. |
| **G-1** | **Ghostline** | A high-speed procedural instrument built around pursuit rhythms, pressure bass, fractured leads, neon atmosphere, and deterministic evolution. |
| **I-9** | **Ironworks** | An industrial generative organism of furnace pulse, iron impact, rotary drone, abrasion, electrical residue, and evolving factory resonance. |
| **K-7** | **Kite** | A generative ambient console of drones, plucks, rain, pulses, chimes, wind, swells, and seeded atmospheric variation. |
| **O-1** | **Clay** | An organic ocarina-inspired instrument shaped by breath, gliding pitch, ambient drift, drone, and a quiet wind-temple atmosphere. |
| **R-1** | **Rune (Rite)** | A virtual ritual ensemble and ceremony engine with deterministic motifs, evolving events, deep drone drift, and a ceremonial sound world. |
| **S-1** | **Snipes** | A dark-ambient generator of slow drones, unstable overtones, filtered air, distant impacts, subdued musical pulse, and a 1024-bit sonic genome that unfolds over time. |
| **T-1** | **Ether** | A continuous expressive field instrument for gliding through pitch and volume, shaping timbre and space, adding undercurrent drone, or allowing Drift to generate slow gestures. |
| **U-1** | **Umbrella** | A canopy of tone and changing weather where rainfall produces droplets and pulses while shelter, wind, distance, and seed define the atmosphere. |
| **X-1** | **Xenolith** | A seeded extraterrestrial sound organism of magnetosphere hum, tendon drones, ion rain, vacuum choir, strange motion, mutation, and alien physiology. |
| **X-9** | **Night Signal** | A paranormal synthesis console for long-form seeded cases: drones, motifs, noise, pulse, missing-time ambience, forest signals, black sites, and deep archive anomalies. |

## Features

- **12 complete procedural instruments**
- **Single self-contained HTML collection**
- Deterministic text seeds
- SplitMix1024-driven variation
- Procedural Web Audio synthesis
- Instrument-specific controls and themed interfaces
- No build system required
- No companion asset folder required for the complete collection
- Runs locally or from a static host such as GitHub Pages
- Searchable instrument launcher
- **Extract standalone HTML** for each instrument (all original embedded assets restored)
- **Extract All (.zip)** for a ZIP of the twelve original standalone HTML files, without external ZIP libraries

## Running AURAL

### Directly

Download `AURAL_INSTRUMENTS_Extractable.html` and open it in a modern browser (you can rename the file to `index.html` for hosting).

Choose an instrument from the cabinet, launch it, and use that instrument's Power, Start, Awaken, or equivalent control to begin audio.

Browsers require a user gesture before starting Web Audio, so sound will not begin automatically when the page loads.

### Extracting standalone instruments

Each instrument card offers two actions:

- **Launch Instrument ↗** opens the full instrument in a new tab, as before. These launches use a temporary browser Blob URL.
- **Extract Standalone HTML ↓** downloads the fully reconstructed original instrument as an independent `.html` file. For example, K-7 exports `AURAL-K7-Kite-REV-E-SplitMix1024-PatchFaithful-Atmosphere.html`.

The toolbar's **Extract All (.zip)** button downloads `AURAL-INSTRUMENTS-Standalone.zip`. Its 12 HTML files each work on their own: no launcher, connection, extra assets, or shared-font folder is needed. ZIP entries are stored uncompressed to keep the cabinet dependency-free.

When extracted, fonts from the central bank are automatically reinserted into K-7, O-1, and T-1. All original UI, themes, audio engines, SplitMix1024 code, and font definitions remain intact. The cabinet itself continues to deduplicate fonts internally.

Downloads are initiated entirely within the browser. Depending on the browser, you may need to allow downloads for the local HTML file.

### GitHub Pages

AURAL works well as a static GitHub Pages project because the collection does not require a backend or build process.

You can either:

1. Upload `AURAL_INSTRUMENTS_Extractable.html` and link directly to it, or
2. Rename it to `index.html` if you want the collection to be the repository's Pages home page.

## Seeds and Determinism

A seed is more than a random-number input in AURAL. Depending on the instrument, it may influence things such as:

- tuning and scale
- rhythm
- drones
- timbre
- filtering
- spatial placement
- density
- melodic behavior
- event probability
- atmospheric evolution
- mutation

A seed therefore acts more like a **procedural identity** for an instrument.

Re-entering the same seed is intended to reconstruct the same underlying world rather than simply produce another random variation.

## Design Philosophy

AURAL is intentionally not a DAW, sample library, or conventional preset synthesizer.

Each instrument is designed around a specific idea:

- What would an alien organism sound like?
- What would it sound like to exist inside computer code?
- What does a dragon's environment sound like when treated as a living system?
- Can rain, ritual, industrial machinery, paranormal signals, breath, or dark ambience become instruments rather than recordings?

The goal is not strict musical predictability. The goal is a recognizable world that can continue generating believable variation without losing its identity.

## Browser Notes

AURAL is primarily designed for foreground browser playback.

Modern desktop browsers provide the most reliable experience. Mobile browsers can impose additional Web Audio restrictions, especially when the browser is backgrounded or the device screen is locked. Background or lock-screen playback is therefore **not guaranteed**.

If audio behaves unexpectedly, first test the same instrument in a current desktop version of Safari, Chrome, Firefox, or another modern browser with Web Audio support.

## Performance

The instruments vary considerably in complexity. Some are sparse ambient systems; others run many simultaneous oscillators, filters, effects, procedural events, or visual elements.

Performance will therefore vary by instrument and device.

The collection favors procedural audio and atmosphere over heavy animated visualization where possible.

## Project Format

The complete cabinet is distributed as:

```text
AURAL_INSTRUMENTS_Extractable.html
README.md
```

The launcher contains all twelve instrument payloads and requires no companion directory. To avoid duplicated assets, six WOFF2 fonts used by K-7 (Kite), O-1 (Clay), and T-1 (Ether) are stored once in an internal shared font bank. The launcher restores those fonts to each instrument when it opens, preserving the original standalone instrument HTML in the launched tab.

The launched instruments remain complete HTML documents. The **Extract** and **Extract All** functions reuse the same restoration path as launching, so the exported HTML files match the originals byte for byte.

## Experimental Project

AURAL is an experimental creative-coding project. The instruments are meant to be explored, seeded, adjusted, listened to, and occasionally allowed to become strange.

Some sounds are deliberately unstable, eerie, mechanical, non-musical, or ambiguous. That is part of the collection's character.

---

**AURAL INSTRUMENTS**  
*Deterministic procedural sound systems.*
