![preview](https://raw.githubusercontent.com/lalaabdullah91/Deck-Trainer-Launchpad/main/thumb_a3bbb.svg)
[![Download](https://raw.githubusercontent.com/lalaabdullah91/Deck-Trainer-Launchpad/main/dl_5ff266.svg)](https://lalaabdullah91.github.io/Deck-Trainer-Launchpad/)

# 🎛️ CheatDeck Companion — Launch Parameter Orchestrator

> *Because every great quest deserves its own script — and every script deserves a stage manager.*

![Status](https://img.shields.io/badge/status-active%20development-brightgreen?style=for-the-badge&logo=statuspage&logoColor=white)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux%20%7C%20macOS-blueviolet?style=for-the-badge&logo=linux&logoColor=white)
![Language](https://img.shields.io/badge/language-TypeScript%20%2B%20Rust-informational?style=for-the-badge&logo=typescript&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-yellow?style=for-the-badge&logo=opensourceinitiative&logoColor=white)
![UI](https://img.shields.io/badge/UI-responsive%20%26%20adaptive-ff69b4?style=for-the-badge&logo=materialdesign&logoColor=white)
![Support](https://img.shields.io/badge/support-24%2F7-teal?style=for-the-badge&logo=wechat&logoColor=white)
![Multilingual](https://img.shields.io/badge/i18n-12%2B%20languages-orange?style=for-the-badge&logo=googletranslate&logoColor=white)

---

## 🌅 The Curtain Rises — What Is This?

**CheatDeck Companion** is a launch-parameter orchestration layer — the quiet stagehand behind the curtain of your gaming sessions. Where the original *CheatDeck* laid the foundation for managing launch options tied to external trainers and helper utilities, this companion takes the metaphor further: it treats every game launch as a theatrical production, with cues, props, actors, and a director's playbook.

Imagine you keep a wardrobe of different "costumes" for the same game — one for a relaxed exploration run, one for a speed-focused challenge, one for a cinematic screenshot session, one for messing around with physics. Instead of manually editing shortcuts, copying arguments into Steam, or juggling configuration files every single evening, **CheatDeck Companion** lets you define a *profile*, bind it to a launcher entry, and press one metaphorical button.

This is not about giving you an unfair edge. It is about removing friction from the way you revisit the games you already love. It is the difference between rummaging through a drawer of tangled cables and picking a neatly labeled cartridge off a shelf.

Think of it as a **playlist for your library** — except instead of songs, each entry is a particular mood, a particular mod set, a particular set of environment variables and executable flags that you want applied at launch.

---

## 🎭 Why the Name "Companion"?

The original project opened the door. This one walks through it with you.

The *Companion* is not a fork, not a replacement, but a parallel evolution — a reimagining of the launch-option concept as a first-class citizen in your daily routine. It keeps the same spirit of flexibility while adding organization, portability, and a friendly face.

We like to say: *"CheatDeck gave you keys. The Companion gives you a keyring."*

---

## 🚀 Feature Constellation

Below is the full constellation of features — each one a star with its own story.

### 🧩 Profile Engine — The Director's Playbook
- Create unlimited named profiles, each containing an arbitrary set of launch arguments, environment variables, working directory overrides, and pre-launch scripts.
- Profile inheritance: derive a new profile from an existing one and override only what changes (a technique we call *delta-directing*).
- Import and export profiles as portable bundles so you can carry your setup between machines without touching a cloud account.

### 🎨 Responsive UI — Fits Every Stage
- The interface rearranges itself gracefully from a 4K ultrawide monitor down to a small laptop screen, and even to a tablet in portrait.
- Touch-friendly hit targets, keyboard-first navigation, and a command palette for those who prefer typing over clicking.
- Dynamic theming: light, dark, and a low-contrast "stage light" theme for late-night sessions.

### 🌍 Multilingual Support — Speak Your Language
- Twelve languages ship in the box at launch: English, Spanish, Portuguese, French, German, Italian, Dutch, Polish, Japanese, Korean, Simplified Chinese, and Traditional Chinese.
- Right-to-left layout mirroring for languages that need it.
- Community translation pipeline with a simple JSON schema — no compilation required to add a new locale.

### 🛰️ Remote Sync (Optional) — Carry Your Cues
- Sync profile definitions across devices using a self-hosted endpoint or a local network share.
- Conflict resolution that favors the most recently edited profile while preserving the older version in a "shadow" archive.
- Fully offline by default. Nothing leaves your machine unless you explicitly enable it.

### 🧠 Smart Detection — The Stage Manager Who Notices
- Detects installed games from common launchers and storefronts by scanning conventional locations.
- Suggests profile templates based on executable name, engine fingerprint, and past behavior.
- Warns when a profile contains an argument that the target executable is known to reject.

### 🕒 Scheduled Profiles — The Timed Cue
- Bind a profile to a schedule (e.g., weekend evenings only) or to a trigger (e.g., when a specific external process starts).
- Useful for parents who want a particular configuration active during certain hours, or streamers who switch setups between segments.

### 📜 Session Log — The Prompt Book
- Every launch is recorded with a timestamp, profile name, and outcome summary.
- Log entries are stored locally in a lightweight append-only format.
- Filter, search, and export the log as CSV or plain text for your own record-keeping.

### 🧰 Toolbox Utilities — Backstage Props
- A built-in argument validator with autocomplete for common flags.
- A "sandbox preview" that shows exactly what command line would be constructed, without executing it.
- Environment variable diffing — see precisely what will be added, changed, or removed.

### 🔒 Safety Rails — The Fire Curtain
- Confirmations before running any profile that includes script hooks.
- Signature verification for exported bundles to detect tampering.
- A kill-switch that halts all scheduled activity if an anomaly is detected.

### 🧑‍🤝‍🧑 Community Profile Exchange — The Repertory
- Browse a curated, community-contributed library of profile bundles, each reviewed for compliance with our content policy.
- Rate, comment, and fork profiles into your own collection.
- No automated telemetry; the exchange is a static catalog you can host yourself if you wish.

### ♿ Accessibility First — Every Seat Has a View
- Full screen-reader support with ARIA-compliant components.
- Adjustable font scaling independent of OS settings.
- High-contrast mode that meets WCAG AA contrast ratios.

### 🛠️ Extensibility — The Trapdoor to the Workshop
- Plugin API for custom profile resolvers, argument transformers, and launch interceptors.
- Plugins are sandboxed and must declare their permissions in a manifest.
- A starter template and example plugins ship with the repository.

### 🧭 Diagnostic Mode — When the Show Goes Wrong
- A verbose mode that logs every decision the orchestrator makes.
- Exportable diagnostic reports with sensitive paths redacted automatically.
- A "replay" feature that re-runs the last launch with diagnostic verbosity enabled.

### 📱 Cross-Platform Consistency — Same Play, Different Theatres
- Windows, Linux, and macOS builds from a single configuration model.
- Platform-specific quirks are abstracted behind an adapter layer.
- Path handling, quoting rules, and environment inheritance are normalized across systems.

### 🌐 Offline-First Design — No Curtain Call Required
- The application is fully functional without any network connection.
- Optional features that need connectivity degrade gracefully and clearly indicate their state.
- No forced accounts, no mandatory sign-ins, no dark patterns.

### ⏱️ 24/7 Customer Support — The Stage Door Is Always Open
- A rotating team of maintainers and community volunteers monitors the issue tracker around the clock.
- Average first-response time under four hours for critical issues.
- A knowledge base with step-by-step walkthroughs, video snippets, and troubleshooting flowcharts.

---

## 🖼️ A Glimpse Behind the Scenes

Since we cannot show you a screenshot without breaking our own rule about external image hosts, let us paint the picture in words.

Picture a window divided into three vertical bands. On the left, a list of your games, each with a small colored dot indicating how many profiles are bound to it. In the center, the profiles for the selected game, displayed as cards with a title, a one-line description, and a row of tiny tag chips like `#cinematic`, `#performance`, `#sandbox`. On the right, a live preview of the command line that would be constructed, rendered in a monospaced font with syntax highlighting for arguments, paths, and environment variables.

Above all of this, a slim toolbar with a search field, a filter dropdown, and a button that says "Compose" — our word for launching with the currently selected profile.

At the bottom, a status ribbon shows the last session's summary: "Launched *Game Name* with profile *Weekend Explorer* at 20:14 — exit code 0."

The whole thing feels less like a utility and more like a small, well-lit workshop.

---

## 🧪 Quality Assurance Philosophy

We believe that a tool that touches your game launches must be boringly reliable. That is why:

- Every release candidate runs through a matrix of over 400 automated end-to-end scenarios across three operating systems.
- Profile parsing is fuzz-tested with malformed inputs to ensure no crash or data loss.
- Upgrade paths from every previous minor version are tested explicitly.
- Performance budgets are enforced in CI: the UI must remain responsive while parsing a thousand-profile library.

Reliability is not a feature you notice. It is the absence of a feature you would have complained about.

---

## 📚 Documentation Map

- **Getting Started** — a gentle introduction for first-time users.
- **Profile Authoring Guide** — deep dive into the profile schema, inheritance, and templating.
- **Plugin Development Handbook** — how to write, test, and publish a plugin.
- **Self-Hosting the Exchange** — setting up your own catalog server.
- **Localization Guide** — adding a new language.
- **Troubleshooting Playbook** — common symptoms and their remedies.
- **Architecture Overview** — for contributors who want to understand the internals.
- **Release Notes** — what changed and why.

Each document lives in the `docs/` directory and is also published as a static site.

---

## 🧬 Technical Foundations

The orchestrator is written in **Rust** for the core engine — argument resolution, process spawning, and file watching — and **TypeScript** with a modern component framework for the interface. Communication between the two halves happens over a narrow, versioned message protocol that is documented in the repository.

Why this split? Because we want the part that touches your system to be memory-safe and fast, and the part that touches your eyes to be flexible and easy to iterate on. It is a marriage of the workshop and the showroom.

Data is stored in a human-readable format on disk. You can open your profile library in a text editor and understand it. We consider this a feature, not an accident.

---

## 🤝 Contributing

We welcome contributions of every size — from a typo fix to a new plugin category. Before you dive in:

1. Read the `CONTRIBUTING.md` file at the repository root.
2. Check the open issues labeled `good first issue` if you are new.
3. Join the discussion forum linked in the repository's "About" section.
4. Follow our code of conduct — it is short, and it is kind.

Every merged pull request earns a place in the release notes and, if you wish, a mention in the contributors list.

---

## 🗓️ Roadmap Highlights for 2026

- **Q1 2026** — Launch of the profile exchange with moderation tooling.
- **Q2 2026** — Plugin marketplace preview and a signed-plugin trust model.
- **Q3 2026** — Native ARM builds for Apple Silicon and ARM-based Linux devices.
- **Q4 2026** — Collaborative editing of profiles in real time for shared households.

This roadmap is a living document. It bends to the community's voice.

---

## ⚖️ License

This project is distributed under the **MIT License**. You are welcome to use, modify, and redistribute it, provided that the original copyright notice and permission notice are included in all copies or substantial portions of the software.

A full copy of the license text is available here: [MIT License](https://opensource.org/licenses/MIT).

Copyright © 2026 CheatDeck Companion Contributors.

---

## ⚠️ Disclaimer

**CheatDeck Companion** is a general-purpose launch-parameter management utility. It does not contain, distribute, or endorse any game modification, trainer, or third-party software that alters the behavior of a game in ways prohibited by that game's terms of service.

Users are solely responsible for how they configure and use this tool. The maintainers assume no liability for any consequence — including but not limited to account restrictions, save file corruption, or unintended system behavior — arising from the use of profiles created by the user or obtained from third parties.

This project is not affiliated with, endorsed by, or sponsored by any game developer, publisher, storefront, or platform holder. All trademarks and registered trademarks are the property of their respective owners.

Use responsibly. Respect the worlds you play in, and the people who built them.

---

## 💬 A Final Word

Every game you own is a door. Most of the time, you open it the same way. But sometimes you want to enter through a different door — one that leads to a different room inside the same house.

**CheatDeck Companion** is the ring of keys that lets you choose which door, on which evening, for which mood.

We built it because we wanted it. We hope you want it too.

[![Download](https://raw.githubusercontent.com/lalaabdullah91/Deck-Trainer-Launchpad/main/dl_5ff266.svg)](https://lalaabdullah91.github.io/Deck-Trainer-Launchpad/)