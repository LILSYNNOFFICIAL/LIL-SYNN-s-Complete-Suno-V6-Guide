# 🎵 LIL SYNN's Complete Suno V6 Guide

<p align="center">
  <img src="https://img.shields.io/badge/Suno-V6-111111?style=for-the-badge&logo=suno&logoColor=white" alt="Suno V6">
  <img src="https://img.shields.io/badge/V6--WILD-EXPERIMENTAL-6f42c1?style=for-the-badge" alt="V6 Wild">
  <img src="https://img.shields.io/badge/V6--MINI-FAST-0b7fab?style=for-the-badge" alt="V6 Mini">
  <img src="https://img.shields.io/badge/Studio-2.0-2563eb?style=for-the-badge" alt="Studio 2.0">
  <img src="https://img.shields.io/badge/Knowledge%20Base-LIVING-f59e0b?style=for-the-badge" alt="Living Knowledge Base">
  <img src="https://img.shields.io/badge/Status-CURRENT-16a34a?style=for-the-badge" alt="Current">
</p>

<p align="center"><strong>THE GOD GUIDE TO SUNO V6</strong><br>Creation • Prompting • Lyrics • Style • Models • Sliders • References • Voices • Custom Models • Editing • Stems • Studio 2.0 • MIDI • Effects • Automation • Production • Rights • Testing • Troubleshooting</p>

> **Current-reference date: September 13, 2026.** Suno changes quickly. This repository is a living knowledge base: current official Suno documentation and release notes outrank old screenshots, old tutorials, remembered behavior, and community claims.

---

# 📖 INTRODUCTION

This is not a basic “how to make a song” tutorial.

It is a **complete working reference for the current Suno V6 ecosystem**: what the tools are, where they live, what they are good for, how they interact, how to troubleshoot them, how to test them scientifically, and where the boundaries of the evidence are.

The central philosophy is simple:

```text
IDEA
  ↓
PROMPT / LYRICS / REFERENCES
  ↓
V6 GENERATION
  ↓
LISTEN
  ↓
DIAGNOSE THE ACTUAL PROBLEM
  ↓
SURGICAL EDITING
  ↓
STEMS / REMASTER
  ↓
STUDIO 2.0
  ↓
MIX / AUTOMATION / MIDI / EFFECTS
  ↓
QC
  ↓
EXPORT
```

**Do not regenerate a great song to solve a problem that can be fixed locally. Preserve good information; repair bad information locally.**

Suno currently describes V6 as its flagship model, V6-WILD as the experimental/less predictable variant, and V6-MINI as the faster version available to all users. All three support up to eight minutes per generation. urlSuno Current Modelshttps://help.suno.com/en/articles/13924737

---

# 🧭 QUICK NAVIGATION

## Core Guide

