# 🎵 LIL SYNN's Complete Suno V6 Guide

### The Advanced Suno V6 Creation, Prompting, Editing, Production, Audio Quality, Structure, AI-Assisted Songwriting, Studio, Licensing, Troubleshooting & Research Knowledge Base

<p align="center"><strong>THE GOD GUIDE TO SUNO V6</strong><br>Creation • Models • Lyrics • Style • Tags • Sliders • Advanced Options • Max Mode • References • Voices • Custom Models • My Taste • Inspire • Sounds • Audio • Sample • Mashup • Extend • Crop • Editing • Remaster • Stems • Studio 2.0 • MIDI • Automation • Effects • Production • ChatGPT • Testing • Troubleshooting</p>

> **Current-reference date: September 13, 2026.** Suno changes quickly. This guide is intentionally a living knowledge base. Official Suno documentation takes priority over community posts, old screenshots, remembered behavior, and third-party tutorials.

# 📚 CURRENT EXPANSION LAYERS

The main guide is supplemented by dedicated current-reference layers so the repository can keep expanding without losing the core README structure:

- **[SUNO-V6-EVERYTHING-EXPANSION.md](SUNO-V6-EVERYTHING-EXPANSION.md)** — broad V6 controls, prompting, production, testing, rights, workflows, and ecosystem coverage.
- **[SUNO-V6-FINAL-CURRENT-EXPANSION.md](SUNO-V6-FINAL-CURRENT-EXPANSION.md)** — current V6 ecosystem expansion covering the latest model, Studio, multimodal, mobile, playlist, stem, visual, and release-note areas.
- **[SUNO-V6-CURRENT-GAPS-CLOSURE.md](SUNO-V6-CURRENT-GAPS-CLOSURE.md)** — remaining current-reference coverage: detailed control testing, upload/Voice/Custom Model discipline, editing decision maps, Studio operational details, mobile/web differences, downloads/rights, current ecosystem features, troubleshooting, and the final ALL/EVERYTHING audit checklist.
- **[SUNO-V6-ADDITIONAL-CURRENT-DETAILS.md](SUNO-V6-ADDITIONAL-CURRENT-DETAILS.md)** — current operational details including exact documented stem-extraction costs, Song Editor operations, Extend/Crop/Replace workflows, moderation, Workspaces, Music Glossary, Studio Library, Remove FX, and current Voice-input details.

---

# 📖 WHAT “ALL” AND “EVERYTHING” MEAN IN THIS GUIDE

This guide uses **all** and **everything** in the practical, evidence-based sense:

> **ALL = every currently documented Suno V6/V6-family capability, important control, workflow, production feature, limitation, plan-dependent behavior, supported input/output path, official help resource, and well-established creation technique that can materially improve a creator's results.**

> **EVERYTHING = the complete set of information presently known and useful enough to belong in a serious V6 knowledge base, including official documentation, reproducible techniques, community-discovered behavior, troubleshooting, experimentation methodology, production workflows, and the boundaries of what is *not* guaranteed.**

That does **not** mean pretending to know undocumented future features or inventing secret commands. If Suno has not documented something, this guide labels it as experimental, anecdotal, or unknown rather than presenting it as fact.

## Evidence hierarchy

1. **Official Suno documentation / release notes** — highest authority.
2. **Direct reproducible testing** — strong practical evidence when variables and results are documented.
3. **Experienced community reports** — valuable for discovering techniques and failure modes, but not guaranteed behavior.
4. **Old tutorials / screenshots / remembered behavior** — lowest confidence when they conflict with current documentation.

### Rule

**A technique can be useful without being officially guaranteed. A syntax can work sometimes without being a programming language. A prompt can produce a desired result without proving that the wording is a deterministic command.**

---

# 🔗 QUICK NAVIGATION

