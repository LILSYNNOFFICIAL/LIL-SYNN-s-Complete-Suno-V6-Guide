# 🎵 SUNO V6 — ADDITIONAL CURRENT OPERATIONAL DETAILS

> **Audit date: September 13, 2026**
>
> This addendum captures additional current details that are easy to miss in a broad V6 guide: exact current stem extraction economics, Song Editor operations, moderation, Workspaces, Music Glossary, Studio Library behavior, Remove FX, and platform-specific operational distinctions.

---

# 1. ADVANCED STEM SEPARATION — CURRENT EXTRACTION ECONOMICS

Current Suno documentation states:

| Split type | What it does | Current availability | Current documented cost |
|---|---|---|---:|
| **Auto Split** | Separates a song into up to 12 broad stem categories | Pro / Premier | **50 credits per extraction** |
| **Split from Mix** | Extracts one selected instrument/voice plus a complement track | Pro / Premier | **10 credits per stem** |
| **Advanced Split** | Choose individual stems from a list of nearly 100 instruments | Premier | **10 credits per stem** |

### Operational rule

Do not request every possible stem merely because they are available. Decide what you actually need before extracting, because stem separation can consume credits.

### Example

```text
Need vocal only?
→ Split from Mix

Need a broad multitrack reconstruction?
→ Auto Split

Need a specific uncommon instrument?
→ Advanced Split
```

These costs are **current documented values**, not permanent guarantees. Recheck the current Suno help article before budgeting a large project.

---

# 2. STEMS — TWO ACCESS PATHS

Current documentation provides two primary access paths:

### From Library / Workspace

```text
Song
→ More Actions (...)
→ Get Stems
→ Choose split type
→ Extract
```

### From Studio

```text
Audio clip
→ Right-click
→ Split Stems
→ Choose split type
→ Extract
```

This matters because a creator does not need to enter Studio merely to obtain stems.

---

# 3. SONG EDITOR — CURRENT OPERATION MAP

The Song Editor provides localized editing operations around a song timeline.

Current documented operations include:

- moving sections;
- Quick Replace;
- adding a new section;
- setting the number of beats for an added section;
- generating multiple section versions;
- previewing before committing;
- editing section names/colors;
- splitting sections;
- cropping sections;
- editing lyrics for a highlighted region;
- extending the song;
- Fade In;
- Fade Out.

### Local-edit philosophy

```text
WHOLE SONG IS GOOD
       ↓
IDENTIFY THE BAD REGION
       ↓
EDIT ONLY THAT REGION
       ↓
PREVIEW
       ↓
COMMIT ONLY IF BETTER
```

This is one of the most important principles in the entire guide: **preserve good generations instead of regenerating them unnecessarily.**

---

# 4. REPLACE SECTION — PREVIEW BEFORE COMMIT

Current Song Editor documentation describes a Replace workflow where you can select a region, provide a prompt, preview alternate versions, generate more alternatives, and fine-tune the transition boundary.

### Recommended workflow

```text
HIGHLIGHT REGION
↓
WRITE THE SMALLEST USEFUL CHANGE
↓
GENERATE ALTERNATES
↓
AUDITION
↓
COMPARE TRANSITION
↓
ADJUST BOUNDARY
↓
COMMIT WINNER
```

Do not ask a localized replacement to redesign the entire song unless that is actually the goal.

---

# 5. QUICK REPLACE

Quick Replace is designed for rapid auditioning of a new version of a selected section.

Use it as an exploration step before making a larger commitment to the song.

```text
CURRENT SECTION
→ QUICK REPLACE
→ HEAR ALTERNATE
→ KEEP / REJECT
```

---

# 6. ADDING NEW SECTIONS

The current Song Editor supports inserting a new section between existing sections.

The workflow includes selecting the insertion point, specifying lyrics/direction, setting the desired number of beats, generating versions, previewing them, and committing the preferred version.

This is useful for:

- adding a pre-chorus;
- extending a bridge;
- inserting an instrumental break;
- adding a final chorus;
- creating a custom ending.

---

# 7. FADE IN / FADE OUT

Song Editor supports localized fade-in and fade-out control at the beginning/end of audio clips.

