# Tanner

I build automations, internal tools, browser extensions and desktop apps, and hand
over the finished thing: software that runs on your machine, its source, and a
written record of what was tested and what was not.

Available for contract work. Fixed price, agreed before I start. The first thing
you buy is a $60-100 trial task small enough to check yourself, so the cheapest
version of hiring me comes first. Written only, so you keep the record. Source
included, so you are never locked to me.

---

## Shipped

The number beside each project below is that project's own test run or
instrumentation, and the source is here to check it against.

| Project | What it does | The number |
| --- | --- | --- |
| **[Pulse](https://github.com/Xer0z-gh/Pulse)** | Music discovery over internet radio. Logs what each station actually broadcasts, resolves the artists against MusicBrainz, and profiles the station from what it played rather than from the tags it claims. | Read from one running library on 2026-09-16: **418,009 plays heard across 27,994 announcing stations**, producing **31,140 genre links no station ever claimed for itself** (and 6,181 where listening confirms the station's own tag). `cargo test`: **167 tests, 0 failures.** |
| **[Launch Deck](https://github.com/Xer0z-gh/Launch-Deck)** | A local control centre that works out what a project is and how to start it, then runs, supervises and stops it. 32 runner definitions. Supervision built on Windows Job Objects, so nothing survives a kill. | **353 Rust tests and 14 browser suites**, the browser suites driven against the shipped release binary rather than a dev server. Pointed at the real registry of **37 projects**, it names each one that cannot start and the exact repairable fault, from filesystem reads alone, before anything is launched. |
| **[VideoForge](https://github.com/Xer0z-gh/Video-Forge)** | One command turns a brief into a rendered, captioned, loudness-normalized MP4 with thumbnail, titles and chapters. Every edit, yours or the copilot's, is one of 19 typed, invertible, journaled operations — which is where undo, version history and crash recovery come from. | **211 tests pass** (last run 2026-09-16), 11 of them on the editor's HTTP trust boundary. **Undo survives closing the program**: a reopened project replays its journal to a byte-identical document. An export was re-transcribed by whisper with no knowledge of the edit — **45 words became 42, every filler gone.** Runtime dependencies: **2**. |
| **[Vesper](https://github.com/Xer0z-gh/Vesper)** | A 13-module sound design plugin in one window, reordered from the chain-order menu: 17 saturation algorithms, linear-phase match EQ, shimmer reverb. VST3 and standalone. | **142 unit checks and 49 integration checks, 0 failures**, the integration suite driving the real processor rather than the DSP in isolation. All 13 modules together render at **26x realtime**; the editor opens in 2.5 ms. CI runs pluginval at **strictness 8** on Windows and macOS; strictness 10 across 5 sample rates x 7 block sizes is a manual sweep. |
| **[Coupon Hunter](https://github.com/Xer0z-gh/Coupon-Hunter)** | Browser extension that finds checkout codes, types each candidate, watches the order total react, and keeps the one that drops it most. It never clicks anything that places the order. | **22 sources queried in a single fan-out**, and one that hangs is dropped at 8 s while the rest carry on. **25 tests pass** in about a tenth of a second, including one that pins **16 order-submitting labels** — `Pay $42.99`, `Place order`, `Review order`, the bare `Continue` — as never-click, and 10 apply labels as safe. |

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

Every number above is the output of a test run or a live measurement, not an
estimate, and that output goes into your handover next to the code. So does the
other half: what was not tested, and why. That is the part you actually need,
because it tells you where to look first.

Not on offer: hourly work, calls or live interviews, or reviewing someone else's
code without building anything. Everything runs in writing, so you keep the
record of what was agreed, and so do I.

---

**Written enquiries:** xer0z.1nz@gmail.com

<sub>Source in these repositories is published so you can check the work. Each repository states its own licence.</sub>
