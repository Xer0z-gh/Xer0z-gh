# Tanner

I build automations, internal tools, browser extensions and desktop apps, and hand
over the finished thing: software that runs, with a written record of what was
tested and what was not.

Available for contract work. Fixed price, written updates, no calls, paid trial
task first, source included.

---

## Shipped

| Project | What it does | The number |
| --- | --- | --- |
| **[Pulse](https://github.com/Xer0z-gh/Pulse)** | Music discovery over internet radio. Logs what each station broadcasts, resolves artists against MusicBrainz, and profiles the station from what it played, not its directory tags. | Measured 2026-09-16: **417,992 plays heard across 27,977 stations**, producing **31,140 genre links no station listed for itself** (and 6,181 where listening confirms the station's own tag). |
| **[Launch Deck](https://github.com/Xer0z-gh/Launch-Deck)** | A local control centre that detects what a project is, works out how to start it, then runs, supervises and stops it. 32 runner definitions. Supervision on Windows Job Objects, so nothing survives a kill. | **353 Rust tests and 14 browser suites.** A readiness check reports 16 of 56 registered projects blocked, each with the cause and the repair. |
| **[VideoForge](https://github.com/Xer0z-gh/Video-Forge)** | One command turns a brief into a rendered, captioned, loudness-normalized MP4 with thumbnail, titles and chapters. Every edit is a typed, invertible, journaled operation. | **211 tests pass** (2026-09-15): caption timing and grouping, SRT/ASS emit, script parsing, chapters, project persistence. Word-level TTS timestamps drive the captions, so cutting a word from the transcript cuts it from the video. |
| **[Vesper](https://github.com/Xer0z-gh/Vesper)** | A 13-module sound design plugin: reorderable effects rack, 17 saturation algorithms, linear-phase match EQ, shimmer reverb. VST3 and standalone. | **All 13 modules together run at 26x realtime**; the editor opens in 2.5 ms; pluginval passes at strictness 10 across 5 sample rates and 7 block sizes. |
| **[Coupon Hunter](https://github.com/Xer0z-gh/Coupon-Hunter)** | Browser extension that finds checkout codes, types each candidate, watches the order total react, and keeps the one that drops it most. It never clicks anything that places the order. | **~20 sources queried in parallel**, answered at a 1.2 s cutoff. On the benchmark checkout (12 codes, winner 6th), time to discount went from 19.1 s to 5.1 s. |

Stack across these: **Rust** (Tauri), **Python**, **TypeScript/React**,
**C++** (JUCE). Windows-first, local-first.

---

## How a job runs

1. **You describe the outcome**: the thing you want to be true when it's done. A spec is optional.
2. **A small paid trial task, $60-100**: the smallest piece of your problem with a result you can check yourself.
3. **Fixed quote for the real work**, agreed before I start. The number doesn't move unless the scope does.
4. **You get software that runs, plus its source**, and a written handover covering what was tested and what was not.

---

## How the work is checked

Nothing is reported done until it has been run. Every number in the table above
comes from a test run or a live measurement, and the output goes in the handover
alongside the code. Where something could not be run, the handover says so and
says why. A claim nobody exercised is not a result.

Not on offer: hourly work, calls or live interviews, or reviewing someone else's
code without building anything.

---

**Written enquiries:** tanner8206@gmail.com

<sub>Source in these repositories is published so you can check the work. Each repository states its own licence.</sub>