Use this for:

- cleaner starts;
- smoother endings;
- removing abrupt clip boundaries;
- shaping transitions before exporting.

A fade is a production edit, not a prompt instruction.

---

# 8. EXTEND — CHOOSE WHERE THE NEW MATERIAL STARTS

Current Extend documentation allows the creator to choose how much of the original song to retain before the new material begins.

Conceptually:

```text
ORIGINAL SONG
|-----------------------------|
                  ↑
             EXTEND POINT
                  |
                  +------ NEW MATERIAL
```

After choosing a preferred extension, Suno provides a Whole Song workflow that stitches the new ending to the original track.

### Extend is ideal for

- longer outros;
- new final choruses;
- alternate endings;
- instrumental extensions;
- resolving a song that ends too abruptly.

---

# 9. CROP — CURRENT SCOPE

Current Crop documentation identifies Crop as a desktop-web editing feature for Pro/Premier users that can remove unwanted material from the beginning or end of a song.

Use Crop when the generation is good but its opening/ending contains unwanted material.

Do not use full regeneration simply to remove dead air or an unwanted tail.

---

# 10. REUSE PROMPT — WHAT IT ACTUALLY TRANSFERS

Reuse Prompt can bring an existing song's creative setup back into the Create workflow so the creator can modify lyrics, style, and title before making another version.

Think of it as:

```text
OLD CREATIVE SETUP
↓
REUSE
↓
EDIT
↓
NEW GENERATION
```

It is not a guarantee that the new generation will reproduce the original performance exactly.

---

# 11. REMIX IS A CATEGORY, NOT ONE SINGLE OPERATION

Current Suno help documentation uses “Remix” as an umbrella for multiple transformation features, including:

- Cover;
- Extend;
- Adjust Speed;
- Use Styles and Lyrics / Reuse Prompt workflows;
- Crop;
- Replace Section.

On the web, these are accessed through Remix/Edit in the More Actions menu where applicable.

This distinction matters because a tutorial saying “use Remix” may actually mean a specific operation inside that category.

---

# 12. REMIX PERMISSION ≠ OWNERSHIP

If another creator's song allows remixing, that only establishes platform-level permission to use the applicable remix functionality. It does not automatically transfer ownership or grant unrestricted commercial rights.

Current Suno documentation also states that remix rights can remain tied to the original creator, and historical/new songs can have different default remix settings.

Always distinguish:

```text
CAN I TECHNICALLY REMIX IT?
        ≠
DO I OWN THE RESULT?
        ≠
CAN I MONETIZE THE RESULT?
```

---

# 13. MODERATION — CURRENT FAILURE CLASSIFICATION

Suno's current help documentation says content can be flagged before generation and gives examples including:

- names of well-known artists or people;
- copyrighted or trademarked terms;
- derogatory/defamatory terms;
- excessive profanity;
- other inappropriate content/topics.

Moderation outcomes can include preventing generation, asking for a song to be switched to Link Only, or removal of material.

### Diagnostic rule

If a prompt repeatedly fails:

```text
1. Check whether the request contains a protected name/term.
2. Remove unnecessary identifying references.
3. Replace direct imitation language with audible characteristics.
4. Retry with an original creative description.
5. If still blocked, consult current Suno support/terms.
```

Do not automatically label moderation as a model bug.

---

# 14. WORKSPACES — PROJECT ORGANIZATION

Suno Workspaces provide a separate project-management surface from the general Library.

Use Workspaces for larger projects where you need to keep:

- alternate generations;
- stems;
- drafts;
- edits;
- production versions;
- final candidates;

organized together.

### Suggested project structure

```text
ALBUM / SONG PROJECT
├── 01 IDEAS
├── 02 SHORTLIST
├── 03 VOCALS
├── 04 EDITS
├── 05 STEMS
├── 06 STUDIO
└── 07 FINAL
```

Exact Workspace UI can change; treat this as a workflow strategy rather than a claim about fixed folder semantics.

---

# 15. MUSIC GLOSSARY — PROMPT VOCABULARY TOOL

Suno maintains a Music Glossary for musical terminology that can help creators describe what they want when they are stuck on a prompt.

