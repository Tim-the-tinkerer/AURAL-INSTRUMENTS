# AURAL INSTRUMENTS

**Procedural sound systems for the browser.**

AURAL INSTRUMENTS is a collection of **17 self-contained generative instruments and soundscapes** built around the Web Audio API. Each instrument is a different sonic environment, with its own controls, behavior, visual identity, and procedural audio engine.

The entire collection lives inside one HTML **cabinet**. Launch any instrument in its own tab, extract one complete standalone HTML file, or download all 17 instruments together as a ZIP archive. No build system, server, or companion asset folder is required.

## What Is AURAL?

AURAL is less a conventional synthesizer collection than a set of small procedural worlds.

Instead of playing a song or a fixed soundtrack, its instruments generate sound using combinations of oscillators, noise, filtering, modulation, drones, pulses, spatial effects, and evolving events. The instruments range from musical ambience to simulated environments, fictional organisms, spectral presences, and machines.

Most instruments use text seeds and deterministic pseudo-random generation, often through the collection's experimental **SplitMix1024** design. A seed can define a reproducible *procedural character*—though the exact audible performance may also depend on settings, timing, browser, and audio device. SplitMix1024 is an artistic, non-cryptographic generator.

**A deliberate exception is K-7 Kite.** The cabinet now contains the **original K-7 REV D** sound engine, not the later SplitMix or SplitMix1024 adaptations. That original version uses non-seeded random variation and is not intended to recreate an identical performance from a seed.

## The Collection

| Model | Instrument | Character |
|---|---|---|
| **C-1** | **Continuum** | A synthetic-consciousness soundscape of resonant substrate, uneven clock pulses, FM packets, melodic memory, harmonic thoughts, restrained glitches, and long-form evolution. |
| **D-9** | **Wyrm** | A dragon and its cavern: stone drips, hoard movement, embers, flame, storm pressure, subterranean pulse, and creature calls ranging from purrs to shrieks. |
| **F-1** | **Frequency** | Musical ambient piano with six presets, including the preserved Original mode; harmonic fields, chord cycling, and a circular audio visualizer. |
| **G-1** | **Ghostline** | High-speed cyberpunk atmosphere built from pursuit rhythms, pressure bass, fractured leads, neon textures, and evolving tension. |
| **I-9** | **Ironworks** | An industrial generative organism of furnace pulses, iron impacts, rotary drones, abrasion, electrical residue, and factory resonance. |
| **K-7** | **Kite** | The **original REV D** ambient console: drones, plucks, rain, pulses, chimes, wind, swells, and organic, non-SplitMix variation. |
| **O-1** | **Clay** | An ocarina-inspired instrument shaped by breath, gliding pitch, ambient drift, drone, and a quiet wind-temple atmosphere. |
| **P-4** | **Phantoms** | Ghostly rooms, whispered presences, spectral bells, distant movements, apparitions, and seeded supernatural ambience. |
| **P-7** | **Flux Core** | A fictional energy reactor with subharmonic pressure, evolving field harmonics, resonant heartbeat, energy surges, controlled shutdown, and an **Overload** preset. |
| **R-1** | **Rune (Rite)** | A virtual ritual ensemble with deterministic motifs, deep drone drift, evolving events, and ceremonial atmosphere. |
| **S-1** | **Snipes** | Dark ambient drones, unstable overtones, filtered air, distant impacts, subdued pulse, and a long-form seeded sonic identity. |
| **T-1** | **Ether** | An expressive field instrument: glide through pitch and volume, shape timbre and space, add drone, or let Drift generate slow gestures. |
| **T-1** | **The Tell-Tale Heart** | A five-chapter Poe-inspired musical soundscape of piano, heartbeat, dread, and growing psychological tension, with a Full Tale mode. |
| **U-1** | **Umbrella** | A canopy of tone and changing weather, where rain produces droplets and pulses while shelter, wind, and distance shape the sound. |
| **W-4** | **Womb** | A sealed organic instrument: one heartbeat, amniotic low-pass warmth, blood-flow noise, and slow cellular harmonic changes. |
| **X-1** | **Xenolith** | A strange extraterrestrial sound organism of magnetosphere hum, tendon drones, ion rain, vacuum choir, mutation, and alien physiology. |
| **X-9** | **Night Signal** | Paranormal long-form synthesis: drones, motifs, noise, pulse, missing-time ambience, forest signals, black sites, and archive anomalies. |

