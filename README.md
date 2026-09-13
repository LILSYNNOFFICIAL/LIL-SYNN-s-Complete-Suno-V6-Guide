# 🎵 LIL SYNN's Complete Suno V6 Guide

### The Advanced Suno V6 Creation, Prompting, Editing, Production, Audio Quality, Structure, AI-Assisted Songwriting, Studio, Licensing, Troubleshooting & Research Knowledge Base

<p align="center"><strong>THE GOD GUIDE TO SUNO V6</strong><br>Creation • Models • Lyrics • Style • Tags • Sliders • Advanced Options • Max Mode • References • Voices • Custom Models • My Taste • Inspire • Sounds • Audio • Sample • Mashup • Extend • Crop • Editing • Remaster • Stems • Studio 2.0 • MIDI • Automation • Effects • Production • ChatGPT • Testing • Troubleshooting</p>

> **Current-reference date: September 13, 2026.** Suno changes quickly. This guide is intentionally a living knowledge base. Official Suno documentation takes priority over community posts, old screenshots, remembered behavior, and third-party tutorials.

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

- [What “All” and “Everything” Mean](#-what-all-and-everything-mean)
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

V6-WILD is deliberately more unpredictable. Use it when you want ideas you would not have designed yourself: unusual instrumentation, textures, arrangements, genre collisions, melodic turns, or unexpected transitions.

**Mental model:**

```text
V6-WILD = “Surprise me, but stay musical.”
```

A strong discovery workflow is:

```text
V6-WILD → discover interesting idea → identify what worked → rebuild/refine in V6
```

## V6-MINI

Use V6-MINI for fast prompt experiments, rough concepts, lyric tests, arrangement tests, and high-volume iteration.

**Mental model:**

```text
V6-MINI = “Test the idea quickly before spending time polishing it.”
```

## Model switching

Current Suno documentation says the model picker is in the Create form and can be changed at any time. Custom Models also appear in the model picker for eligible users. citehttps://help.suno.com/en/articles/13924993

---

# 🔄 V6 MIGRATION / RETIRED MODELS

Suno's September 2026 documentation says models before V6 have been retired. Existing songs remain in the library and can still be listened to, shared, remastered, and covered. New iterations use the current V6 family. Existing custom models are automatically upgraded so V6 powers them going forward, while songs previously made with old custom models remain available and unchanged. citehttps://help.suno.com/en/articles/13924481

### Important consequence

Do **not** assume an old tutorial's exact output is reproducible in V6 merely because the old model, prompt, or tag syntax once worked.

Treat older material as historical reference, then retest it under V6.

---

# 🏗️ V6 CREATION ARCHITECTURE

Think of Suno as a stack rather than one giant prompt:

```text
MODEL
  ↓
CREATION MODE
  ↓
STYLE / SONG IDENTITY
  ↓
LYRICS / CONTENT
  ↓
SECTION-SPECIFIC DIRECTION
  ↓
REFERENCES / AUDIO / IMAGE / VIDEO
  ↓
SLIDERS / ADVANCED OPTIONS
  ↓
GENERATION
  ↓
LISTEN + EVALUATE
  ↓
SURGICAL EDITING
  ↓
REMASTER / STEMS
  ↓
STUDIO / DAW
  ↓
FINAL EXPORT
```

The biggest mistake is trying to solve every problem at the generation stage.

**Generation creates the raw artistic material. Editing repairs local problems. Stems separate components. Studio performs production work. A DAW can perform final professional mastering/editing when needed.**

---

# 🪄 SIMPLE MODE VS CUSTOM MODE

## Simple Mode

Simple Mode is useful when you want to describe the musical result naturally and let Suno determine the appropriate generation workflow.

V6 is designed to understand complex natural-language directions and multiple references. Suno specifically says V6 can accept multiple inputs such as songs, playlists, audio uploads, images and video in supported workflows. citehttps://help.suno.com/en/articles/13924481

### Good Simple Mode prompt

```text
Dark emotional electropop about realizing you were the problem in a relationship. Intimate low-register male vocal, sparse nocturnal verses, rising tension into a huge bittersweet chorus, warm analog synths, controlled sub bass, tight electronic drums, layered harmonies, polished modern production, emotionally devastating but restrained rather than theatrical.
```

## Custom Mode

Custom Mode is preferable when you need explicit separation between lyrics and musical identity and want greater control over structure, style, and iterative testing.

Use it for:

- original lyrics
- carefully engineered Style prompts
- section-level cues
- controlled experiments
- repeatable workflow testing
- specific vocal/arrangement goals

---

# ✍️ LYRICS ENGINEERING

Lyrics are not only poetry. In Suno they are also part of the performance and arrangement input.

## Basic structure

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

## Production-oriented structure

```text
[Intro | instrumental | atmospheric synth swell | filtered drums]

[Verse 1 | intimate lead vocal | sparse arrangement | restrained delivery]

[Pre-Chorus | rising tension | bass opens | additional percussion]

[Chorus | full drums | wide synths | stacked harmonies | vocal forward]

[Verse 2 | reduced density | new counter-melody | intimate delivery]

[Pre-Chorus | larger build | increasing vocal intensity]

[Chorus | same core hook | full arrangement | stacked harmonies]

[Bridge | contrasting harmony | reduced drums | exposed vocal]

[Final Chorus | expanded harmonies | maximum emotional lift]

[Outro | instrumental release | final vocal phrase]
```

These instructions are **guidance**, not a deterministic programming language. Suno may interpret, reinterpret, ignore, or occasionally vocalize descriptive text.

## Lyric density

Avoid making every section a wall of instructions.

Good:

```text
[Verse 1 | intimate lead | sparse drums | restrained delivery]
```

Overloaded:

```text
[Verse 1 | intimate lead | sparse drums | exact EQ curve | exact compressor ratio | exact stereo position | no reverb | no distortion | exact LUFS | exact dB level | ...]
```

Put musical concepts in the Style prompt when they apply to the entire song. Put local performance/arrangement ideas in the relevant section.

## Lyric writing principles

### Strong chorus

A useful chorus normally has:

- a recognizable central hook
- repeatable phrasing
- melodic room for emphasis
- emotional escalation
- a phrase the listener can remember after one listen

### Verse contrast

Verses should normally provide new information, imagery, perspective, or emotional development rather than simply repeating the chorus idea.

### Bridge function

A bridge can change:

- harmony
- perspective
- instrumentation
- vocal intensity
- rhythmic feel
- lyrical information
- emotional temperature

A bridge that does none of these may feel like another verse.

---

# 🎨 STYLE BOX ENGINEERING

The Style Box is the song-wide musical identity layer.

## Style prompt anatomy

```text
PRIMARY GENRE
+ SUBGENRE
+ ERA / PRODUCTION FAMILY
+ VOCAL IDENTITY
+ CORE INSTRUMENTS
+ RHYTHM / GROOVE
+ HARMONY / TONAL FEEL
+ ARRANGEMENT ARC
+ DYNAMICS
+ ATMOSPHERE
+ MIX CHARACTER
+ MASTER CHARACTER
```

## Master Style template

```text
Primary identity: [genre + subgenre + era/production family].
Vocal: [register + texture + delivery + emotional behavior].
Core instruments: [3–7 important instruments].
Rhythm: [groove + drum character + tempo feel].
Harmony: [tonal/modal character if important].
Arrangement: [density progression and section arc].
Dynamics: [where the track grows, contracts, peaks and resolves].
Atmosphere: [environmental and emotional character].
Mix: [vocal position + stereo width + low-end behavior + transient behavior].
Master: [open + controlled + dynamic + polished].
```

## Avoid prompt soup

Bad:

```text
pop rock EDM hip hop R&B metal jazz cinematic orchestral hyperpop trap house techno folk
```

Better:

```text
dark electropop with cinematic synth-pop influence
```

Then describe **audible behavior**:

```text
intimate dry vocal, sparse verses, rising pre-choruses, huge melodic chorus, controlled sub bass, punchy electronic drums, wide synths, stacked harmonies, clean kick-bass separation, preserved dynamics
```

Generic adjectives are weaker than concrete sound descriptions.

Instead of:

```text
beautiful, amazing, professional, cinematic, high quality
```

prefer:

```text
vocal-forward, controlled low end, wide chorus, dry close vocal, defined transients, restrained reverb, preserved dynamic contrast
```

---

# 🧱 PROMPT ANATOMY

When a prompt becomes too long, protect information in this order:

```text
1. PRIMARY GENRE / IDENTITY
2. VOCAL IDENTITY
3. CORE INSTRUMENTS
4. RHYTHM / GROOVE
5. ARRANGEMENT
6. DYNAMICS
7. ATMOSPHERE
8. MIX CHARACTER
9. MASTER CHARACTER
```

Remove redundancy before removing identity.

```text
sad + heartbreaking + melancholic + somber + emotionally devastating
```

can often become:

```text
dark melancholic emotionally devastating
```

## Positive instruction vs exclusion

Use positive language when possible:

```text
restrained reverb, dry intimate vocal, controlled low end
```

rather than stacking dozens of prohibitions.

Negative language can still be useful when a recurring failure needs explicit correction:

```text
Avoid excessive vocal reverb and avoid muddy low-mid buildup.
```

But do not build the entire prompt from exclusions.

---

# 🏷️ STRUCTURE / META TAGS

Commonly useful section labels include:

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

Common performance vocabulary:

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
[Rap Verse]
[Ad-lib]
[Call and Response]
```

Common instrument vocabulary:

```text
[Guitar Solo]
[Piano Solo]
[Drum Solo]
[Bass Break]
[Synth Solo]
[Drum Fill]
[Acoustic Guitar]
[Piano]
[Strings]
```

### Important warning

These are useful organizational/performance cues, not guaranteed API commands. Community syntax should never be represented as a secret Suno programming language.

---

# 🎚️ CREATIVE SLIDERS

Suno's documented Creative Sliders include:

| Slider | Purpose |
|---|---|
| **Weirdness** | Moves from safer/more expected results toward more chaotic/unusual results. |
| **Style Influence** | Controls how closely the result follows the supplied Style input, from looser to stronger influence. |
| **Audio Influence** | Appears when using an Audio Upload and controls the influence of the uploaded audio. |
| **Variety** | In current V6 documentation, changes/updates style prompts to introduce variation; setting Variety to 0 is recommended when you want to retain full control of supplied style tags. |

Official Creative Sliders documentation describes Weirdness as Safe → Chaos with 50% as the normal expected result, and Style Influence as Loose → Strong. Audio Influence appears with Audio Uploads. citehttps://help.suno.com/en/articles/6141377

Current V6 documentation separately explains Variety: it is designed to introduce variety by adjusting/updating style prompts, and reducing it to 0 preserves supplied style tags. citehttps://help.suno.com/en/articles/13924481

## Practical slider strategy

### Controlled final

```text
Weirdness: low → moderate
Style Influence: strong
Audio Influence: moderate → strong when preserving a reference
Variety: low / 0 when exact style control matters
```

### Discovery

```text
Weirdness: moderate → high
Style Influence: moderate
Variety: moderate → high
```

### Reference preservation

Start conservatively. Increase Audio Influence or other preservation controls only when the source needs to remain more dominant.

### Experimental rule

Change **one slider at a time** when you are trying to learn what a slider actually does.

---

# ⚙️ ADVANCED OPTIONS

Advanced options change the generation environment and should be treated separately from lyrics and Style text.

The exact visible controls can change as Suno updates its interface, plan availability, and model family. Do not rely on screenshots from old versions as the definitive current UI.

### Important principle

```text
Prompt = what you want
Slider = how strongly / variably you want it explored
Reference = what source material should influence it
Model = which generation personality should execute it
```

Do not use a slider to compensate for a fundamentally bad Style prompt.

---

# 🧠 MAX MODE

Current V6 documentation says Max Mode costs more credits and is intended for cases where V6 should spend more effort getting the result right.

Suno specifically recommends it for:

- songs longer than two minutes
- covers where you want the result close to the original
- transferring one song's style to another
- maintaining vocal consistency
- maintaining style consistency throughout the track

For quick ideas and shorter songs, standard generation is normally sufficient. citehttps://help.suno.com/en/articles/13924481

### Max Mode mental model

```text
STANDARD = fast / efficient / normal generation
MAX     = spend more resources on difficult fidelity/consistency tasks
```

Do not assume Max Mode magically fixes bad source material. It is a better tool for difficult controlled tasks, not a substitute for good inputs.

---

# 🖼️ REFERENCES & MULTIMODAL CREATION

V6 supports richer reference workflows than older Suno generations.

Supported V6 workflows can use combinations of:

- Suno songs
- playlists
- audio uploads
- images
- video
- textual instructions

Suno explicitly describes multi-input reference workflows in its current V6 FAQ. citehttps://help.suno.com/en/articles/13924481

## Reference hierarchy

When combining multiple references, explicitly explain their roles.

Bad:

```text
Use all these references.
```

Better:

```text
Use Reference A for vocal character.
Use Reference B for drum groove and rhythmic energy.
Use Reference C for synth palette.
Use the supplied lyrics as the only lyrical source.
Do not copy unrelated structural elements from the references.
```

This makes the creative intent much clearer.

---

# 🎧 AUDIO UPLOADS

Audio Uploads are useful for:

- starting from an existing recording
- supplying a musical reference
- using a performance as source material
- testing Audio Influence
- feeding material into later transformation/editing workflows
- bringing outside material into Studio

When an Audio Upload is involved, Creative Sliders can include Audio Influence. citehttps://help.suno.com/en/articles/6141377

### Best practice

Use the cleanest source you legally control. Avoid unnecessary clipping, noise, extreme processing, or poor-quality conversions when the audio is intended to be a reference.

---

# 🎤 VOICES

Suno's Voices feature allows a creator to record or upload a voice and use it in songs. Suno recommends an acapella recording for best results, although background music can also be provided and Suno can isolate the vocal. Voices became available on iOS and Android in August 2026 and can be tried on free plans with additional access on paid plans. citehttps://help.suno.com/en/articles/11362369

## Voice workflow

```text
Clean voice recording
        ↓
Create / select Voice
        ↓
Confirm compatible model/workflow
        ↓
Build song
        ↓
Evaluate vocal identity
        ↓
Iterate lyrics / Style / arrangement
```

### Recording best practices

- quiet room
- minimal room reflections
- stable microphone position
- consistent distance
- clean vocal performance
- no unnecessary clipping
- avoid excessive effects unless intentionally part of the reference

### Identity consistency

Do not change several variables at once while evaluating voice behavior. First determine whether the vocal identity is correct; then work on arrangement and mix.

### Rights and consent

Only use voices you have permission to use. Do not treat a voice model as permission to imitate another person commercially or deceptively.

---

# 🧠 CUSTOM MODELS

Current Suno documentation says Custom Models are available to Pro and Premier users. You can build up to **three** private custom models using as few as **six songs**. Bulk Upload is supported, Suno says training takes roughly **2–5 minutes**, and you must own the rights to every song used. Custom Models are private and cannot be shared with other users. citehttps://help.suno.com/en/articles/11362497

## Custom Model preparation

Use a coherent training set.

A useful conceptual training set should have consistency in:

- vocal identity
- production philosophy
- genre family
- instrumentation
- songwriting approach
- mix character

Avoid training a single model with unrelated material if the goal is a coherent identity.

### Rights rule

```text
IF YOU DO NOT OWN / CONTROL THE RIGHTS:
DO NOT USE THE SONG IN YOUR CUSTOM MODEL TRAINING SET.
```

---

# 🧠 MY TASTE

My Taste is Suno's personalization system for learning preferences such as genres and moods and using them to personalize creation behavior and Magic Wand style augmentation.

Use it as a personalization layer rather than treating it as a replacement for explicit prompting.

### Controlled workflow

When evaluating a prompt scientifically, remember that personalized systems can influence outputs. If reproducibility matters, document whether personalization features are enabled and keep that condition consistent across tests.

---

# ✨ INSPIRE

Inspire is useful for turning existing musical material into a creative springboard.

Conceptually:

```text
Existing idea
   ↓
Inspire / reference
   ↓
New interpretation
   ↓
Select useful musical idea
   ↓
Refine with V6
```

Do not assume an inspired output will preserve the original exactly. Treat Inspire as a discovery/variation tool.

---

# 🔊 SUNO SOUNDS

Suno Sounds is an experimental/beta sound-generation workflow for creating things such as:

- one-shots
- loops
- sound effects
- instrument samples
- ambient noises

The current help documentation describes a **Create → Sounds** workflow with One Shot or Loop modes and BPM controls for loops. citehttps://help.suno.com/en/articles/10625537

### Production uses

```text
Generate sound
→ audition
→ trim / edit
→ layer with song
→ process in Studio
→ export if needed
```

---

# 🧪 SAMPLE / SAMPLING

Sampling workflows let a creator use a selected musical element or moment as a creative starting point.

Use sampling when you want to preserve a specific musical idea while changing its context.

### Good sample prompt

```text
Preserve the rhythmic identity of the supplied riff, but rebuild it as a dark analog synth hook with a wider stereo image and a more aggressive chorus arrangement.
```

### Do not over-constrain

If you require every micro-detail to remain identical, you may be better served by working from stems or the original audio in Studio/DAW rather than asking a generative model to reconstruct it.

---

# 🧩 MASHUP

V6 supports richer mashup workflows and can use multiple source inputs.

### Role-based mashup prompting

```text
SOURCE A → vocal identity
SOURCE B → drum groove
SOURCE C → harmonic / synth palette
NEW SONG → original arrangement and lyrics
```

Explicitly assign each source a job.

### Mashup quality rule

The more unrelated sources you throw into a prompt without roles, the more ambiguous the target becomes.

---

# ➡️ EXTEND

Use Extend when the existing song contains material worth preserving and you need additional music beyond the current section.

### Good Extend strategy

Describe what the next section should accomplish rather than simply saying “continue.”

```text
Extend into a final chorus. Increase drum energy gradually, introduce wider synth layers, add stacked harmonies, and create a clear emotional peak before a short instrumental outro.
```

### Continuity checklist

- vocal identity
- key / harmonic feel
- rhythmic feel
- instrumentation
- energy level
- lyrical narrative
- transition point

---

# ✂️ CROP

Crop is useful when the beginning/end of a generated song contains material you do not want to retain.

Use it before expensive downstream production when the unwanted material is structurally irrelevant.

### Production principle

```text
REMOVE BAD MATERIAL EARLY
KEEP GREAT MATERIAL INTACT
```

Do not repeatedly regenerate a great song just to remove a bad intro if a surgical editing tool can solve it.

---

# ♻️ REUSE PROMPT

Reuse Prompt is useful for inspecting and reusing the creative setup of an existing generation.

A disciplined reuse workflow:

```text
Good song
 ↓
Reuse prompt
 ↓
Change ONE important variable
 ↓
Generate alternatives
 ↓
Compare
```

This is especially useful for learning which part of a prompt actually caused an improvement.

---

# ✏️ SONG EDITOR / NATURAL-LANGUAGE EDITING

V6 significantly expands natural-language editing. Suno documents the ability to make localized changes, including changing a single word or line while leaving the rest intact in supported workflows. citehttps://help.suno.com/en/articles/13924481

### Surgical editing principle

```text
DO NOT REBUILD THE WHOLE SONG
IF ONLY ONE PART IS WRONG.
```

Examples:

```text
Change only the word “love” to “light” in the second chorus.
```

```text
Keep the existing arrangement and vocal identity. Replace only the bridge with a darker harmonic section.
```

```text
Keep the chorus unchanged. Make the second verse more intimate and sparse.
```

---

# 🔧 REPLACE SECTION

Replace Section is the appropriate tool concept when a local portion is bad while the rest is worth preserving.

### Rescue hierarchy

```text
BAD WORD / LINE
→ single lyric edit

BAD PHRASE / LOCAL MOMENT
→ localized edit / Replace Section

BAD SECTION
→ Replace Section / targeted generation

BAD ARRANGEMENT BUT GOOD SONG
→ stems / Studio

BAD WHOLE GENERATION
→ regenerate
```

This minimizes destruction of good material.

---

# 🎙️ ADD VOCALS

Add Vocals can be used when the musical bed exists but the vocal layer needs to be generated or replaced.

### Workflow

```text
Instrumental / existing track
        ↓
Define vocal identity
        ↓
Supply lyrics / direction
        ↓
Generate vocal
        ↓
Evaluate phrasing + pitch + identity
        ↓
Edit / replace / stem-process
```

Treat the instrumental and vocal as separate creative variables whenever possible.

---

# ✨ REMASTER

Remaster is best understood as a refinement workflow, not a guarantee of perfect mastering.

Use it when:

- the song is fundamentally right
- the overall sound needs refinement
- you want a different sonic finish
- the arrangement does not need major surgery

Do **not** use Remaster as the first response to a clearly wrong chorus, lyric, melody, or arrangement. Fix the underlying musical problem first.

---

# 🥁 STEM SEPARATION

Current Suno documentation describes multiple stem-separation levels:

- **Auto Split:** 12 categories.
- **Split from Mix:** selected instrument/vocal plus everything else.
- **Advanced Split:** nearly 100 instruments; available to Premier.

Advanced stem separation is also integrated into Studio. citehttps://suno.com/release-notes/advanced-stems

## Stem rescue workflow

```text
Full song
 ↓
Separate stems
 ↓
Solo each stem
 ↓
Identify the actual problem
 ↓
Mute / replace / process the bad element
 ↓
Rebalance
 ↓
Export
```

### Example

If the vocals are excellent but the drums are weak:

```text
DO NOT regenerate the entire song immediately.

Separate stems.
Keep the vocal.
Repair / replace the drums.
Rebalance the mix.
```

---

# 🎛️ SUNO STUDIO 2.0

Suno Studio 2.0 is a full production environment for Premier users. Suno describes it as including automation, effects, MIDI, a wavetable synth, advanced stems, recording, editing, chat-based production, and custom plugin creation. Studio is designed for desktop/laptop/tablet environments with at least 768px screen width; mobile devices are not supported. Google Chrome is recommended and Safari does not currently support Web MIDI. citehttps://help.suno.com/en/articles/13670529

## Studio mental model

```text
Suno generation
      ↓
Studio timeline
      ↓
Edit clips
      ↓
Generate / record / arrange
      ↓
Separate stems
      ↓
MIDI / synth
      ↓
Effects
      ↓
Automation
      ↓
Mix
      ↓
Export
```

---

# 💬 STUDIO CHAT

Studio Chat is a natural-language collaborator inside Studio.

Suno says the chat bar can be used to:

- generate audio clips
- generate MIDI clips
- create instruments/vocals
- design custom plugins
- arrange songs
- make mix changes
- ask project questions
- tidy sessions

It is currently described as beta in Studio documentation. citehttps://suno.com/blog/studio-2

### Strong Studio Chat prompt

```text
On the vocal track, reduce the harsh high-mid character, keep the vocal forward, preserve the existing dynamics, and do not change the drums or bass.
```

### Better than vague language

Bad:

```text
Make it sound better.
```

Better:

```text
Make the vocal clearer and more forward while preserving the current low end, drum transients, stereo width, and overall loudness.
```

---

# 🎹 STUDIO MIDI

Studio 2.0 supports MIDI tracks, piano-roll editing, musical typing, external MIDI input, and audio-to-MIDI / MIDI-to-audio workflows. citehttps://help.suno.com/en/articles/13670529

## MIDI capabilities

- draw notes
- move notes
- resize notes
- quantize
- adjust velocity
- pitch bend
- modulation
- use computer keyboard as MIDI controller
- use external MIDI controllers through Web MIDI
- generate audio from MIDI
- transcribe audio into MIDI in supported workflows

### Why MIDI matters

Audio is a finished waveform. MIDI is a description of musical events.

That means MIDI lets you change:

```text
NOTE
TIMING
DURATION
VELOCITY
PITCH
INSTRUMENT
```

without re-recording the entire performance.

---

# 🌊 STUDIO WAVETABLE SYNTH

Studio 2.0 includes a wavetable synth.

Use it for:

- basses
- pads
- leads
- plucks
- evolving textures
- experimental sounds

### Sound-design prompting concept

Instead of:

```text
cool synth
```

try:

```text
warm analog-style bass with a rounded low end, subtle harmonic saturation, slow filter movement, short attack, controlled decay, and enough midrange definition to remain audible on small speakers
```

The more the requested sound is described in audible behavior, the more useful the target becomes.

---

# 🎚️ STUDIO EFFECTS & CUSTOM PLUGINS

Studio 2.0 includes effects such as:

- Compressor
- Convolution
- Delay
- Distortion
- EQ
- Gate
- Reverb

Suno says Studio is **not compatible with conventional VST or Audio Units plugins**. Instead, creators can design custom effects/plugins through the Studio chat system. citehttps://help.suno.com/en/articles/13670529

## Custom plugin concept

You can describe an effect such as:

```text
Create a warm tape saturation effect with subtle wow and flutter, gentle high-frequency rolloff, mild harmonic coloration, and a mix control.
```

Suno says generated plugins can be saved, revised conversationally, and used with presets, automation, and MIDI Learn. citehttps://help.suno.com/en/articles/13670529

---

# 📈 STUDIO AUTOMATION

Automation lets you change parameters over time.

Useful automation targets include:

- volume
- panning
- plugin parameters
- filter movement
- reverb amount
- delay send
- distortion intensity

### Arrangement example

```text
VERSE
low vocal volume automation
minimal reverb

PRE-CHORUS
slow volume rise
slight filter opening

CHORUS
full level
wider stereo effect
larger reverb/delay

OUTRO
gradual volume reduction
```

Automation is often better than permanently changing a sound because it preserves movement and contrast.

---

# 🎛️ STUDIO RECORDING, EDITING & TAKE LANES

Studio 2.0 supports recording audio and MIDI into the timeline. Each generation produces two versions, and Studio's Take Lanes provide access to alternate generated takes. citehttps://help.suno.com/en/articles/13670529

### Take-selection workflow

```text
Generate
 ↓
Listen to Take A
 ↓
Listen to Take B
 ↓
Compare section by section
 ↓
Choose strongest material
 ↓
Commit the best take to timeline
```

Do not automatically choose the first generation.

---

# 📦 STUDIO EXPORT

Current Studio documentation says you can export:

- the full song
- a selected range
- the multitrack
- individual stems

Studio supports 32-bit WAV and MP3 export, with individual stems available as WAV. Suno's Studio 2.0 announcement describes high-quality 32-bit/48kHz multitrack/stem export for Premier Studio workflows. citehttps://help.suno.com/en/articles/13670529https://suno.com/blog/studio-2

Studio supports uploads including:

- WAV
- MP3
- MIDI

citehttps://help.suno.com/en/articles/13670529

---

# 🎚️ PRODUCTION VOCABULARY

Use production terms that correspond to audible results.

## Vocals

```text
intimate
close-mic
breathy
airy
dry
wet
forward
recessed
warm
bright
dark
nasal
raspy
smooth
husky
low-register
high-register
head voice
chest voice
falsetto
stacked harmonies
double-tracked
call-and-response
```

## Drums

```text
punchy
tight
transient-heavy
soft
dry
roomy
compressed
crushed
four-on-the-floor
half-time
syncopated
swinging
humanized
mechanical
```

## Bass

```text
sub-heavy
round
controlled
growling
clean
saturated
sidechain-pumped
short
sustained
mid-bass focused
```

## Synths

```text
analog
warm
cold
glassy
metallic
shimmering
textured
wide
mono
stereo
filtered
resonant
pulsing
arpeggiated
```

## Mix

```text
vocal-forward
centered
wide
narrow
deep
intimate
open
controlled low end
clean kick-bass separation
clear midrange
smooth high end
transient definition
restrained reverb
short room
long tail
```

## Master

```text
dynamic
controlled
open
clean
polished
punchy
transparent
warm
bright
balanced
```

Avoid contradictory combinations unless the contrast is intentional.

---

# 🎤 VOCAL ENGINEERING

A strong vocal prompt describes more than gender.

## Vocal identity template

```text
[gender / register]
+ [age impression]
+ [texture]
+ [delivery]
+ [emotional behavior]
+ [phrasing]
+ [harmonic behavior]
+ [mix position]
```

Example:

```text
Low-register male lead vocal, mature emotional character, slightly husky texture, intimate close-mic delivery in verses, restrained intensity, stronger chest voice in choruses, natural conversational phrasing, selective stacked harmonies, centered vocal image, clear forward presence without excessive brightness.
```

## Vocal failure diagnosis

### Too weak
Try:

```text
forward lead vocal, clear presence, stronger projection, vocal-led arrangement
```

### Too theatrical
Try:

```text
restrained emotional delivery, conversational phrasing, intimate performance, avoid exaggerated belting
```

### Too wet
Try:

```text
dry close vocal, restrained room ambience, minimal vocal reverb
```

### Too buried
Try:

```text
vocal-forward mix, clear center image, reduce competing midrange density
```

---

# 🎼 ARRANGEMENT ENGINEERING

Describe **energy movement**, not just instruments.

Weak:

```text
piano, drums, bass, synth
```

Strong:

```text
Sparse piano-led verse with minimal percussion → rising bass and additional rhythmic layers in pre-chorus → full punchy drums and wide synths in chorus → reduced instrumentation for bridge → expanded final chorus with stacked harmonies and additional counter-melody.
```

## Arrangement arc

```text
INTRO      = establish world
VERSE      = deliver information
PRE        = increase anticipation
CHORUS     = emotional/melodic payoff
VERSE 2    = develop
PRE 2      = build more strongly
CHORUS 2   = reinforce
BRIDGE     = contrast/reset
FINAL      = maximum payoff
OUTRO      = resolution
```

Not every song needs this exact structure. It is a starting architecture.

---

# 🎚️ MIX / MASTER PROMPTING

Suno is not a DAW, and textual mix instructions are not equivalent to numerical engineering controls. Still, production language can communicate desired sonic behavior.

## Useful mix prompt

```text
Vocal-forward center image, controlled sub bass, clear kick-bass separation, punchy drum transients, uncluttered low mids, wide but stable synth field, restrained reverb, smooth open high end, preserved dynamic contrast, polished modern master without excessive loudness distortion.
```

## Avoid fake precision

Do not assume that writing:

```text
-1.0 dB at 3.2 kHz, Q 1.4, 4:1 compression, -14 LUFS
```

causes Suno to perform exact DAW-style engineering. Use exact numeric instructions only where the specific tool genuinely supports numerical parameters.

---

# 🔊 AUDIO QUALITY

## Source quality

The quality of an input reference matters.

Prefer:

- clean recordings
- minimal clipping
- adequate headroom
- minimal unnecessary codec damage
- consistent level
- no accidental noise

## Generation quality

Do not judge a generation solely by loudness.

Listen for:

- vocal clarity
- kick/bass interaction
- harshness
- low-mid buildup
- stereo stability
- transient definition
- arrangement density
- clipping/distortion
- unwanted artifacts
- timing drift
- unnatural vocal phrasing

## Loudness is not quality

A louder master can sound more impressive for a few seconds while actually losing:

- transient impact
- dynamic contrast
- clarity
- emotional movement

---

# 🔁 REPEATABILITY / SAME CHORUS

One of the hardest goals in generative music is getting the same musical identity across repeated sections.

Use a layered strategy:

```text
1. Keep chorus lyrics identical.
2. Keep the core Style identity stable.
3. Describe chorus identity consistently.
4. Avoid unnecessary changes between repeated sections.
5. Use surgical editing when possible.
6. Use Max Mode for difficult consistency tasks where appropriate.
7. If exact audio identity is required, use stems/Studio/DAW rather than relying on generation alone.
```

### Important distinction

```text
LYRIC CONSISTENCY ≠ MELODIC CONSISTENCY ≠ VOCAL CONSISTENCY ≠ ARRANGEMENT CONSISTENCY
```

A song can repeat the same words while changing melody or performance.

---

# ❌ PROMPT FAILURE MODES

## 1. Prompt soup

Too many genres and contradictory directions.

**Fix:** choose one primary identity and 1–2 supporting influences.

## 2. Too many adjectives

```text
amazing epic beautiful incredible cinematic powerful emotional professional
```

**Fix:** describe audible behavior.

## 3. Contradictory instructions

```text
minimal and huge throughout
soft and aggressive throughout
raw and perfectly polished throughout
```

**Fix:** assign characteristics to different sections.

## 4. Changing too many variables

**Fix:** A/B one variable at a time.

## 5. Trying to fix arrangement with mastering language

**Fix:** repair the arrangement first.

## 6. Trying to fix a bad lyric with production

**Fix:** edit the lyric.

## 7. Rebuilding a great song because one section is bad

**Fix:** use localized editing / Replace Section / stems.

## 8. Assuming tags are commands

**Fix:** treat community tags as probabilistic guidance unless officially documented.

## 9. Overloading section tags

**Fix:** one section = one primary job.

## 10. Chasing an old model's exact behavior

**Fix:** translate the musical intent into current V6 language and test it.

---

# 🧪 COMMUNITY TECHNIQUES

Community techniques can be extremely valuable. They must be labeled correctly.

## Useful community experimentation areas

- bracketed section labels
- performance descriptors
- arrangement descriptors
- dynamic language
- vocal cues
- ad-lib notation
- call-and-response structures
- genre hybrid recipes
- repeated chorus engineering
- prompt compression
- iterative variation testing

## Community rule

If a technique appears to work:

```text
OBSERVE
 ↓
REPEAT
 ↓
CHANGE ONE VARIABLE
 ↓
REPEAT
 ↓
DOCUMENT
 ↓
LABEL AS:
OFFICIAL / REPRODUCIBLE / ANECDOTAL
```

Do not turn one lucky generation into a universal law.

---

# 🔬 SCIENTIFIC SUNO TESTING

To understand a Suno behavior, use controlled experiments.

## Test design

```text
BASE PROMPT
A = unchanged

TEST 1
A + Weirdness change

TEST 2
A + Style Influence change

TEST 3
A + one new instruction

TEST 4
A + one changed reference
```

Keep a log:

```text
DATE
MODEL
PLAN
PROMPT
LYRICS
SLIDERS
REFERENCES
MAX MODE
OUTPUT ID
WHAT WORKED
WHAT FAILED
```

## Why this matters

Generative outputs have variance. A single successful result does not prove causation.

---

# 🆚 A/B TESTING FRAMEWORK

## Question

> Does variable X improve result Y?

### Procedure

1. Freeze the base prompt.
2. Freeze lyrics.
3. Freeze model.
4. Freeze references.
5. Change only X.
6. Generate enough examples to detect a pattern.
7. Compare using a fixed rubric.

## Example scoring rubric

| Category | Score 1–10 |
|---|---:|
| Vocal quality |  |
| Vocal consistency |  |
| Melody |  |
| Lyrics delivery |  |
| Arrangement |  |
| Drums |  |
| Bass |  |
| Instrument separation |  |
| Emotional impact |  |
| Mix quality |  |
| Overall |  |

The goal is not fake scientific certainty. The goal is better evidence than intuition alone.

---

# 🚑 PRODUCTION RESCUE WORKFLOW

When a generated song is “almost perfect,” do not immediately regenerate.

```text
SONG IS ALMOST RIGHT
        ↓
What exactly is wrong?
        ↓
ONE WORD / LINE?
        → lyric edit

LOCAL PERFORMANCE?
        → section edit / Replace Section

WHOLE SECTION?
        → Replace Section / targeted generation

ONE INSTRUMENT?
        → stems / Studio

MIX BALANCE?
        → stems / Studio / DAW

OVERALL SONIC FINISH?
        → Remaster / Studio / DAW

FUNDAMENTALLY WRONG?
        → regenerate
```

This is one of the most important principles in the entire guide:

> **Preserve good information. Repair bad information locally.**

---

# 🤖 SUNO + CHATGPT WORKFLOW

ChatGPT is best used as a **creative/technical co-pilot**, not as a replacement for listening.

## Master workflow

```text
IDEA
 ↓
CHATGPT: clarify concept
 ↓
LYRICS
 ↓
CHATGPT: edit for singability / structure
 ↓
STYLE PROMPT
 ↓
CHATGPT: engineer Style
 ↓
SUNO V6
 ↓
LISTEN
 ↓
REPORT SPECIFIC FAILURES
 ↓
CHATGPT: diagnose
 ↓
CHANGE ONE VARIABLE
 ↓
SUNO
 ↓
COMPARE
 ↓
EDIT / STEM / STUDIO
 ↓
FINAL
```

## Useful ChatGPT request

```text
Analyze this Suno V6 result as a production engineer.
Do not rewrite everything.
Identify the three biggest audible problems.
For each problem, tell me whether the correct fix is:
1. lyric change,
2. Style change,
3. slider/reference change,
4. regeneration,
5. section replacement,
6. stems,
7. Studio processing.
Then give me the smallest change likely to fix each problem.
```

## 10/10 iteration loop

```text
GENERATE
→ LISTEN
→ SCORE
→ IDENTIFY BIGGEST FAILURE
→ CHANGE ONE VARIABLE
→ REGENERATE
→ COMPARE
→ KEEP / DISCARD
→ REPEAT
```

Do not keep changing prompts without listening.

---

# 🍳 GENRE PROMPT COOKBOOK

These are starting points, not guaranteed formulas.

## Dark Electropop

```text
Dark emotional electropop, intimate expressive male lead vocal, warm analog polysynths, controlled sub bass, tight punchy electronic drums, sparse nocturnal verses, rising pre-chorus tension, huge bittersweet melodic chorus, layered vocal harmonies, wide synth textures, vocal-forward center image, clean kick-bass separation, restrained reverb, smooth open high end, preserved dynamics, polished modern production.
```

## Indie Pop

```text
Intimate nocturnal indie pop, close expressive lead vocal, warm electric piano, soft analog synth pads, round bass, understated electronic percussion, sparse verses, subtle stereo movement, natural human phrasing, gradual dynamic growth, minimal reverb, clear midrange, controlled low end, emotionally vulnerable delivery.
```

## Synthwave

```text
Cinematic modern synthwave, analog polysynth chords, pulsing arpeggiator, deep controlled synth bass, gated electronic drums, wide chorus synths, nocturnal atmosphere, strong melodic hook, dramatic builds, neon retro-futurist texture, punchy transients, controlled stereo width, polished modern low end.
```

## Cinematic Ballad

```text
Cinematic alternative pop ballad, intimate low-register lead vocal, piano-led foundation, soft strings, distant atmospheric synths, subtle sub bass, restrained percussion, sparse verse, emotionally rising pre-chorus, expansive chorus, layered harmonies, natural room ambience, vocal-forward center image, wide uncluttered stereo field, preserved dynamics.
```

## Dark R&B / Pop

```text
Dark contemporary R&B-pop, intimate expressive lead vocal, deep controlled sub bass, muted electronic drums, warm electric piano, atmospheric synth textures, syncopated groove, restrained verses, sensual but emotionally tense pre-chorus, spacious chorus, layered harmonies, clean low end, smooth high frequencies, close vocal presence.
```

## Pop Rock

```text
Modern emotional pop rock, expressive lead vocal, live-feeling punchy drums, melodic electric guitar, controlled bass, atmospheric piano, dynamic verse-to-chorus expansion, wide guitar layers, strong melodic chorus, stacked vocal harmonies, energetic but polished drums, clear midrange, controlled low end, natural room ambience.
```

---

# 💼 COMMERCIAL USE / DOWNLOADS / TERMS

This section is especially important because Suno changed its download policy in September 2026.

Current Suno documentation says:

| Plan | Current download allowance | Commercial-use note |
|---|---:|---|
| **Free** | Up to 7 lifetime trial downloads for eligible accounts; newer accounts may receive trial downloads differently | Trial downloads are personal/non-commercial |
| **Pro** | 20 downloads/month | Paid-plan downloads have commercial-use rights under Suno's stated terms |
| **Premier** | 60 downloads/month | Paid-plan downloads have commercial-use rights under Suno's stated terms |
| **Premier + Studio** | Studio workflow downloads are not limited in the same way | Commercial-use rights remain subject to Suno's terms |

Suno says download limits apply to downloads beginning September 3, 2026, including older songs. Existing songs remain playable and shareable in Suno. Downloading the same song again does not consume another download, downloading multiple formats counts as one song download, and stems from the same song count as part of that song's download. Failed/interrupted downloads do not count. citehttps://help.suno.com/en/articles/13926209https://help.suno.com/en/articles/13926593

Suno's August 2026 Terms/Downloads announcement states that paid-plan songs downloaded by paying subscribers retain commercial-use rights under its stated terms, while free trial downloads are for personal use only. citehttps://suno.com/blog/suno-updates-tos

### Important legal disclaimer

This guide is not legal advice. Commercial rights, copyright, ownership, training-data rights, voice rights, samples, trademarks, and jurisdiction-specific law can be complicated. Always read Suno's current Terms of Service for your account and use case.

---

# 💳 PLANS / CREDITS / DOWNLOAD LIMITS

Current V6 generation pricing is documented as the same credit cost as previous generations: each generation produces two songs for a total of 10 credits. Suno notes that using many images/videos in prompts can increase credit cost. Max Mode costs more credits. citehttps://help.suno.com/en/articles/13924481

### Do not confuse:

```text
GENERATION CREDITS
≠
DOWNLOAD ALLOWANCE
```

A user can be able to generate while having limited remaining downloads.

---

# ⌨️ STUDIO KEYBOARD SHORTCUTS

Studio 2.0 emphasizes keyboard control. Current documentation explicitly gives examples including:

| Action | Shortcut |
|---|---|
| Record | `Shift-R` |
| Play / Stop | `Spacebar` |
| Metronome | `Shift-C` |
| Loop | `Cmd-L` |
| Solo instrument (timing-check workflow) | `Shift-S` |

Suno's Studio documentation also provides a dedicated current keyboard-shortcuts resource, and shortcut availability can change with platform/browser. citehttps://help.suno.com/en/categories/2701953-studio-2-0

---

# 🛠️ TROUBLESHOOTING DECISION TREE

## Song sounds wrong

```text
WRONG?
 ↓
What exactly is wrong?
 ↓
LYRICS → edit lyrics
VOCAL → revise vocal identity / voice / arrangement
MELODY → regenerate / edit section
INSTRUMENT → stems / Studio
ARRANGEMENT → section edit / regenerate
MIX → stems / Studio
MASTER → Remaster / Studio / DAW
```

## Too random

```text
Reduce Weirdness.
Reduce Variety when appropriate.
Strengthen Style Influence.
Simplify conflicting instructions.
Use V6 rather than V6-WILD.
```

## Too generic

```text
Strengthen the musical identity.
Specify instruments and audible behavior.
Specify vocal character.
Specify arrangement movement.
Reduce vague adjectives.
```

## Ignores Style

```text
Check Variety.
Reduce Variety toward 0 when you need supplied style tags preserved.
Increase Style Influence.
Remove contradictory genres.
Simplify the prompt.
```

Current V6 documentation specifically says reducing Variety to 0 preserves full control of supplied style tags. citehttps://help.suno.com/en/articles/13924481

## Chorus changes too much

```text
Keep lyrics identical.
Keep chorus descriptors identical.
Keep core Style stable.
Avoid unnecessary reference changes.
Use Max Mode when appropriate.
Use surgical editing/stems when exact continuity matters.
```

## Vocal buried

```text
Vocal-forward
clear center image
reduce competing midrange density
restrained instrumentation around key vocal moments
```

## Muddy mix

```text
controlled low end
clean kick-bass separation
uncluttered low mids
clear midrange
restrained reverb
```

## Timing problem in Studio

Use the metronome, solo the relevant track, inspect the timeline, and check whether a generated clip is ahead of/behind the beat. Suno's Studio documentation acknowledges that some timing issues can still occur and recommends rigorous timing checks. citehttps://help.suno.com/en/articles/13670529

---

# 🧠 V6 MASTER WORKFLOW

## PHASE 1 — CONCEPT

```text
What is the song about?
What should the listener feel?
What genre is primary?
What is the vocal identity?
What is the emotional arc?
```

## PHASE 2 — LYRIC ENGINEERING

```text
Hook
Verse 1
Pre
Chorus
Verse 2
Pre
Chorus
Bridge
Final Chorus
Outro
```

## PHASE 3 — STYLE ENGINEERING

```text
Genre
Vocal
Instrumentation
Rhythm
Harmony
Arrangement
Dynamics
Atmosphere
Mix
Master
```

## PHASE 4 — FIRST GENERATION

Use V6 for controlled work or V6-WILD for discovery.

## PHASE 5 — EVALUATION

Score:

```text
Lyrics delivery
Vocal
Melody
Arrangement
Drums
Bass
Emotion
Mix
Artifacts
Overall
```

## PHASE 6 — SURGICAL ITERATION

Change one important variable.

## PHASE 7 — EDIT

Use natural-language editing, Replace Section, Crop, Extend, Add Vocals, or other appropriate tools.

## PHASE 8 — REMASTER / STEMS

Use Remaster for overall sonic refinement and stems when individual elements need work.

## PHASE 9 — STUDIO

Use Studio for:

- detailed arrangement
- MIDI
- synth design
- effects
- automation
- stem editing
- recording
- custom plugins
- final export

## PHASE 10 — FINAL QC

Check:

```text
LYRICS
VOCALS
PITCH
TIMING
ARRANGEMENT
LOW END
MIDRANGE
HIGH END
STEREO
DYNAMICS
CLIPPING
ARTIFACTS
TRANSITIONS
ENDING
METADATA
COMMERCIAL / RIGHTS STATUS
```

---

# 🧪 MASTER V6 CONTROLLED PRESET

Use this as a starting point for systematic testing:

```text
MODEL: V6

GOAL:
[Describe the exact song outcome.]

PRIMARY GENRE:
[One primary identity.]

SUPPORTING INFLUENCES:
[0–2 compatible influences.]

VOCAL:
[Register + texture + delivery + emotion + phrasing.]

INSTRUMENTS:
[Core instruments and roles.]

RHYTHM:
[Groove + drum character + tempo feel.]

ARRANGEMENT:
[Sparse verse → build → chorus → contrast → final payoff.]

DYNAMICS:
[Where energy rises and falls.]

ATMOSPHERE:
[Emotional / environmental character.]

MIX:
[Vocal position + low end + width + transients.]

MASTER:
[Open + controlled + dynamic + polished.]

LYRICS:
[Complete lyrics with clear section structure.]

SLIDERS:
[Record exact values for experiments.]

REFERENCES:
[Document the role of every reference.]

MAX MODE:
[ON/OFF + reason.]
```

---

# 📋 CREATION LOG TEMPLATE

Use this to build your own Suno knowledge base.

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

## Current V6

- [Current Models: V6](https://help.suno.com/en/articles/13924737)
- [V6 FAQ](https://help.suno.com/en/articles/13924481)
- [How to Change Models](https://help.suno.com/en/articles/13924993)
- [Introducing V6](https://suno.com/blog/introducing-v6)
- [V6 Release Notes](https://suno.com/release-notes/introducing-v6)

## Creation

- [Suno Help — Making Music](https://help.suno.com/en/categories/550017)
- [Creative Sliders](https://help.suno.com/en/articles/6141377)
- [Custom Models](https://help.suno.com/en/articles/11362497)
- [Voices](https://help.suno.com/en/articles/11362369)
- [My Taste](https://help.suno.com/en/articles/11362561)
- [Sounds](https://help.suno.com/en/articles/10625537)

## Studio

- [Studio 2.0](https://help.suno.com/en/articles/13670529)
- [Studio 2.0 Help Category](https://help.suno.com/en/categories/2701953-studio-2-0)
- [Studio 2.0 Announcement](https://suno.com/blog/studio-2)

## Stems

- [Advanced Stem Separation](https://suno.com/release-notes/advanced-stems)

## Downloads / Terms

- [Download Limits FAQ](https://help.suno.com/en/articles/13926209)
- [Existing Songs / Download Limits](https://help.suno.com/en/articles/13926593)
- [Downloads, Models & Terms FAQ](https://help.suno.com/en/articles/13614785)
- [Suno Downloads & Terms Announcement](https://suno.com/blog/suno-updates-tos)

---

# 🗓️ CURRENT V6 CHANGELOG / TIMELINE

## July 2026

Suno introduced/expanded major creation and editing capabilities during the V6 rollout period, including improved lyric workflows, structure labels, lyric editing, variations/references, cover-art iteration, and duration controls.

## August 2026

Studio 2.0 launched with:

- MIDI
- wavetable synth
- automation
- effects
- custom plugins
- Studio Chat
- advanced stems
- recording/editing improvements

Voices expanded to iOS and Android.

## September 2026

V6 officially became the current model family:

```text
V6      = controlled flagship
V6-WILD = exploration
V6-MINI = fast access
```

Older models were retired while existing songs remained available.

Download limits began September 3, 2026.

The V6 FAQ and current help center should be treated as the live authority when this guide conflicts with older material.

---

# 🧭 WHAT THIS GUIDE WILL NEVER CLAIM

This guide will **not** claim that:

- a bracket tag is a guaranteed hidden command when it is not documented
- a prompt guarantees a specific melody
- a prompt guarantees an exact BPM unless the relevant tool actually supports it
- a slider has a hidden effect not supported by evidence
- a community trick works 100% of the time
- an old model behaves identically to V6
- a lucky output proves causation
- AI-generated audio is automatically copyrightable in every jurisdiction
- a voice may legally be cloned simply because the software permits a technical workflow
- a third-party tutorial is current merely because it ranks highly in search

Instead, the guide distinguishes:

```text
DOCUMENTED
REPRODUCIBLE
ANECDOTAL
UNKNOWN
```

That distinction is part of the guide's core design.

---

# 🧠 THE FUNDAMENTAL RULES OF SUNO V6

### Rule 1
**Write for the ear, not the checkbox.**

### Rule 2
**One primary musical identity beats ten competing identities.**

### Rule 3
**Concrete audible behavior beats generic adjectives.**

### Rule 4
**Change one major variable when testing.**

### Rule 5
**Listen before rewriting the prompt.**

### Rule 6
**Preserve excellent material. Repair bad material locally.**

### Rule 7
**Use V6-WILD for discovery and V6 for controlled refinement.**

### Rule 8
**Use Max Mode when consistency/fidelity is worth the extra cost.**

### Rule 9
**Use stems and Studio when the problem is production rather than songwriting.**

### Rule 10
**Do not confuse probabilistic generation with deterministic programming.**

### Rule 11
**Document experiments so you learn what actually worked.**

### Rule 12
**When official documentation changes, the guide changes.**

---

# 🏁 FINAL “GOD WORKFLOW”

```text
IDEA
 ↓
DEFINE EMOTION
 ↓
DEFINE PRIMARY GENRE
 ↓
DEFINE VOCAL IDENTITY
 ↓
WRITE / ENGINEER LYRICS
 ↓
BUILD STYLE PROMPT
 ↓
CHOOSE V6 / V6-WILD / V6-MINI
 ↓
SET SLIDERS
 ↓
ADD REFERENCES ONLY WITH CLEAR ROLES
 ↓
USE MAX MODE WHEN JUSTIFIED
 ↓
GENERATE
 ↓
LISTEN
 ↓
SCORE
 ↓
IDENTIFY THE SINGLE BIGGEST FAILURE
 ↓
CHANGE ONE VARIABLE
 ↓
GENERATE AGAIN
 ↓
KEEP THE BEST TAKE
 ↓
SURGICALLY EDIT WEAK SECTIONS
 ↓
EXTEND / CROP / ADD VOCALS AS NEEDED
 ↓
REMASTER IF THE WHOLE SONIC CHARACTER NEEDS REFINEMENT
 ↓
SEPARATE STEMS WHEN INDIVIDUAL ELEMENTS NEED CONTROL
 ↓
OPEN IN STUDIO
 ↓
EDIT AUDIO / MIDI
 ↓
DESIGN SYNTHS
 ↓
ADD EFFECTS
 ↓
AUTOMATE
 ↓
BALANCE
 ↓
QC
 ↓
EXPORT
 ↓
FINAL MASTER
```

---

# 📌 GUIDE STATUS

**Status:** Living / continuously expandable.

**Current reference:** September 13, 2026.

The purpose of this repository is not to create a frozen tutorial. It is to maintain a comprehensive working knowledge base for Suno V6 as the product evolves.

When a new official feature appears, the guide should add:

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
INTERACTIONS WITH OTHER FEATURES
KNOWN FAILURE MODES
OFFICIAL SOURCE
COMMUNITY OBSERVATIONS
TESTING METHOD
```

That is what **“ALL”** and **“EVERYTHING”** mean operationally for this repository: not random information dumped into a README, but every materially useful piece of the current Suno V6 creation and production system organized so it can be found, tested, and updated.

---

## ⚠️ ACCURACY POLICY

Suno is an evolving product. UI labels, feature availability, plan restrictions, credit costs, model behavior, download rules, and supported workflows can change.

**Always verify current official Suno documentation before relying on a time-sensitive claim.**

This guide intentionally separates:

- **Officially documented behavior**
- **Observed/reproducible behavior**
- **Community technique**
- **Speculation / unknown behavior**

No undocumented trick should be treated as a guaranteed feature.

---

<p align="center"><strong>🎵 LIL SYNN's COMPLETE SUNO V6 GUIDE 🎵</strong><br><em>Hear the idea. Engineer the prompt. Generate. Listen. Refine. Produce. Repeat.</em></p>