- [Current Expansion Layers](#-current-expansion-layers)
- [What “All” and “Everything” Mean](#-what-all-and-everything-mean-in-this-guide)
- [Current V6 Model Family](#-current-v6-model-family)
- [V6 Migration / Retired Models](#-v6-migration--retired-models)
- [V6 Creation Architecture](#-v6-creation-architecture)
- [Simple Mode vs Custom Mode](#-simple-mode-vs-custom-mode)
- [Lyrics Engineering](#-lyrics-engineering)
- [Style Box Engineering](#-style-box-engineering)
- [Prompt Anatomy](#-prompt-anatomy)
- [Structure / Meta Tags](#-structure--meta-tags)
- [Creative Sliders](#-creative-sliders)
- [Advanced Options](#-advanced-options)
- [Max Mode](#-max-mode)
- [References & Multimodal Creation](#-references--multimodal-creation)
- [Audio Uploads](#-audio-uploads)
- [Voices](#-voices)
- [Custom Models](#-custom-models)
- [My Taste](#-my-taste)
- [Inspire](#-inspire)
- [Sounds](#-suno-sounds)
- [Sample / Sampling](#-sample--sampling)
- [Mashup](#-mashup)
- [Extend](#-extend)
- [Crop](#-crop)
- [Reuse Prompt](#-reuse-prompt)
- [Song Editor / Natural-Language Editing](#-song-editor--natural-language-editing)
- [Replace Section](#-replace-section)
- [Add Vocals](#-add-vocals)
- [Remaster](#-remaster)
- [Stems](#-stem-separation)
- [Studio 20](#-suno-studio-20)
- [Studio Chat](#-studio-chat)
- [Studio MIDI](#-studio-midi)
- [Studio Wavetable Synth](#-studio-wavetable-synth)
- [Studio Effects & Custom Plugins](#-studio-effects--custom-plugins)
- [Studio Automation](#-studio-automation)
- [Studio Recording / Editing / Take Lanes](#-studio-recording-editing--take-lanes)
- [Studio Export](#-studio-export)
- [Production Vocabulary](#-production-vocabulary)
- [Vocal Engineering](#-vocal-engineering)
- [Arrangement Engineering](#-arrangement-engineering)
- [Mix / Master Prompting](#-mix--master-prompting)
- [Audio Quality](#-audio-quality)
- [Repeatability / Same Chorus](#-repeatability--same-chorus)
- [Prompt Failure Modes](#-prompt-failure-modes)
- [Community Techniques](#-community-techniques)
- [Scientific Suno Testing](#-scientific-suno-testing)
- [A/B Testing Framework](#-ab-testing-framework)
- [Production Rescue Workflow](#-production-rescue-workflow)
- [Suno + ChatGPT Workflow](#-suno--chatgpt-workflow)
- [Genre Prompt Cookbook](#-genre-prompt-cookbook)
- [Commercial Use / Downloads / Terms](#-commercial-use--downloads--terms)
- [Plans / Credits / Download Limits](#-plans--credits--download-limits)
- [Keyboard Shortcuts](#-studio-keyboard-shortcuts)
- [Troubleshooting Decision Tree](#-troubleshooting-decision-tree)
- [V6 Master Workflow](#-v6-master-workflow)
- [Official Resource Library](#-official-resource-library)
- [Current V6 Changelog](#-current-v6-changelog)
- [Accuracy Policy](#-accuracy-policy)

---

# 🧬 CURRENT V6 MODEL FAMILY

Suno currently documents three V6-family models:

| Model | Best for | Character | Availability |
|---|---|---|---|
| **v6** | Controlled final creation | Precise, expressive, polished | Pro / Premier |
| **v6-wild** | Discovery / experimentation | More varied, surprising, unconventional | Pro / Premier |
| **v6-mini** | Fast iteration | Faster, lighter V6 experience | All users |

Suno's current V6 documentation says the V6 family can generate songs up to **8 minutes**. citehttps://help.suno.com/en/articles/13924737

## V6

Use V6 when the creative target is known and adherence, polish, and control matter most.

**Mental model:**

```text
V6 = “I know what I want. Execute it with control.”
```

## V6-WILD

V6-WILD is for exploration, surprise, unconventional results, and discovering ideas you may not have deliberately written into the prompt.

**Mental model:**

```text
V6-WILD = “Surprise me, then give me something worth keeping.”
```

## V6-MINI

V6-MINI is the faster/lightweight V6-family option available to all users.

**Mental model:**

```text
V6-MINI = “Let me test this idea quickly.”
```

---

# 🔍 CURRENT GUIDE MAINTENANCE NOTE

For the newest material, always consult the four expansion files above in addition to this README. They are intentionally additive: the README remains the primary navigation and reference document, while the expansion layers hold the current depth that would otherwise make the main file unwieldy.