### Added in This Update (F-1, T-1, W-4)

**F-1 · Frequency** preserves the original Frequency piano and five-chord cycling as its **Original** preset, and adds five further ambient sound modes. Its circular visualizer, manual keyboard, variable cycle speed, warmth, space, stereo motion, master volume and seeded variation remain within a single independent HTML file.

**T-1 · The Tell-Tale Heart** is a five-chapter musical narrative inspired by Edgar Allan Poe. Its gentle heartbeat, piano, and gradually unsettled harmonies convey the tale without narration, sudden loud impacts, or sampled sound effects. Choose a scene or let **Full Tale** progress through the chapters.

**W-4 · Womb** creates a warm, sealed organic environment. A heartbeat anchors low-pass amniotic textures, filtered blood-flow noise, and slowly shifting harmonic ratios. The included W-4 is kept exactly as supplied.

**Model-code overlap:** the existing **T-1 Ether** and new **T-1 The Tell-Tale Heart** both use the model identifier **T-1**. Neither instrument was renumbered or modified. The cabinet now routes launch and extraction using each file's unique filename, so both cards and both downloads work separately. Their existing model labels remain unchanged.

### Earlier Additions (P-4, P-7)

**P-4 · Phantoms** is a spectral soundscape with scene presets and controls for Presence, Restlessness, Distance, the Veil, Dread, and Drift. It also offers actions to summon a presence or call into the dark, plus incarnation saving/loading and audio recording. Its illustrated haunted environment is a still scene, avoiding continuous visual animation.

**P-7 · Flux Core** is a fictional reactor rather than a conventional musical instrument. Its startup builds into a low-midrange heartbeat and surrounding field textures. It includes ignition timing, energy and instability controls, field motion, spectral glow, spatial depth, Thrum Strength, Pulse Cadence, Energy Surge, recording, and patch import/export. Its shutdown winds down the core and heartbeat over approximately nine seconds.

P-7 includes the finalized **Overload** preset: the principal sound controls and master volume are set to maximum, while Ignition Time is reduced to its minimum of **4 seconds**. The core's simulated field flux and harmonic shear respond dynamically to this high-energy configuration.

### K-7 Version Choice

K-7 is intentionally **not** the later SplitMix1024 adaptation. The original **REV D** edition was restored because its earlier musical behavior was preferred. The cabinet preserves that engine and interface instead of modifying it to follow the newer instruments' seeded architecture.

## Cabinet Features

- **17 complete procedural instruments** in one HTML file.
- Searchable instrument cards, each with its own model, description, and controls. Each card routes by its unique filename to prevent model-code collisions.
- **Launch Instrument** opens an independent instrument experience in a separate tab.
- **Extract Standalone HTML** reconstructs and downloads an individual instrument.
- **Extract All (.zip)** exports all 17 standalone HTML files at once.
- Embedded instrument code, visuals, and required assets; no external audio samples or backend.
- A **shared internal font bank** removes redundant embedded font data from the cabinet without changing the standalone output.
- Shared internal **DOWNLOAD**, **RECORDING**, and **PATCH** helpers are restored into participating instruments during launch or extraction.
- Runs locally or from static hosting such as GitHub Pages.
- No package manager, compilation step, or external ZIP library.

## Running AURAL

### Open the Cabinet

Open `AURAL_INSTRUMENTS.html` in a modern browser. The collection can also be renamed `index.html` for static hosting.