Use a glossary term when you know the audible concept but do not know the conventional production/musical word for it.

### Example progression

```text
“I want the drums to feel like they are pushing forward.”
        ↓
Search musical terminology
        ↓
Identify a useful rhythm/dynamics term
        ↓
Test that term in the Style prompt
```

The glossary should be treated as a vocabulary resource, not as a list of secret commands.

---

# 16. STUDIO LIBRARY — CURRENT PROJECT INTEGRATION

Studio 2.0's Library dock provides access to current library material inside Studio.

Current documented views include:

- All Songs;
- Liked;
- Stems;
- Uploads;
- Workspaces;
- Studio Projects.

The Library supports search/filtering and quick auditioning. Songs can be dragged onto the Studio timeline or attached to Chat Bar prompts.

### Practical workflow

```text
LIBRARY
↓
AUDITION
↓
DRAG SOURCE INTO TIMELINE
↓
EDIT / SPLIT / PROCESS
```

This makes Studio more than a separate editor; it is connected to the broader Suno library.

---

# 17. STUDIO NOTES AND SONG DETAILS

Current Studio Library documentation describes Song Details with Stems and Notes views.

Use Notes for project-specific information such as:

```text
VOCAL TAKE: best
CHORUS: keep original
BRIDGE: replace
MASTER: candidate B
EXPORT: 32-bit WAV
```

This is especially useful when a project contains many generated variations.

---

# 18. REMOVE FX — DRY-SOURCE WORKFLOW

Studio's Remove FX workflow can create a dry version of an audio clip by stripping added reverb and delay effects.

This is useful when you want to:

- process a vocal from scratch;
- isolate a cleaner instrument source;
- rebuild an effect chain;
- reduce unwanted ambience before mixing.

### Dry-source workflow

```text
WET CLIP
↓
REMOVE FX
↓
DRY VERSION
↓
NEW EQ / COMP / REVERB / DELAY CHAIN
```

Do not assume “dry” means perfect separation or complete removal of every artifact. Listen to the result.

---

# 19. STUDIO TAKE / EDITING PRINCIPLE

Studio is designed around iterative production rather than one irreversible edit.

Use alternates and take-oriented workflows to preserve options.

Recommended principle:

```text
NEVER DESTROY A GOOD TAKE TO TEST A RISKY IDEA
```

Duplicate/alternate first when possible, then experiment.

---

# 20. CURRENT VOCAL-GENDER CONTROL

Current Suno documentation confirms two routes:

### Simple Mode

Describe the desired voice using “male” or “female” in the description.

### Custom Mode

Use:

```text
Advanced Options
→ Vocal Gender
→ Male / Female
```

Then use the Style field to further define the vocal character, such as gritty, soft, intimate, breathy, etc.

This is more explicit than relying on a community section tag alone.

---

# 21. VOICE PROFILE INPUT — CURRENT PRACTICAL LIMIT

Current Voices documentation says a voice source can be recorded/uploaded from approximately **15 seconds to 4 minutes**, after which the creator can select the best **2 minutes** of the recording for the voice profile.

Acapella recordings are recommended for the cleanest results, although recordings containing background music are accepted and Suno can isolate the vocal.

### Preparation

```text
QUIET ROOM
→ CLEAN RECORDING
→ CLEAR PRONUNCIATION
→ NO CLIPPING
→ MINIMAL REVERB
→ SELECT BEST 2-MINUTE WINDOW
```

Voice availability and compatibility remain plan/platform/region-sensitive and should be checked against current Suno documentation.

---

# 22. VOICE SAFETY / SHARING DISTINCTION

Current Voices documentation distinguishes creating with your own voice from other users remixing published/shared songs that feature that voice.

The creator controls whether a song is published/shared and whether remixing is enabled.

The guide should therefore distinguish:

```text
VOICE PROFILE ACCESS
≠
SONG REMIX ACCESS
```

A shared/remixable song can expose the voice within that song's remix context without making the underlying voice profile freely reusable by everyone.

---

# 23. OFFICIAL VS COMMUNITY PROMPT SYNTAX

The guide should keep three categories separate:

### Officially documented

