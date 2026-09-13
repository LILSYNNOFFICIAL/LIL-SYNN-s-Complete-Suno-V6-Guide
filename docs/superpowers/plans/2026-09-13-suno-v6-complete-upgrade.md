# Suno V6 Complete Guide Upgrade Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Upgrade the living Suno V6 knowledge base with the requested control matrix, prompt hierarchy, slider laboratory, mythbusters, reproducibility protocol, Studio 2.0 deep dive, vocal engineering, diagnostic/rescue workflows, platform matrix, rights decision tree, and Creator's Operating System while repairing GitHub Markdown links.

**Architecture:** Keep the existing README as the organized master index and add a focused current-reference addendum containing the deep new material. Extend the existing README maintenance workflow so it automatically removes ChatGPT-only citation markup, inserts the new addendum into navigation, and preserves back-to-top navigation. Source current claims from official Suno help/release-note material and label experimental/community claims explicitly.

**Tech Stack:** GitHub Markdown, GitHub Actions, Python standard library.

**Spec:** The user-approved 2026-09-13 guide-upgrade design in conversation.

## Global Constraints

- Official Suno documentation/release notes outrank older tutorials and community claims.
- Never present undocumented prompt tricks as guaranteed commands.
- Date-stamp current product/plan/rights information.
- Keep GitHub README links as normal Markdown/HTML; never leave ChatGPT `url...` or `cite...` markup in repository content.
- Preserve the existing `<a id="top"></a>` target and back-to-top navigation.
- Separate OFFICIAL, RELEASE NOTE, REPRODUCIBLE, COMMUNITY, EXPERIMENTAL, UNKNOWN, and RETIRED evidence.
- Verify the final README and new addendum after changes.

---

### Task 1: Add the complete 2026 upgrade addendum

**Files:**
- Create: `SUNO-V6-ULTIMATE-CONTROL-AND-PRODUCTION-ADDENDUM-2026.md`

- [ ] Add V6/V6-WILD/V6-MINI control matrix and model-selection decision tree.
- [ ] Add prompt anatomy and instruction-hierarchy model.
- [ ] Add negative-prompting/avoidance guidance with evidence boundaries.
- [ ] Add Slider Laboratory with controlled A/B test matrices for Weirdness, Style Influence, Audio Influence, Variety, and Max Mode.
- [ ] Add reproducibility protocol and generation log schema.
- [ ] Add Suno Mythbusters separating official facts from unproven community folklore.
- [ ] Add Studio 2.0 deep dive: Chat Bar, MIDI, piano roll, musical typing, external MIDI, audio↔MIDI, wavetable, effects, custom plugins, automation, recording, Take Lanes, Remove FX, timing, shortcuts, export, and September 2026 update notes.
- [ ] Add expanded vocal engineering taxonomy and failure diagnostics.
- [ ] Add “Why Suno Did That” diagnostic tree and Generation → Rescue → Production decision tree.
- [ ] Add Web/iOS/Android feature-parity matrix with September 2026 verification date and explicit rollout caveat.
- [ ] Add rights/commercial-release decision tree covering paid commercial-use rights, copyright distinction, download limits, and source-material permissions.
- [ ] Add Creator's Operating System end-to-end workflow with exit criteria.
- [ ] Add official-source index with normal Markdown links.

### Task 2: Repair README navigation and invalid citation markup automatically

**Files:**
- Modify: `.github/workflows/readme-back-to-top.yml`

- [ ] Extend workflow triggers to include the new addendum.
- [ ] Add a deterministic cleanup pass converting ChatGPT citation constructs to ordinary Markdown links for known official URLs and removing unsupported citation tokens.
- [ ] Add a stable navigation entry for the new addendum if absent.
- [ ] Keep existing back-to-top insertion idempotent.
- [ ] Keep bot commits protected from recursive runs.

### Task 3: Verify repository content

**Files:**
- Verify: `README.md`
- Verify: `SUNO-V6-ULTIMATE-CONTROL-AND-PRODUCTION-ADDENDUM-2026.md`
- Verify: `.github/workflows/readme-back-to-top.yml`

- [ ] Confirm no `cite` or `url` strings remain in repository Markdown.
- [ ] Confirm the new addendum is linked from README.
- [ ] Confirm current V6 model, Studio, downloads/rights, and mobile claims are date-stamped.
- [ ] Confirm back-to-top target and links remain present.
- [ ] Confirm the GitHub Actions maintenance workflow completes successfully after the update.