- [What “ALL” and “EVERYTHING” Mean](#-what-all-and-everything-mean)
- [Current V6 Model Family](#-current-v6-model-family)
- [Creation Architecture](#-creation-architecture)
- [Simple Mode vs Custom Mode](#-simple-mode-vs-custom-mode)
- [Lyrics Engineering](#-lyrics-engineering)
- [Style Box Engineering](#-style-box-engineering)
- [Prompt Engineering](#-prompt-engineering)
- [Structure / Meta Tags](#-structure--meta-tags)
- [Creative Sliders](#-creative-sliders)
- [Advanced Options / Max Mode](#-advanced-options--max-mode)
- [References & Multimodal Creation](#-references--multimodal-creation)
- [Audio Uploads](#-audio-uploads)
- [Voices](#-voices)
- [Custom Models](#-custom-models)
- [My Taste](#-my-taste)
- [Inspire](#-inspire)
- [Sounds](#-sounds)
- [Sample & Mashup](#-sample--mashup)
- [Editing: Extend / Crop / Replace / Reuse / Adjust](#-editing-extend--crop--replace--reuse--adjust)
- [Song Editor / Natural-Language Editing](#-song-editor--natural-language-editing)
- [Add Vocals](#-add-vocals)
- [Remaster](#-remaster)
- [Stem Separation](#-stem-separation)
- [Studio 2.0](#-studio-20)
- [Studio Chat](#-studio-chat)
- [Studio MIDI](#-studio-midi)
- [Wavetable Synth](#-wavetable-synth)
- [Effects & Custom Plugins](#-effects--custom-plugins)
- [Automation](#-automation)
- [Recording / Editing / Take Lanes](#-recording--editing--take-lanes)
- [Library / Workspaces](#-library--workspaces)
- [Studio Export](#-studio-export)
- [Production Vocabulary](#-production-vocabulary)
- [Vocal Engineering](#-vocal-engineering)
- [Arrangement Engineering](#-arrangement-engineering)
- [Audio / Mix / Master Quality](#-audio--mix--master-quality)
- [Repeatability / Same Chorus](#-repeatability--same-chorus)
- [Failure Modes](#-failure-modes)
- [Scientific Testing](#-scientific-testing)
- [Production Rescue](#-production-rescue)
- [Suno + ChatGPT Workflow](#-suno--chatgpt-workflow)
- [Genre Cookbook](#-genre-cookbook)
- [Plans / Credits / Downloads / Rights](#-plans--credits--downloads--rights)
- [Mobile / Web Ecosystem](#-mobile--web-ecosystem)
- [Troubleshooting](#-troubleshooting)
- [Master Workflow](#-master-workflow)
- [Official Resource Library](#-official-resource-library)
- [Accuracy Policy](#-accuracy-policy)

## Deep-Dive Expansion Files

- **[SUNO-V6-EVERYTHING-EXPANSION.md](SUNO-V6-EVERYTHING-EXPANSION.md)** — broad V6 controls, prompting, production, testing, rights, workflows, limitations and community techniques.
- **[SUNO-V6-FINAL-CURRENT-EXPANSION.md](SUNO-V6-FINAL-CURRENT-EXPANSION.md)** — current model, multimodal, Studio, mobile, playlist, stems, visual and release-note coverage.
- **[SUNO-V6-CURRENT-COVERAGE-AUDIT.md](SUNO-V6-CURRENT-COVERAGE-AUDIT.md)** — coverage audit and evidence map.
- **[SUNO-V6-CURRENT-GAPS-CLOSURE.md](SUNO-V6-CURRENT-GAPS-CLOSURE.md)** — detailed current-reference gap closure and testing methodology.
- **[SUNO-V6-GAP-CLOSURE-ALL-REMAINING-CURRENT.md](SUNO-V6-GAP-CLOSURE-ALL-REMAINING-CURRENT.md)** — all remaining current ecosystem details identified during the audit.
- **[SUNO-V6-ADDITIONAL-CURRENT-DETAILS.md](SUNO-V6-ADDITIONAL-CURRENT-DETAILS.md)** — current operational details including stems, Song Editor, editing, moderation, Workspaces, Music Glossary, Studio Library, Remove FX and Voices.

> **How to use the repository:** Start here for the organized master reference. Use the expansion files when you need deeper coverage, historical/current audits, or detailed operational notes.

---

# 📖 WHAT “ALL” AND “EVERYTHING” MEAN

**ALL** means every currently documented and materially useful Suno V6/V6-family capability, control, workflow, input/output path, production feature, limitation, plan-dependent behavior, official resource, and well-established technique that belongs in a serious creator reference.

**EVERYTHING** means ALL of that **plus the boundaries of the knowledge**: reproducible behavior, community discoveries, troubleshooting, testing methodology, workflow strategy, historical migration context, known limitations, plan/credit interactions, and things Suno has not guaranteed.

It does **not** mean inventing undocumented secret commands or pretending a lucky prompt is deterministic.

### Evidence hierarchy

```text
1. OFFICIAL DOCUMENTATION / RELEASE NOTES
2. DIRECT REPRODUCIBLE TESTING
3. EXPERIENCED COMMUNITY REPORTS
4. OLD TUTORIALS / SCREENSHOTS / MEMORY
```

Evidence labels used throughout the repository:

- **OFFICIAL** — directly documented by Suno.
- **RELEASE NOTE** — announced in Suno's release notes.
- **REPRODUCIBLE** — repeatedly observed under controlled conditions.
- **COMMUNITY** — useful technique reported by creators but not guaranteed.
- **EXPERIMENTAL** — promising but insufficiently established.
- **UNKNOWN** — not established by reliable evidence.
- **RETIRED** — historical behavior no longer current.

---

# 🧬 CURRENT V6 MODEL FAMILY

| Model | Best use | Character | Availability |
|---|---|---|---|
| **V6** | Controlled creation / refinement | Precise, expressive, polished | Pro / Premier |
| **V6-WILD** | Discovery / experimentation | More varied, surprising, unconventional | Pro / Premier |
| **V6-MINI** | Fast iteration / idea testing | Faster, efficient V6 experience | All users |

All three current V6-family variants support up to **8 minutes per generation**. citeturn0search4

### V6 mental model

```text
I know what I want.
Execute it with control.
```

### V6-WILD mental model

```text
Surprise me.
Give me ideas I would not have designed myself.
```

### V6-MINI mental model

```text
Test the idea quickly before spending time polishing it.
```

### Best discovery pipeline

```text
V6-MINI → cheap/fast concept exploration
        ↓
V6-WILD → unusual ideas / arrangement discoveries
        ↓
V6 → controlled refinement
        ↓
Edit → Stems → Studio 2.0 → final production
```

Suno's model picker is in the top-right of the Create form and stays selected until changed. Custom Models can also appear there for eligible users. citeturn0search6

---

# 🏗️ CREATION ARCHITECTURE

Treat Suno as a layered system rather than one giant prompt:

```text
MODEL
↓
MODE
↓
SONG IDENTITY / STYLE
↓
LYRICS
↓
SECTION DIRECTION
↓
REFERENCES / AUDIO / IMAGE / VIDEO
↓
SLIDERS / ADVANCED OPTIONS
↓
GENERATION
↓
LISTEN + SCORE
↓
SURGICAL EDITING
↓
REMASTER / STEMS
↓
STUDIO 2.0
↓
EXPORT
```

Each layer solves a different class of problem. Use the smallest layer capable of fixing the problem.

---

# 🪄 SIMPLE MODE VS CUSTOM MODE

### Simple Mode

Best when you want to describe an outcome naturally and let Suno infer the generation workflow.

Example:

```text
Dark emotional electropop about realizing you were the problem in a relationship. Intimate low-register male vocal, sparse nocturnal verses, rising tension into a huge bittersweet chorus, warm analog synths, controlled sub bass, tight electronic drums, layered harmonies, polished modern production, emotionally devastating but restrained rather than theatrical.
```

### Custom Mode

Use when you need explicit control over lyrics, Style, structure, vocal direction and testing variables.

Best for:

- original lyrics
- structured songs
- repeatability experiments
- exact creative intent
- controlled A/B testing
- section-level direction

---

# ✍️ LYRICS ENGINEERING

Lyrics are both words **and performance input**.

A strong baseline structure:

```text
[Intro]
[Verse 1]
[Pre-Chorus]
[Chorus]
[Verse 2]
[Pre-Chorus]
[Chorus]
[Bridge]
[Final Chorus]
[Outro]
```

Production-oriented section direction can combine structure with performance/arrangement intent:

```text
[Verse 1 | intimate lead vocal | sparse drums | restrained delivery]
[Pre-Chorus | rising tension | bass opens | increasing vocal intensity]
[Chorus | full drums | wide synths | stacked harmonies | vocal forward]
[Bridge | contrasting harmony | reduced drums | exposed vocal]
[Final Chorus | expanded harmonies | maximum emotional lift]
```

**Important:** bracket syntax is guidance, not a guaranteed programming language. Suno may interpret, reinterpret, ignore, or occasionally vocalize descriptive text.

### Lyric density rule

Do not put DAW engineering instructions into every line. Keep song-wide sound in Style and local performance/arrangement guidance near the relevant section.

### Strong chorus

Prioritize:

- recognizable hook
- repeatable phrasing
- melodic room for emphasis
- emotional escalation
- memorable language

### Bridge function

A useful bridge can change harmony, perspective, instrumentation, rhythm, vocal intensity, lyrical information or emotional temperature.

---

# 🎨 STYLE BOX ENGINEERING

Think in audible behavior, not adjective soup.

```text
PRIMARY GENRE
+ SUBGENRE
+ VOCAL IDENTITY
+ CORE INSTRUMENTS
+ GROOVE
+ HARMONIC FEEL
+ ARRANGEMENT ARC
+ DYNAMICS
+ ATMOSPHERE
+ MIX CHARACTER
+ MASTER CHARACTER
```

### Master Style template

```text
Primary identity: [genre + subgenre + production family].
Vocal: [register + texture + delivery + emotional behavior].
Core instruments: [3–7 important instruments].
Rhythm: [groove + drum character + tempo feel].
Harmony: [tonal/modal character if important].
Arrangement: [density progression and section arc].
Dynamics: [where the track grows, contracts, peaks and resolves].
Atmosphere: [emotional/environmental character].
Mix: [vocal position + stereo width + low-end behavior + transients].
Master: [open + controlled + dynamic + polished].
```

Prefer:

```text
vocal-forward, controlled low end, wide chorus, dry close vocal, defined transients, restrained reverb
```

over:

```text
amazing, epic, beautiful, professional, high quality, cinematic
```

### Avoid prompt soup

One primary identity plus a small number of compatible influences is usually easier to control than a list of ten unrelated genres.

---

# 🧱 PROMPT ENGINEERING

Protect information in this order when shortening a prompt:

```text
1. PRIMARY IDENTITY
2. VOCAL
3. CORE INSTRUMENTS
4. GROOVE
5. ARRANGEMENT
6. DYNAMICS
7. ATMOSPHERE
8. MIX
9. MASTER
```

Remove redundancy before removing identity.

Positive descriptions are generally easier to reason about than dozens of exclusions, but exclusions can be useful for recurring failures.

```text
Good: dry intimate vocal, restrained reverb, controlled low end
Useful exclusion: avoid excessive vocal reverb and muddy low-mid buildup
```

---

# 🏷️ STRUCTURE / META TAGS

Useful section labels include:

```text
[Intro]
[Verse]
[Verse 1]
[Verse 2]
[Pre-Chorus]
[Chorus]
[Post-Chorus]
[Hook]
[Bridge]
[Break]
[Breakdown]
[Build]
[Drop]
[Interlude]
[Instrumental]
[Instrumental Break]
[Solo]
[Outro]
[End]
[Fade Out]
```

Performance vocabulary can include:

```text
[Lead Vocal]
[Backing Vocals]
[Harmony]
[Stacked Harmonies]
[Duet]
[Choir]
[Whispered]
[Spoken]
[Rapped]
[Ad-lib]
[Call and Response]
```

These are **probabilistic creative cues**, not guaranteed hidden API commands.

---

# 🎚️ CREATIVE SLIDERS

Current documented controls include:

| Control | What it does |
|---|---|
| **Weirdness** | Moves from safer/expected toward more chaotic/unusual results. |
| **Style Influence** | Controls how strongly supplied Style input influences the result. |
| **Audio Influence** | Appears with Audio Upload workflows and controls source-audio influence. |
| **Variety** | Current V6 behavior can modify/update style prompts to introduce variation. Variety 0 is useful when you need supplied style tags preserved. |

Suno documents Weirdness as Safe → Chaos with 50% as the normal expected result, and Style Influence as Loose → Strong. citehttps://help.suno.com/en/articles/6141377

### Testing rule

Change one slider at a time when learning its effect. Keep model, lyrics, references and prompt fixed.

### Controlled final

```text
Weirdness: low → moderate
Style Influence: strong
Audio Influence: moderate → strong when preservation matters
Variety: low / 0 when supplied Style must remain stable
```

### Discovery

```text
Weirdness: moderate → high
Style Influence: moderate
Variety: moderate → high
```

---

# ⚙️ ADVANCED OPTIONS & MAX MODE

Think of the controls this way:

```text
Prompt    = what you want
Model     = generation personality
Reference = what source material should influence it
Slider    = how strongly / variably it should explore
Max Mode  = extra effort for difficult fidelity/consistency tasks
```

Suno recommends Max Mode for longer songs, close covers, style transfer, and maintaining vocal/style consistency. It costs more credits. citeturn0search7

Do not use Max Mode as a substitute for a bad prompt or poor source material.

---

# 🖼️ REFERENCES & MULTIMODAL CREATION

V6 supports creation workflows using combinations of:

- text
- Suno songs
- playlists
- audio uploads
- images
- video

Suno explicitly describes multimodal V6 creation and role-based reference use. citeturn0search0

### Role-based reference prompting

```text
Reference A → vocal character
Reference B → drum groove
Reference C → synth palette
Lyrics      → only lyrical source
```

Do not simply say “use all references.” Assign each source a job.

---

# 🎧 AUDIO UPLOADS

Use Audio Uploads for demos, musical references, performances, source material, and transformation workflows.

Current Suno documentation distinguishes short uploads on free/basic access from longer uploads for Pro/Premier; current V6 workflows can work with audio references and Audio Influence. Verify the current upload limit in the live help page before relying on a duration limit because this is a product-controlled value.

Best source:

```text
clean recording
↓
minimal clipping
↓
consistent level
↓
legal/rightful source
↓
clear creative role
```

---

# 🎤 VOICES

Voices lets creators use a recorded/uploaded voice in Suno songs. Suno recommends clean/acapella source material for best results, while background music can also be supplied and isolated. Voices is available on iOS and Android and can be tried on free plans, with additional functionality on paid plans. citeturn0search1

### Voice workflow

```text
Clean recording
↓
Create / verify Voice
↓
Use compatible creation workflow
↓
Generate
↓
Evaluate identity
↓
Iterate arrangement / lyrics / Style
```

Only use voices you have permission to use. Technical capability does not establish legal permission.

---

# 🧠 CUSTOM MODELS

Current documentation says Pro/Premier users can create up to **three private Custom Models** using at least **six songs**. Bulk upload is supported; training takes roughly 2–5 minutes; uploaded songs must be ones you have rights to; custom models are private. citeturn0search6

### Training-set discipline

For a coherent model, use material with consistent:

- vocal identity
- genre family
- instrumentation
- songwriting style
- production philosophy
- mix character

Do not mix unrelated catalogs and then expect a tightly defined sonic identity.

---

# 🧠 MY TASTE

My Taste learns preferences such as genres, moods and references and can personalize creation through the Magic Wand/Style Augmentation workflow.

For controlled experiments, document whether personalization is enabled. Personalization can be a hidden variable if you are trying to determine whether a prompt change caused an output change.

---

# ✨ INSPIRE

Inspire uses a playlist as a creative springboard for a new song.

Best practice:

```text
Short focused playlist
↓
Inspire
↓
Select useful idea
↓
Refine in V6
```

A focused playlist of a few relevant songs is generally easier to reason about than an enormous mixed playlist.

---

# 🔊 SOUNDS

Suno Sounds generates individual audio material such as one-shots, loops, samples, effects and ambient sounds. Loop workflows can include key/BPM information. It is a separate sound-generation surface from full-song generation.

Use it for:

- percussion layers
- transitions
- atmospheres
- instrument samples
- one-shot impacts
- loops

Then bring useful material into the larger production workflow.

---

# 🧪 SAMPLE & MASHUP

### Sample

Use a selected musical moment as the starting point for a new creation. This is best when you want to preserve the identity of an idea while changing its context.

### Mashup

Assign explicit roles to multiple sources:

```text
SOURCE A → vocal identity
SOURCE B → drums
SOURCE C → harmonic/synth palette
NEW SONG → original arrangement / lyrics
```

V6 officially supports multi-source mashups and sample/isolate workflows. citeturn0search0

---

# ✂️ EDITING: EXTEND / CROP / REPLACE / REUSE / ADJUST

### Extend

Continue an existing song while describing the musical job of the next section.

```text
Extend into a final chorus. Increase drum energy, widen synth layers, add stacked harmonies and create a clear emotional peak before a short instrumental outro.
```

### Crop

Remove unwanted beginning/end material without regenerating the entire song.

### Replace Section

Use when one section is wrong while the surrounding song is valuable. The original can remain recoverable through take-lane/undo workflows in Studio.

### Reuse Prompt

Reuse an existing generation setup, then change one variable to create controlled alternatives.

### Adjust Speed

Use when a speed change is the appropriate musical edit rather than rebuilding the whole song.

### Rescue hierarchy

```text
BAD WORD / LINE → lyric edit
LOCAL MOMENT → localized edit
BAD SECTION → Replace Section
BAD INSTRUMENT → stems / Studio
BAD MIX → stems / Studio / DAW
BAD WHOLE SONG → regenerate
```

---

# ✏️ SONG EDITOR / NATURAL-LANGUAGE EDITING

V6 supports natural-language localized editing and single-lyric changes. citeturn0search0

Examples:

```text
Change only the word “love” to “light” in the second chorus.
```

```text
Keep the existing vocal and arrangement. Replace only the bridge with a darker harmonic section.
```

```text
Keep the chorus unchanged. Make Verse 2 more intimate and sparse.
```

The governing rule is:

> **Do not rebuild the entire song when the actual defect is local.**

---

# 🎙️ ADD VOCALS

Add Vocals is for adding a generated vocal layer to an instrumental/existing track.

```text
Instrumental
↓
Define vocal identity
↓
Lyrics / direction
↓
Generate vocal
↓
Evaluate phrasing + identity
↓
Edit / stem-process
```

Use it when the instrumental is already worth preserving and only the vocal layer needs work.

---

# ✨ REMASTER

Remaster is for **subtle refinement**, not radical songwriting changes.

Current documented variation choices are:

```text
Subtle  → closest to original
Normal  → default balance
High    → more noticeable variation
```

Use it for overall sound, balance, texture and clarity. Use Cover/Edit/Replace when the musical content itself needs substantial transformation.

---

# 🥁 STEM SEPARATION

Current extraction modes:

| Mode | Result | Availability | Cost |
|---|---|---|---:|
| **Auto Split** | Up to 12 broad categories | Pro / Premier | 50 credits/extraction |
| **Split from Mix** | One selected instrument/voice + complement | Pro / Premier | 10 credits/stem |
| **Advanced Split** | Select from nearly 100 instruments | Premier | 10 credits/stem |

These costs are currently documented by Suno. citeturn2search4

### Where to get stems

From Library/Workspace:

```text
More Actions (...) → Get Stems → choose split → Extract
```

From Studio:

```text
Right-click audio clip → Split Stems → choose split → Extract
```

citeturn2search4

### Stem rescue

```text
FULL SONG
↓
SEPARATE
↓
SOLO
↓
IDENTIFY BAD ELEMENT
↓
MUTE / REPLACE / PROCESS
↓
REBALANCE
↓
EXPORT
```

---

# 🎛️ STUDIO 2.0

Studio 2.0 is Suno's browser-based generative DAW and is available to Premier subscribers. It adds a production environment around generation: automation, effects, MIDI, wavetable synthesis, custom plugins, recording, stems and Chat Bar workflows. citeturn2search9

### Current environment

- Desktop/laptop/tablet; minimum 768px screen width.
- Mobile devices are not supported for Studio.
- Chrome is recommended.
- Safari Web MIDI is not supported.
- Minimum hardware: CPU with SSE4.1 or Neon SIMD support and at least 4 GB RAM. citeturn2search9

### Studio mental model

```text
Suno generation
↓
Studio timeline
↓
Edit / generate / record
↓
Stems / MIDI
↓
Synths / effects
↓
Automation
↓
Mix
↓
Export
```

---

# 💬 STUDIO CHAT

The Chat Bar is the natural-language production layer inside Studio. It can generate audio/MIDI, arrange, create plugins, design synth presets and make project changes. citeturn2search9

A September 2026 Studio update made the Chat Bar BPM-aware, improved reliability, added undo for prompt edits, and improved plugin duplication/movement. citeturn0search2

### Strong prompt

```text
On the vocal track, reduce harsh high-mid character, keep the vocal forward, preserve the existing dynamics, and do not change the drums or bass.
```

The more specific the requested scope, the easier it is to protect unrelated parts.

---

# 🎹 STUDIO MIDI

Studio 2.0 supports MIDI tracks, piano-roll editing, musical typing, external MIDI input and audio↔MIDI workflows. citeturn2search9

MIDI lets you edit:

```text
NOTE
TIMING
DURATION
VELOCITY
PITCH
INSTRUMENT
```

### Audio → MIDI

Drag an audio clip onto a MIDI track to transcribe it into notes in supported workflows.

### MIDI → audio

Use MIDI as the musical instruction for generated/Studio audio creation.

### Musical typing

The computer keyboard can act as a MIDI controller; Studio also provides chord modes and an arpeggiator. citeturn2search9

---

# 🌊 WAVETABLE SYNTH

Use the built-in wavetable synth for:

- bass
- pads
- leads
- plucks
- chords
- evolving textures

Studio's September update also improved high-frequency wavetable fidelity and reduced aliasing. citeturn0search2

Describe sound in behavior, not adjectives:

```text
Warm analog-style bass, rounded low end, subtle harmonic saturation, slow filter movement, short attack, controlled decay, enough midrange definition for small speakers.
```

---

# 🎚️ EFFECTS & CUSTOM PLUGINS

Built-in effects include:

- Compressor
- Convolution
- Delay
- Distortion
- EQ
- Gate
- Reverb

Studio does **not** host conventional VST or Audio Unit plugins. Instead, custom plugins can be designed through the Chat Bar. citeturn2search9

Custom plugins can support presets, automation and MIDI Learn. citeturn2search9

### Plugin management

September 2026 updates added:

```text
Drag/drop → move/copy between tracks
Cmd-D / Ctrl-D → duplicate plugin on same track
Option-drag → duplicate across tracks
```

citeturn0search2

---

# 📈 AUTOMATION

Automation can control track parameters such as:

- volume
- panning
- plugin parameters
- filter movement
- reverb/delay behavior
- effect intensity

MIDI Learn can map compatible hardware controls to Studio parameters. citeturn2search9

Automation is the right tool when a sound should **change over time** rather than remain permanently altered.

---

# 🎛️ RECORDING / EDITING / TAKE LANES

Every generation produces two versions. Take Lanes let you audition, rate and promote the strongest version without immediately destroying the alternatives. citeturn2search2

Take Lanes can also preserve the original when using Replace Section.

### Current Take Lane workflow

```text
Generate
↓
Audition takes
↓
Rate if desired
↓
Compare
↓
Promote/Commit best take
↓
Keep original recoverable
```

Suno documents keyboard access to the Take Lanes view and a non-destructive commit workflow. citeturn2search2

### Remove FX / Get Dry

Studio's Remove FX uses AI to strip baked-in reverb, delay and other effects, creating a dry version as a new take lane. citeturn2search0

Use this when you want to rebuild the effect chain yourself rather than processing an already-wet recording.

### Timing / time signature

Studio includes project tempo and time-signature controls. Earlier Studio 1.2 introduced Warp Markers and additional time-signature support; treat these as production tools for timing correction and meter setup rather than generation prompts. citeturn2search1

---

# 📚 LIBRARY / WORKSPACES

### Library

The Library organizes songs and provides filters, playlists and Hooks. citeturn2search11

### Workspaces

Workspaces organize songs/edits while creating. They are especially useful for separating Extend branches, experiments and project variants. citeturn2search6

### Studio Library

Studio's right-side Library dock can show All Songs, Liked, Stems, Uploads, Workspaces and Studio Projects. It is searchable/filterable; songs can be auditioned and dragged onto the timeline or into Chat. citeturn2search5

A song's details can include Stems and Notes tabs. citeturn2search5

---

# 📦 STUDIO EXPORT

Current Studio export options include:

- Full Song
- Selected Time Range
- Multitrack
- Individual clip WAV
- MIDI extracted from supported stems

All Studio audio exports are high-quality WAV. Exporting MIDI from a stem currently costs **10 credits**. citeturn2search7

Studio can upload WAV, MP3 and MIDI. It can export full/selected/multitrack audio and individual stem WAVs. citeturn2search9turn2search7

---

# 🎚️ PRODUCTION VOCABULARY

### Vocals

```text
intimate • close-mic • breathy • airy • dry • wet • forward • recessed
warm • bright • dark • raspy • smooth • husky • chest voice • falsetto
stacked harmonies • double-tracked • call-and-response
```

### Drums

```text
punchy • tight • transient-heavy • soft • dry • roomy • compressed
four-on-the-floor • half-time • syncopated • swung • humanized • mechanical
```

### Bass

```text
sub-heavy • round • controlled • growling • clean • saturated
sidechain-pumped • short • sustained • mid-bass focused
```

### Synths

```text
analog • warm • cold • glassy • metallic • shimmering • textured
wide • mono • stereo • filtered • resonant • pulsing • arpeggiated
```

### Mix

```text
vocal-forward • centered • wide • deep • open • controlled low end
clean kick-bass separation • clear midrange • smooth high end
transient definition • restrained reverb • short room • long tail
```

### Master

```text
dynamic • controlled • open • clean • polished • punchy
transparent • warm • bright • balanced
```

---

# 🎤 VOCAL ENGINEERING

Describe more than gender:

```text
register
+ texture
+ delivery
+ emotional behavior
+ phrasing
+ harmony behavior
+ mix position
```

Example:

```text
Low-register male lead vocal, mature emotional character, slightly husky texture, intimate close-mic verses, restrained intensity, stronger chest voice in choruses, natural conversational phrasing, selective stacked harmonies, centered and forward without excessive brightness.
```

### Vocal troubleshooting

**Too weak:** forward lead, stronger projection, vocal-led arrangement.

**Too theatrical:** restrained emotional delivery, conversational phrasing, intimate performance.

**Too wet:** dry close vocal, restrained room ambience, minimal vocal reverb.

**Too buried:** vocal-forward center image and reduced competing midrange density.

---

# 🎼 ARRANGEMENT ENGINEERING

Describe **movement** rather than merely naming instruments.

```text
Sparse piano-led verse
→ rising bass and percussion
→ full punchy chorus
→ reduced bridge
→ expanded final chorus
```

The arrangement should explain where energy enters, peaks, retreats and resolves.

---

# 🔊 AUDIO / MIX / MASTER QUALITY

Listen for:

- vocal clarity
- kick/bass interaction
- low-mid buildup
- harshness
- stereo stability
- transient definition
- clipping/distortion
- timing drift
- unwanted artifacts
- unnatural vocal phrasing
- transitions
- ending quality

### Loudness ≠ quality

Excessive loudness can reduce transient impact, dynamic contrast and clarity.

### Fake precision warning

A text prompt such as `-1 dB at 3.2 kHz, Q 1.4, 4:1 compression, -14 LUFS` does not automatically create DAW-style numerical processing. Use exact numbers only when the actual tool exposes a numerical control.

---

# 🔁 REPEATABILITY / SAME CHORUS

Keep these variables stable:

```text
lyrics
core Style identity
chorus descriptors
references
model
```

But remember:

```text
LYRIC CONSISTENCY
≠ MELODIC CONSISTENCY
≠ VOCAL CONSISTENCY
≠ ARRANGEMENT CONSISTENCY
```

When exact identity matters, stop asking generation to perform a job better handled by editing, stems or Studio.

---

# ❌ FAILURE MODES

### Prompt soup
Choose one primary identity.

### Too many adjectives
Describe audible behavior.

### Contradictions
Assign contrasting characteristics to different sections instead of asking for everything simultaneously.

### Changing too many variables
Change one major variable per test.

### Fixing arrangement with mastering language
Fix the arrangement.

### Fixing lyrics with production
Edit the lyrics.

### Rebuilding a great song for one bad section
Use localized editing.

### Treating tags as commands
Treat undocumented tags as probabilistic cues.

### Chasing retired-model behavior
Translate the intent into current V6 behavior and retest.

---

# 🔬 SCIENTIFIC TESTING

A proper test freezes everything except the variable under investigation.

```text
BASE PROMPT
MODEL = fixed
LYRICS = fixed
REFERENCES = fixed

TEST A → baseline
TEST B → change one slider
TEST C → change one prompt variable
TEST D → change one reference
```

Log:

```text
DATE
MODEL
PLAN
PROMPT
LYRICS
SLIDERS
REFERENCES
MAX MODE
OUTPUT IDS
WHAT WORKED
WHAT FAILED
NEXT TEST
```

Generative variance means one successful output does not prove causation.

### A/B scoring rubric

| Category | Score 1–10 |
|---|---:|
| Vocal quality | |
| Vocal consistency | |
| Melody | |
| Lyrics delivery | |
| Arrangement | |
| Drums | |
| Bass | |
| Instrument separation | |
| Emotional impact | |
| Mix quality | |
| Overall | |

---

# 🚑 PRODUCTION RESCUE

```text
SONG IS ALMOST RIGHT
↓
Identify exact defect
↓
WORD / LINE → lyric edit
LOCAL MOMENT → localized edit
SECTION → Replace Section
INSTRUMENT → stems / Studio
MIX → stems / Studio / DAW
SONIC FINISH → Remaster / Studio
WHOLE SONG → regenerate
```

This is one of the guide's foundational rules:

> **Preserve good information. Repair bad information locally.**

---

# 🤖 SUNO + CHATGPT WORKFLOW

Use ChatGPT as a creative/technical co-pilot, but use your ears as the final authority.

```text
IDEA
↓
ChatGPT: clarify concept
↓
Lyrics
↓
ChatGPT: improve singability / structure
↓
Style prompt
↓
Suno V6
↓
Listen
↓
Describe actual failure
↓
ChatGPT: diagnose smallest correct fix
↓
Change one variable
↓
Generate
↓
Compare
↓
Edit / stems / Studio
```

Useful diagnostic prompt:

```text
Analyze this Suno V6 result as a production engineer.
Do not rewrite everything.
Identify the three biggest audible problems.
For each problem classify the correct fix as:
1. lyric change
2. Style change
3. slider/reference change
4. regeneration
5. section replacement
6. stems
7. Studio processing
Then give me the smallest change likely to fix each problem.
```

---

# 🍳 GENRE COOKBOOK

These are starting points, not guaranteed formulas.

### Dark Electropop

```text
Dark emotional electropop, intimate expressive male lead vocal, warm analog polysynths, controlled sub bass, tight punchy electronic drums, sparse nocturnal verses, rising pre-chorus tension, huge bittersweet melodic chorus, layered harmonies, wide synth textures, vocal-forward center image, clean kick-bass separation, restrained reverb, smooth open high end, preserved dynamics.
```

### Indie Pop

```text
Intimate nocturnal indie pop, close expressive lead vocal, warm electric piano, soft analog synth pads, round bass, understated electronic percussion, sparse verses, subtle stereo movement, natural phrasing, gradual dynamic growth, minimal reverb, clear midrange, controlled low end.
```

### Synthwave

```text
Cinematic modern synthwave, analog polysynth chords, pulsing arpeggiator, deep controlled synth bass, gated electronic drums, wide chorus synths, nocturnal atmosphere, strong melodic hook, dramatic builds, neon retro-futurist texture, punchy transients, controlled stereo width.
```

### Cinematic Ballad

```text
Cinematic alternative pop ballad, intimate low-register lead vocal, piano foundation, soft strings, atmospheric synths, subtle sub bass, restrained percussion, sparse verse, rising pre-chorus, expansive chorus, layered harmonies, natural room ambience, vocal-forward center image, preserved dynamics.
```

---

# 💼 PLANS / CREDITS / DOWNLOADS / RIGHTS

### Current download rules

| Plan | Downloads | Commercial-use note |
|---|---:|---|
| Free | Up to 7 lifetime trial downloads for eligible accounts | Trial downloads are personal/non-commercial |
| Pro | 20/month | Paid-plan downloads have commercial-use rights under Suno's terms |
| Premier | 60/month | Paid-plan downloads have commercial-use rights under Suno's terms |

Monthly paid download allowances reset on the billing date and unused downloads do not roll over. A song counts once regardless of format; re-downloading the same song does not consume another quota unit, and stems from the same song count as part of that song's download. citeturn2search3

Suno says existing songs remain playable/shareable in the platform; download limits are distinct from listening/sharing. citeturn2search3

### Generation credits ≠ downloads

```text
GENERATION CREDITS
≠
DOWNLOAD ALLOWANCE
```

Current V6 generation pricing is documented as two songs per 10 credits. Max Mode costs more; image/video-heavy generation can increase cost. citeturn0search7

### Rights warning

Paid-plan commercial-use rights are not the same thing as a guarantee of copyright protection. Copyright eligibility varies by jurisdiction and by the human contribution involved. User-written lyrics remain subject to the user's rights; third-party lyrics, voices, samples and source material require appropriate permission.

This guide is not legal advice. Always read the current Suno Terms for your actual use case.

---

# 📱 MOBILE / WEB ECOSYSTEM

Current Suno is not only the Create page.

Recent/current ecosystem features include:

- Voices on iOS and Android.
- Offline playlist listening on mobile.
- Playlist shuffle on web, with mobile rollout timing subject to Suno's current release state.
- Playlist search/filtering/reordering/pinning features.
- Cover-art generation/iteration on web for songs, playlists and profiles.
- iOS Notes → lyrics creation.
- iOS Voice Memos → audio input.
- iMessage keyboard creation/sharing on iOS.
- Android Auto / CarPlay integration.
- Hooks for short-form music-video pairing.

Suno's release notes are the authoritative place for rollout status because mobile features can arrive at different times on iOS, Android and web. citeturn0search1

### Important distinction

```text
OFFLINE PLAYLISTS
≠
OFFLINE SONG CREATION
```

Offline playlist support is for listening to saved playlists; do not assume it means the full generative creation system works offline.

---

# 🛡️ MODERATION / SAFEGUARDS / SOURCE MATERIAL

Suno may moderate generated or submitted material. Uploaded audio/lyrics can also be screened for unauthorized use under Suno's safeguards.

Do not design workflows around attempts to bypass moderation or rights protections.

When a source is important to a project, keep a record of:

```text
SOURCE
OWNER / PERMISSION
DATE ACQUIRED
WHERE IT CAME FROM
HOW IT IS USED
```

---

# 🧾 MUSIC GLOSSARY / TERMINOLOGY

Use Suno's Music Glossary when you need a precise musical term rather than a generic adjective. Useful categories include:

```text
rhythm
meter
groove
tempo
instrumentation
vocal technique
harmonic language
arrangement
production
mixing
mastering
```

The glossary is a vocabulary aid, not a list of guaranteed prompt commands.

---

# ⌨️ STUDIO SHORTCUTS

| Action | Shortcut |
|---|---|
| Record | `Shift-R` |
| Play / Stop | `Spacebar` |
| Metronome | `Shift-C` |
| Loop | `Cmd-L` |
| Solo for timing checks | `Shift-S` |

Studio also uses number-key toggles for major panels such as Take Lanes and Library in current workflows; exact shortcuts can change, so verify the live Studio shortcut reference before relying on them.

---

# 🛠️ TROUBLESHOOTING

### Too random

```text
Lower Weirdness.
Lower Variety when appropriate.
Increase Style Influence.
Simplify contradictory instructions.
Use V6 rather than V6-WILD.
```

### Too generic

```text
Strengthen primary identity.
Specify audible instrument behavior.
Define vocal character.
Define arrangement movement.
Remove vague adjectives.
```

### Ignores Style

```text
Check Variety.
Try Variety = 0 when preserving supplied style tags matters.
Increase Style Influence.
Remove conflicting genres.
Simplify.
```

### Chorus changes too much

```text
Keep lyrics identical.
Keep chorus descriptors identical.
Keep core Style stable.
Keep references stable.
Use Max Mode when justified.
Use editing/stems/Studio when exact continuity matters.
```

### Vocal buried

```text
vocal-forward
clear center image
less competing midrange density
restrained arrangement around vocal phrases
```

### Muddy mix

```text
controlled low end
clean kick-bass separation
uncluttered low mids
clear midrange
restrained reverb
```

### Studio timing problems

Turn on the metronome, solo the relevant instrument, inspect the timeline and check generated clips against the beat. Suno acknowledges that timing issues can still occur in Studio 2.0. citeturn2search9

---

# 🧠 MASTER WORKFLOW

```text
1. DEFINE SONG CONCEPT
2. DEFINE EMOTIONAL TARGET
3. CHOOSE PRIMARY GENRE
4. DEFINE VOCAL IDENTITY
5. ENGINEER LYRICS
6. BUILD STYLE
7. CHOOSE MODEL
8. SET SLIDERS
9. ASSIGN REFERENCE ROLES
10. USE MAX MODE ONLY WHEN JUSTIFIED
11. GENERATE
12. LISTEN
13. SCORE
14. IDENTIFY ONE BIGGEST FAILURE
15. CHANGE ONE VARIABLE
16. GENERATE AGAIN
17. KEEP BEST TAKE
18. SURGICALLY EDIT WEAK SECTIONS
19. EXTEND / CROP / ADD VOCALS AS NEEDED
20. REMASTER WHEN THE WHOLE SONIC CHARACTER NEEDS REFINEMENT
21. SEPARATE STEMS WHEN ELEMENTS NEED INDIVIDUAL CONTROL
22. OPEN IN STUDIO
23. EDIT AUDIO / MIDI
24. DESIGN SYNTHS
25. ADD EFFECTS
26. AUTOMATE
27. BALANCE
28. QC
29. EXPORT
30. VERIFY RIGHTS / METADATA / FINAL FILES
```

---

# 📋 CREATION LOG

```text
PROJECT:
SONG:
DATE:
MODEL:
PLAN:
MODE: Simple / Custom
LYRICS VERSION:
STYLE VERSION:
REFERENCE INPUTS:
VOICE:
CUSTOM MODEL:
MY TASTE:
WEIRDNESS:
STYLE INFLUENCE:
AUDIO INFLUENCE:
VARIETY:
MAX MODE:
DURATION:
OUTPUT IDS:
BEST TAKE:
FAILURE:
CHANGE MADE:
RESULT:
NEXT TEST:
```

---

# 📚 OFFICIAL RESOURCE LIBRARY

### V6

- urlCurrent Models: V6https://help.suno.com/en/articles/13924737
- urlV6 FAQhttps://help.suno.com/en/articles/13924481
- urlWhat's New in V6https://help.suno.com/en/articles/13924801
- urlHow to Change Modelshttps://help.suno.com/en/articles/13924993
- urlIntroducing V6https://suno.com/release-notes/introducing-v6

### Creation

- urlMaking Music Help Centerhttps://help.suno.com/en/categories/550017
- urlCreative Slidershttps://help.suno.com/en/articles/6141377
- urlCustom Modelshttps://help.suno.com/en/articles/11362497
- urlVoiceshttps://help.suno.com/en/articles/11362369
- urlMy Tastehttps://help.suno.com/en/articles/11362561
- urlSuno Soundshttps://help.suno.com/en/articles/10625537

### Editing / Production

- urlStudio 2.0https://help.suno.com/en/articles/13670529
- urlStudio 2.0 Help Categoryhttps://help.suno.com/en/categories/2701953-studio-2-0
- urlAdvanced Stem Separationhttps://suno.com/release-notes/advanced-stems
- urlHow to Get Stemshttps://help.suno.com/en/articles/13925185
- urlTake Laneshttps://help.suno.com/en/articles/13670913
- urlRemove FX / Get Dryhttps://help.suno.com/en/articles/13671105
- urlAccess Library in Studiohttps://help.suno.com/en/articles/13670849
- urlExporting from Studiohttps://help.suno.com/en/articles/13925249

### Organization / Ecosystem

- urlWorkspaceshttps://help.suno.com/en/articles/4326849
- urlSuno Release Noteshttps://suno.com/release-notes
- urlSuno Bloghttps://suno.com/blog

### Downloads / Terms

- urlDownload Limitshttps://help.suno.com/en/articles/13926209
- urlDownloads, Models & Terms FAQhttps://help.suno.com/en/articles/13614785

---

# 🗓️ CURRENT V6 TIMELINE

### July 2026

Major lyric/editor improvements, cover-art iteration and other creation-surface improvements landed during the pre-V6 period.

### August 2026

Studio 2.0 launched with MIDI, effects, wavetable synthesis, automation, Chat Bar, custom plugins and improved production workflows. Voices expanded to iOS/Android. Playlist and mobile improvements continued. citeturn0search1turn0search13

### September 2026

V6 launched on September 9, with:

```text
V6      = flagship / control
V6-WILD = exploration
V6-MINI = fast / accessible
```

Suno also updated Studio on September 2 with BPM-aware Chat Bar behavior, plugin copy/duplicate improvements, wavetable fidelity improvements and performance/bug fixes. citeturn0search0turn0search2

---

# 🚫 WHAT THIS GUIDE WILL NEVER CLAIM

This repository will never present these as facts without evidence:

- undocumented secret commands
- guaranteed exact melodies from prompts
- guaranteed exact BPM from ordinary text
- hidden slider behavior without evidence
- 100% reliable community tricks
- identical behavior between retired models and V6
- copyright protection simply because Suno grants commercial-use rights
- permission to clone another person's voice simply because the feature technically allows voice input
- old tutorials as current truth

The guide separates:

```text
DOCUMENTED
REPRODUCIBLE
COMMUNITY
EXPERIMENTAL
UNKNOWN
RETIRED
```

---

# 🧠 FUNDAMENTAL RULES

1. **Write for the ear, not the checkbox.**
2. **One primary musical identity beats ten competing identities.**
3. **Concrete audible behavior beats generic adjectives.**
4. **Change one major variable when testing.**
5. **Listen before rewriting the prompt.**
6. **Preserve excellent material; repair bad material locally.**
7. **Use V6-WILD for discovery and V6 for controlled refinement.**
8. **Use Max Mode when fidelity/consistency justifies the extra cost.**
9. **Use stems and Studio when the problem is production.**
10. **Do not confuse probabilistic generation with deterministic programming.**
11. **Document experiments.**
12. **When official documentation changes, the guide changes.**

---

# 🔄 MAINTENANCE STANDARD — HOW TO ADD FUTURE FEATURES

Every future Suno feature should be documented with:

```text
WHAT IT IS
WHO HAS IT
WHERE IT LIVES
WHAT IT DOES
HOW TO USE IT
WHEN TO USE IT
WHEN NOT TO USE IT
LIMITATIONS
PLAN / CREDIT IMPACT
INPUT / OUTPUT
INTERACTIONS WITH OTHER FEATURES
KNOWN FAILURE MODES
OFFICIAL SOURCE
COMMUNITY OBSERVATIONS
TESTING METHOD
DATE VERIFIED
```

When Suno changes a feature, update the old description instead of allowing contradictory versions to accumulate.

---

# ⚠️ ACCURACY POLICY

Suno is an evolving product. UI labels, feature availability, plan restrictions, credit costs, download rules, model behavior and supported workflows can change.

**Official Suno documentation and release notes are the live authority.**

This repository intentionally distinguishes:

- officially documented behavior
- directly observed/reproducible behavior
- community techniques
- speculation/unknown behavior

The objective is not to claim impossible omniscience. The objective is to maintain the most complete, useful, testable and current V6 knowledge base possible.

---

<p align="center"><strong>🎵 LIL SYNN's COMPLETE SUNO V6 GUIDE 🎵</strong><br><em>Hear the idea. Engineer the prompt. Generate. Listen. Refine. Produce. Repeat.</em></p>