A feature, control, or workflow described by Suno.

### Reproducible technique

A prompt or method repeatedly observed under controlled tests.

### Community syntax

A tag or notation that users report as useful but Suno does not define as a formal command language.

Examples of community syntax should never be described as guaranteed parser instructions unless Suno explicitly documents them.

---

# 24. THE “NO SECRET COMMANDS” RULE

Never claim that Suno supports an invented syntax merely because a generation appears to respond to it.

Avoid presenting examples such as:

```text
[VOCAL_LOCK: TRUE]
[STEREO_WIDTH: 90]
[EQ: +3DB@8KHZ]
[SEED: 12345]
```

as official Suno controls unless Suno documents them.

They can be used as **experiments** only when clearly labeled experimental.

---

# 25. CURRENT FEATURE-CLASSIFICATION MATRIX

| Area | Official | Reproducible testing useful? | Main caution |
|---|---:|---:|---|
| V6 models | ✅ | ✅ | availability changes |
| Creative sliders | ✅ | ✅ | behavior is not a fixed equation |
| Structure tags | Partly | ✅ | not a guaranteed programming language |
| Style prompts | ✅ | ✅ | prompt wording is probabilistic |
| Voices | ✅ | ✅ | compatibility/availability can change |
| Custom Models | ✅ | ✅ | dataset quality matters |
| My Taste | ✅ | ✅ | personalization adds a variable |
| Sounds | ✅ | ✅ | current beta/feature state can change |
| Sample | ✅ | ✅ | source rights matter |
| Mashup | ✅ | ✅ | source components are not guaranteed perfect isolation |
| Stems | ✅ | ✅ | artifacts may remain |
| Studio effects | ✅ | ✅ | processing decisions remain subjective |
| Chat Bar | ✅ | ✅ | natural-language operations can vary |
| Community tags | ❌ unless documented | ✅ | do not call them official commands |
| Secret model parameters | ❌ | ⚠️ | do not invent |

---

# 26. FINAL OPERATIONAL DECISION TREE

```text
START WITH AN IDEA
        ↓
Need speed?
 ├─ YES → v6-mini
 └─ NO
      ↓
Need surprise?
 ├─ YES → v6-wild
 └─ NO → v6
      ↓
Is the whole song wrong?
 ├─ YES → revise concept/prompt and regenerate
 └─ NO
      ↓
Is one section wrong?
 ├─ YES → Replace Section / Song Editor
 └─ NO
      ↓
Is one word/line wrong?
 ├─ YES → single-lyric editing
 └─ NO
      ↓
Is the sound/mix the problem?
 ├─ YES → Remaster / Stems / Studio
 └─ NO
      ↓
Need detailed production?
 ├─ YES → Studio 2.0
 └─ NO → export / share / archive
```

---

# 27. CURRENT SOURCE LINKS

- V6 current models: https://help.suno.com/en/articles/13924737
- V6 “What’s new”: https://help.suno.com/en/articles/13924801
- V6 FAQ: https://help.suno.com/en/articles/13924481
- Song Editor: https://help.suno.com/en/articles/6141505
- Replace Section: https://help.suno.com/en/articles/3271873
- Extend: https://help.suno.com/en/articles/2409601
- Crop: https://help.suno.com/en/articles/3166529
- Remix: https://help.suno.com/en/articles/6050497
- Remix permissions: https://help.suno.com/en/articles/5675265
- Reuse Prompt: https://help.suno.com/en/articles/2551041
- Moderation: https://help.suno.com/en/articles/3198209
- Vocal Gender: https://help.suno.com/en/articles/10153473
- Voices: https://help.suno.com/en/articles/11362369
- Voices FAQ: https://help.suno.com/en/articles/11362433
- Advanced Stems: https://help.suno.com/en/articles/13925185
- Studio Library: https://help.suno.com/en/articles/13670849
- Studio 1.2 / Remove FX background: https://help.suno.com/en/articles/10625089
- Add Vocals: https://help.suno.com/en/articles/6882817
- Making Music category: https://help.suno.com/en/categories/550017

---

# END — ADDITIONAL CURRENT OPERATIONAL DETAILS