Search or browse the instrument cards, then select **Launch Instrument ↗**. The chosen instrument opens as a complete HTML experience in a new tab. Use its **Power**, **Start**, **Awaken**, **Ignite Core**, or equivalent control to begin audio.

Browsers generally require a direct user gesture to start Web Audio, so instruments do **not** automatically make sound when a page loads. Allow pop-ups if your browser blocks opening an instrument tab.

### Extract One Instrument

Select **Extract Standalone HTML ↓** on any instrument card. The cabinet reconstructs the instrument and downloads an independent `.html` file.

For example:

- K-7 exports `AURAL-K7-Kite-REV-D-self-contained.html`.
- P-4 exports `AURAL-P4-Phantoms-SplitMix1024.html`.
- P-7 exports `AURAL-P7-Flux-Core-Overload-SplitMix1024.html`.
- F-1 exports `AURAL-F1-Frequency.html`.
- T-1 The Tell-Tale Heart exports `AURAL-T1-The-Tell-Tale-Heart.html`.
- W-4 exports `AURAL-W4-Womb.html`.

Each extracted HTML file includes everything needed to run that instrument independently of the cabinet.

### Extract the Entire Collection

Select **Extract All (.zip)** in the cabinet toolbar. This downloads:

`AURAL-INSTRUMENTS-Standalone.zip`

The archive contains **17 individual HTML files**. ZIP entries use the uncompressed **STORE** method so the cabinet can create the archive using its own JavaScript without third-party libraries. The extracted instruments do not need the original cabinet or a shared assets directory. All instrument filenames are distinct, including the two instruments labeled T-1.

Downloads are initiated within the browser. Some browsers may ask you to allow multiple downloads or downloads originating from a local file.

### Host on GitHub Pages

The cabinet is a static HTML document; no hosting runtime is required.

1. Add `AURAL_INSTRUMENTS.html` to your repository and link directly to it, **or** rename it `index.html` to make it the Pages landing page.
2. Publish the repository through GitHub Pages.
3. Open the published page and launch instruments normally, subject to the browser's audio and pop-up policies.

## Seeds and Procedural Variation

In instruments that support them, seeds may affect tuning, rhythm, drone behavior, timbre, filters, spatial position, event probability, density, melodic motifs, mutation, or atmospheric evolution.

Using the same seed and settings is intended to recover a recognizable underlying procedural identity. **That does not necessarily mean a sample-for-sample identical recording.** Timing, user interaction, audio scheduling, and rendering can influence the final performance.

Not all instruments work the same way. In particular, **original K-7 Kite is non-seeded and non-SplitMix**. Its variation is a feature of its original sound engine rather than a repeatable seed system.

The custom SplitMix1024 generators are for creative variation and **must not be treated as cryptographically secure random-number generators**.

## Shared Fonts and Standalone Integrity

The cabinet keeps **six WOFF2 font resources** in a central internal bank rather than storing redundant copies inside multiple embedded instrument payloads.

These resources are used by **K-7 Kite**, **O-1 Clay**, and **T-1 Ether**. When one of these instruments is launched or extracted, the cabinet reinserts the corresponding font data into its HTML document. The same restoration routine is used by launch, individual extraction, and ZIP extraction.

As a result:

- The **cabinet** benefits from deduplicated fonts.
- Each **launched instrument** still receives its full font definitions.
- Each **extracted HTML** is self-contained, with no missing fonts or external companion files.
- The individual instruments retain their own original layouts and sound engines; participating instruments now contain restored utility helpers.

The utility-library refactor retains this shared-font architecture. Font reconstruction and utility reconstruction use the same export path, keeping every standalone HTML independent.

## Shared Utility Libraries (Initial Refactor)

Alongside the existing shared-font bank, this edition introduces three small **internal JavaScript helper libraries**. These are stored once in the cabinet and inserted directly into participating instruments when they launch or are extracted:

| Library | Scope | Instruments using it |
|---|---|---|
| **DOWNLOAD** | Browser Blob download, temporary URL creation, link cleanup, and delayed URL revocation. Each instrument keeps its original filename and cleanup delay. | C-1, O-1, P-4, P-7, T-1 Ether, W-4 |
| **RECORDING** | Selects output filename extensions for recorded audio (`.webm`, `.m4a`, `.ogg`) from the recorder's MIME type. | C-1, P-4, P-7, W-4 |
| **PATCH** | JSON serialization and parsing used by instrument-specific preset, identity, and patch persistence. | C-1, O-1, P-4, P-7, S-1, T-1 Ether, W-4 |

**Deliberately unchanged:** the synthesis engines, `MediaRecorder` start/stop handling, codec preference lists, recording streams, event and audio scheduling, presets and their values, existing patch schemas, per-instrument validation, and instrument-specific import/export behavior. K-7 Kite remains its original non-SplitMix version. The two T-1 instruments keep their existing identities.

The new library is a **small, conservative foundation**, not a replacement for each instrument's recording or patch manager. In particular, encoding still uses the formats supported by the browser's native `MediaRecorder`; these helpers do not add an audio encoder or new export format. The refactor intentionally does not merge differing patch formats.

The cabinet restores the utility code at launch, individual extraction, and Extract All time, **after restoring shared fonts**. Each exported HTML includes its own utility definitions; no external JavaScript files, server, or network connection are required. Participating exports have updated source bytes because helper calls are embedded, but preserve their existing patch data formats.

This first pass is intended to establish a safely reusable architecture rather than reduce size dramatically. Modest overhead from shared-library metadata and reconstruction is expected; future deduplication should be evaluated on measured savings and regression tests, not presumed to improve musical behavior.

## Design Philosophy

AURAL is intentionally **not** a DAW, a sample library, or a set of pre-rendered tracks. Each instrument explores a particular idea:

- Can a fictional life-form or digital consciousness have a convincing sonic presence?
- Can a dragon, a ritual, rainfall, or an abandoned haunted room become a living acoustic environment?
- Can industrial machinery or an impossible energy reactor sound physically suggestive without relying on recordings?
- Can a sparse paranormal signal or a dark-ambient world evolve without becoming a conventional song?

The goal is not perfect predictability or maximal technical complexity. It is a distinctive world capable of sustaining its atmosphere while continuing to change.

## Browser and Playback Notes

AURAL is primarily designed for **foreground browser playback**. Modern desktop browsers with Web Audio support—such as Safari, Chrome, and Firefox—typically offer the most reliable experience.

Mobile devices may impose limitations on audio processing, especially when the browser is backgrounded or the screen is locked. **Background playback and lock-screen playback are not guaranteed.** Browser policy may also restrict pop-up tabs, recording features, or locally initiated downloads.

For audio issues, first test one standalone instrument in a current desktop browser, confirm that its power control was activated, and check the system output volume. Start with moderate volume, particularly for bass-heavy or intense instruments such as P-7.

## Performance

The instruments differ considerably in complexity. Some use relatively sparse drones and occasional events; others synthesize numerous interacting oscillators, filters, effects, or procedural voices.

Visual designs generally favor still backgrounds or modest updates over continuous high-load animation. CPU usage, audible latency, and power consumption nevertheless depend on the instrument, browser, audio hardware, and device.

## Project Files

```text
AURAL_INSTRUMENTS.html
README.md
```

The cabinet carries all **17 instrument payloads** internally. It can launch or export them without a companion directory. Extracted instruments remain independent single-file applications.

## Experimental Project

AURAL is a creative-coding and procedural-audio experiment. The instruments are meant to be explored, adjusted, listened to, and sometimes allowed to become strange.

Some are musical; others are intentionally eerie, mechanical, unstable, organic, or ambiguous. Those differences are the character of the collection.

---

**AURAL INSTRUMENTS**  
*Procedural sound systems for the browser.*
