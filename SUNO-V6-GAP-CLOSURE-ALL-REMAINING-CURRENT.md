# 🎵 SUNO V6 — GAP CLOSURE / ALL REMAINING CURRENT COVERAGE

> **Part of LIL SYNN's Complete Suno V6 Guide**
>
> Current-reference date: **September 13, 2026**
>
> This document closes the remaining identifiable coverage gaps in the guide. It is deliberately broader than a feature list: it records current controls, workflows, practical production methods, compatibility notes, rights boundaries, evidence levels, testing procedures, and known unknowns.

---

# 1. THE OPERATING DEFINITION OF ALL + EVERYTHING

## ALL

For this guide, **ALL** means every currently documented and materially useful part of the Suno V6 ecosystem that can affect creation, editing, sound design, arrangement, vocals, prompting, personalization, production, export, sharing, rights, troubleshooting, or repeatability.

That includes:

- every current V6-family model;
- every creation mode and major Create-form control;
- lyrics, Style, structure labels, exclusions, vocal direction, and prompt architecture;
- Creative Sliders and audio/reference controls;
- text, audio, image, video, song, playlist, and other supported reference paths;
- Voices, Style Personas, Custom Models, My Taste, Inspire, Sounds and related personalization;
- Sample, Mashup, Cover, Extend, Crop, Reuse Prompt, Adjust Speed and other Remix/Edit workflows;
- natural-language editing and single-lyric editing;
- Add Vocals and instrumental-to-vocal workflows;
- Remaster and stem separation;
- Studio 2.0, MIDI, synth, effects, plugins, automation, recording, take lanes, clip editing, dry extraction and export;
- download formats, download limits, credits and plan restrictions;
- commercial-use and copyright boundaries;
- current mobile/web differences;
- reproducible workflows and controlled testing methods;
- known limitations, deprecated behavior, uncertain behavior and unsupported assumptions.

## EVERYTHING

**EVERYTHING** means ALL of the above **plus the evidence boundary** around each item.

Every claim should be understood as one of:

- **OFFICIAL** — directly documented by Suno.
- **RELEASE NOTE** — explicitly announced in Suno release notes.
- **REPRODUCIBLE** — confirmed through controlled testing.
- **COMMUNITY** — repeatedly reported by users but not guaranteed.
- **EXPERIMENTAL** — behavior appears real but is incomplete, beta, unstable or insufficiently characterized.
- **HISTORICAL** — formerly documented behavior that may no longer apply.
- **UNKNOWN** — insufficient evidence.
- **RETIRED** — no longer a current creation path.

### Non-negotiable rule

Never turn an observed prompt effect into a fictional "secret command." Suno is a generative model, not a deterministic text parser. Prompt syntax can influence probability without functioning like a programming language.

---

# 2. CURRENT V6 MODEL MATRIX

| Model | Purpose | Current availability | Best use |
|---|---|---|---|
| **V6** | Main flagship | Pro / Premier | Controlled final generation |
| **V6-WILD** | Experimental V6 variant | Pro / Premier | Discovery, surprise, unusual arrangements |
| **V6-MINI** | Faster/lighter V6 generation | All users | Rapid iteration and inexpensive exploration |
| **Custom Models** | User-trained model variants | Pro / Premier | Personal sonic identity |

All current V6-family variants support generations up to **8 minutes** in the documented workflow.

### Recommended model loop

```text
V6-MINI
  ↓
fast concept screening
  ↓
V6-WILD
  ↓
discovery / happy accidents
  ↓
V6
  ↓
controlled refinement
  ↓
Remaster / Replace / Stems / Studio
```

Do not assume a V6-WILD result can be regenerated identically in V6. Treat the discovery and reconstruction as separate generations.

---

# 3. V6'S MAJOR NEW CREATIVE PARADIGM: NATURAL-LANGUAGE OPERATIONS

V6 is explicitly designed to understand natural-language musical directions rather than requiring a rigid command syntax.

Examples of operation-level instructions:

```text
Make the second chorus larger without making it louder.

Keep the verse intimate but add rhythmic movement in the percussion.

Replace the chorus vocal texture with a gospel choir while preserving the instrumental identity.

Sample the guitar idea around 0:45 and build a new beat around it.

Take the vocal character from one source and the rhythmic character from another, then create a new song.

Change only this lyric from "love" to "light" and preserve everything else.
```

### Practical rule

Describe:

1. **what should change**;
2. **where it should change**;
3. **what must remain**;
4. **what musical result you want**.

A useful template:

```text
CHANGE: [element]
LOCATION: [section/time]
PRESERVE: [elements that must stay]
TARGET: [desired musical result]
AVOID: [undesired result]
```

This is a high-value V6 prompting pattern because it separates surgical intent from global reinvention.

---

# 4. MULTI-SOURCE / MULTIMODAL CREATION

V6 documentation explicitly describes creation from combinations of:

- text;
- audio;
- images;
- video;
- existing Suno songs;
- playlists / inspiration sources;
- other supported references.

### Multi-source prompt architecture

```text
SOURCE A → [what to borrow]
SOURCE B → [what to borrow]
SOURCE C → [what it should inspire]
NEW MATERIAL → [what Suno should invent]
IDENTITY → [genre / vocal / emotional target]
CONSTRAINTS → [what must not change]
```

### Example

```text
Use the vocal character and emotional intimacy of source A as inspiration, the drum energy of source B, and the visual mood of the supplied image. Build a new dark electropop song with original lyrics and original melodic material. Keep the verses sparse, make the chorus expansive, and avoid copying the exact melody of either source.
```

### Evidence boundary

**OFFICIAL:** V6 supports multimodal inputs and multi-source workflows.

**UNKNOWN:** Exact weighting between every simultaneous input is not publicly specified. Do not claim a fixed priority algorithm unless experimentally demonstrated.

---

# 5. CREATIVE SLIDERS — CONTROL MODEL

Current documented Creative Sliders include:

- **Weirdness:** Safe → Chaos.
- **Style Influence:** Loose → Strong.
- **Audio Influence:** appears when Audio Upload is used.

### Weirdness

Think of Weirdness as an exploration pressure, not a quality control.

```text
LOW
↓
more conventional / predictable
↓
MID
↓
balanced exploration
↓
HIGH
↓
more unusual / unstable / surprising
```

The documented midpoint is 50%.

### Style Influence

Think of Style Influence as adherence pressure:

```text
LOW → style is a softer suggestion
HIGH → style description exerts stronger influence
```

### Audio Influence

Use Audio Influence when the uploaded audio is the structural/sonic anchor and you want to control how strongly the result follows it.

### Testing matrix

For serious testing, hold everything constant and vary only one slider:

```text
A = 0 / low
B = 25%
C = 50%
D = 75%
E = 100% / high
```

Then compare:

- melody adherence;
- arrangement adherence;
- vocal identity;
- rhythmic identity;
- sound design;
- novelty;
- artifacts;
- section consistency.

Do not infer a universal mathematical meaning from the slider percentage. Treat it as a control parameter whose perceptual effect must be characterized experimentally.

---

# 6. VOCAL GENDER

Current Suno documentation says vocal gender can be guided in two ways:

### Simple Mode

Mention the desired voice directly:

```text
1990s alternative rock with female vocals
```

### Custom Mode

Use Advanced Options → Vocal Gender:

- Male
- Female

Then refine the vocal character in Style:

```text
gritty male vocal
soft female vocal
breathy female vocal
raspy male vocal
low intimate male vocal
```

### Important

Vocal Gender is a directional control, not a guarantee of every vocal characteristic. Pair it with timbre, register, delivery and performance language.

---

# 7. VOICES — CURRENT PRACTICAL WORKFLOW

Voices lets a creator use their own voice in Suno-generated songs. Current release notes state that Voices is available on iOS and Android and can be tried on free plans, with additional capabilities on paid plans.

### Input guidance

Official guidance says an acapella recording works best, although recordings containing background music can also be accepted because Suno can isolate the vocal.

### Voice preparation checklist

Prefer:

- clean vocal;
- minimal reverb;
- minimal delay;
- minimal background noise;
- stable microphone distance;
- representative pitch range;
- natural performance rather than an exaggerated character voice.

### Voice consistency test

Create the same short song three ways:

```text
A = default Suno vocal
B = your Voice
C = your Voice + explicit timbre/performance direction
```

Compare identity, intelligibility, emotion and artifacts.

### Compatibility caution

The current model picker warns that Voices, Custom Models and My Taste may have model compatibility considerations. Always verify the current UI rather than relying on an old V5.5 tutorial.

---

# 8. STYLE PERSONAS VS VOICES

Voices replaced Personas as the main Create-menu entry, but Style Personas remain within Voices.

Conceptually:

```text
VOICE = singer identity
STYLE PERSONA = stylistic identity / character of a musical reference
```

Do not treat them as interchangeable controls.

A voice can remain constant while style changes. A style identity can remain similar while the vocal identity changes.

---

# 9. CUSTOM MODELS — DATASET DISCIPLINE

Current documentation allows Pro/Premier users to create up to three private Custom Models using at least six songs they own rights to.

### Better dataset practice

Although Suno does not publish a deterministic recipe for the perfect dataset, a controlled dataset should ideally be:

- stylistically coherent;
- consistently mixed;
- representative of the desired vocal identity;
- representative of the desired arrangement density;
- free of accidental genre outliers;
- legally owned/controlled by the uploader.

### Dataset mistake

Do not train a personal model with:

```text
song 1 = intimate electropop
song 2 = death metal
song 3 = acoustic folk
song 4 = EDM festival
song 5 = piano ballad
song 6 = jazz fusion
```

unless the deliberate goal is precisely that broad identity.

### Better experimental protocol

Build separate Custom Models for clearly different creative identities and compare them using the same test prompt.

---

# 10. MY TASTE / MAGIC WAND

My Taste learns from what the user enjoys on Suno and can personalize style augmentation.

The current documented workflow is:

```text
Create → Styles → Magic Wand
```

With Style Augmentation enabled, the generated style description can reflect the user's listening/creation habits.

### Important testing implication

If two creators enter the same initial style text, My Taste can make the effective generation context different.

Therefore, for controlled A/B testing:

```text
record whether My Taste is ON or OFF
```

Otherwise the experiment may contain an uncontrolled personalization variable.

---

# 11. INSPIRE

Inspire creates a new track from a playlist of the user's music by analyzing characteristics such as mood, tempo and instrumentation and channeling those characteristics into a new composition.

Official guidance recommends short playlists of roughly **3–5 songs** for more control.

### Inspire workflow

```text
Create playlist
  ↓
choose 3–5 representative songs
  ↓
Inspire
  ↓
provide lyrics/style target
  ↓
generate
  ↓
compare against source playlist
```

### Dataset principle

The playlist is effectively a creative reference set. Curate it like a training brief, not like a random folder.

---

# 12. SUNO SOUNDS

Suno Sounds is an experimental feature for generating individual audio material such as:

- sound effects;
- instrument samples;
- ambient sounds;
- other standalone audio material.

Treat Sounds as a **source-material generator**, not automatically as a finished song generator.

### Production workflow

```text
Suno Sounds
→ choose useful sample
→ bring into production context
→ layer / process / automate
→ use as transition, texture, rhythm, or ear candy
```

### Creative uses

- risers;
- impacts;
- one-shots;
- atmospheric beds;
- transitional textures;
- percussive accents;
- sampled instrument ideas;
- environmental sound design.

Experimental features can change; verify current availability before relying on a workflow.

---

# 13. ADD VOCALS

Add Vocals is designed to turn an instrumental into a song by layering a generated vocal based on supplied lyrics.

Current help documentation says it can use:

- an uploaded instrumental;
- a generated instrumental;
- stems from an existing song.

Current documentation also identifies **Audio Strength** as an advanced control that affects adherence to the original instrumental.

### Best-practice workflow

```text
instrumental
  ↓
listen for vocal pocket
  ↓
write lyrics to exact phrasing
  ↓
choose vocal identity
  ↓
set Audio Strength
  ↓
generate multiple takes
  ↓
compare timing + melody + preservation
```

### Key lesson

Do not write lyrics in isolation. Write them for the rhythmic and melodic space of the instrumental.

---

# 14. AUDIO UPLOAD LIMITS

Current help documentation states:

- Free/Basic: uploads up to **60 seconds**;
- Pro/Premier: uploads up to **8 minutes**.

Use uploads as:

- demos;
- melodies;
- instrumentals;
- voice memos;
- sound ideas;
- structural references;
- starting points for Cover/Extend/edit workflows.

Always verify the current accepted format and UI at the moment of use because upload support can evolve.

---

# 15. REUSE PROMPT — RIGHTS-AWARE WORKFLOW

Reuse Prompt copies the creation information associated with a song so the creator can make a new version while changing lyrics, style and title.

### If using another creator's song

Current Suno guidance explicitly warns that if the original song contains lyrics written by another artist, permission is required to reuse those lyrics.

Therefore:

```text
borrow inspiration
≠
copy protected lyrics
```

A safe workflow is:

```text
Reuse Prompt
→ replace lyrics with your own
→ modify title
→ modify style where appropriate
→ verify permissions
→ generate
```

---

# 16. REMIX PERMISSIONS / ATTRIBUTION

Current Suno documentation treats Remix as an umbrella for workflows including Cover, Extend, Reuse Prompt and Adjust Speed.

Creators can control whether their songs are remixable through visibility/permissions settings.

When another creator remixes a song, Suno displays the original version so listeners can access the source.

### Practical rule

Publishing a song and enabling remixing are not the same thing as surrendering ownership.

Always distinguish:

```text
LISTEN PERMISSION
SHARE PERMISSION
REMIX PERMISSION
COMMERCIAL RIGHTS
COPYRIGHT OWNERSHIP
```

These are separate concepts.

---

# 17. COVER VS REMASTER VS REPLACE SECTION

These tools solve different problems.

| Tool | Best purpose |
|---|---|
| **Cover** | Transform an existing song into a substantially different version while retaining a relationship to the source |
| **Remaster** | Make a subtler variation/refinement of the existing result |
| **Replace Section** | Repair/rewrite a selected local section |
| **Extend** | Continue or replace the ending with new material |
| **Crop** | Remove unwanted beginning/end material |
| **Reuse Prompt** | Recreate from the original generation context while allowing edits |

### Decision rule

```text
Bad intro/outro → CROP

Need a new ending → EXTEND

One section is wrong → REPLACE SECTION

Want a subtle refinement → REMASTER

Want a major transformation → COVER

Want to rebuild from the original prompt → REUSE PROMPT
```

---

# 18. REMASTER VARIATION STRATEGY

Current Remaster controls include a model selector and Variation strength:

- **Subtle** — closest to the source;
- **Normal** — default middle ground;
- **High** — more noticeable variation.

### Practical ladder

```text
ORIGINAL
 ↓
SUBTLE
 ↓
NORMAL
 ↓
HIGH
```

Do not jump directly to High when the problem is merely mix clarity. Remaster is not the same thing as rewriting the song.

Use Cover or Replace Section for major creative changes.

---

# 19. ADVANCED STEM SEPARATION

Current Advanced Stem Separation provides three approaches:

### Auto Split

Splits into **12 categories** for fast general separation.

### Split from Mix

Extracts a selected instrument or voice plus a remainder containing everything else.

### Advanced Split

Allows selection from **nearly 100 instruments** and is available to Premier users.

### Rescue workflow

```text
song
 ↓
Get Stems
 ↓
extract problem/valuable element
 ↓
inspect isolation
 ↓
replace / process / remix
 ↓
Studio or external DAW
```

Do not assume separated stems are mathematically perfect. Listen for bleed, transient damage, phase changes and artifacts.

---

# 20. STUDIO 2.0 — FULL PRODUCTION MAP

Studio 2.0 is a browser-based generative DAW available to Premier users.

Core systems include:

- multitrack timeline;
- Chat Bar;
- MIDI;
- Wavetable Synth;
- real-time effects;
- custom plugins;
- automation;
- recording;
- clip editing;
- Take Lanes;
- Remove FX / Get Dry;
- Library dock;
- advanced stems;
- export.

Google Chrome is recommended. Safari currently does not support Web MIDI.

---

# 21. STUDIO CHAT BAR

The Studio Chat Bar is a natural-language interface to the production environment.

Current documentation describes it as capable of tasks including:

- generating audio clips;
- generating MIDI clips;
- designing plugins;
- creating synth presets;
- arranging/editing through chat;
- helping with production tasks.

September 2026 Studio updates added better BPM awareness, including tempo-change processing, improved response reliability, and undo for prompt edits.

### Prompt pattern

```text
TASK
SOURCE
TARGET
CONSTRAINTS
```

Example:

```text
TASK: tighten the bass
SOURCE: current bass track
TARGET: controlled low end with more space for kick
CONSTRAINTS: preserve the existing groove and notes
```

---

# 22. STUDIO MIDI

Studio supports:

- MIDI import;
- MIDI recording;
- MIDI editing;
- piano roll editing;
- musical typing;
- MIDI controllers / Web MIDI;
- generating audio from MIDI;
- using MIDI as a prompt/source for new audio.

### Audio ↔ MIDI concept

Studio can transcribe audio onto a MIDI track and can use MIDI to generate an audio cover.

### MIDI workflow

```text
idea
 ↓
MIDI
 ↓
edit notes / rhythm / structure
 ↓
use MIDI as generative instruction
 ↓
generate audio
 ↓
process in Studio
```

MIDI is therefore both a **production format** and a **generative control surface**.

---

# 23. WAVETABLE SYNTH

Studio's Wavetable Synth can generate:

- basses;
- leads;
- pads;
- chords;
- other synth sounds.

Chat Bar can be used to design presets.

September 2026 updates improved high-frequency fidelity and reduced aliasing.

### Sound-design workflow

```text
choose oscillator concept
→ establish harmonic character
→ filter
→ envelope
→ modulation
→ effects
→ automation
```

Use it to replace weak generated synth layers rather than forcing the original generation to solve every sound-design problem.

---

# 24. STUDIO EFFECTS

Current built-in effects include:

- Compressor;
- EQ;
- Reverb;
- Convolution;
- Delay;
- Distortion;
- Gate.

Compressor supports sidechain operation. Convolution uses sampled acoustic profiles / impulse responses.

Effects can be reordered, bypassed and preset-managed.

### Typical vocal chain

```text
Gate / cleanup
→ EQ
→ Compression
→ De-essing strategy if needed
→ Saturation / Distortion if stylistically appropriate
→ Delay
→ Reverb
```

### Typical mix-bus concept

```text
EQ cleanup
→ gentle compression
→ saturation / color
→ controlled spatial processing
```

Do not apply every effect merely because it exists.

---

# 25. CUSTOM PLUGINS

Studio's Chat Bar can design custom plugins.

Treat custom plugins like experimental DSP prototypes.

Before trusting one in a final mix, compare:

```text
BYPASS
vs
PLUGIN ON
```

Check:

- level matching;
- frequency balance;
- transient preservation;
- stereo image;
- noise/artifacts;
- CPU/performance impact;
- whether the effect actually improves the song.

---

# 26. STUDIO AUTOMATION

Automation changes a parameter over time.

Useful targets include:

- volume;
- effect parameters;
- filter movement;
- sends;
- transitions;
- performance intensity.

### Musical automation principle

Do not automate for movement alone. Automate to support:

- anticipation;
- release;
- section contrast;
- emotional emphasis;
- rhythmic energy;
- spatial movement.

---

# 27. EDITING CLIPS

Studio's Arrangement Editor provides waveform editing for audio and piano-roll editing for MIDI.

Current documentation describes tools around clip arrangement, warping and transitions.

Treat clip editing as the place for precision work after generative selection.

```text
GENERATE
→ SELECT
→ CUT
→ ALIGN
→ TRANSITION
→ AUTOMATE
→ MIX
```

---

# 28. TAKE LANES

Every generation produces two versions. Take Lanes provide a stacked area for managing those takes.

Use them as a built-in comparison system rather than immediately choosing the first result.

### Selection workflow

```text
take A
compare

take B
compare

select best section from each
→ assemble strongest composite
```

This is especially useful when one take has the better verse and another has the better chorus.

---

# 29. RECORDING IN STUDIO

Studio can record:

- audio;
- MIDI.

This allows external performance to become part of the generative production environment.

Useful workflow:

```text
hum melody
→ record
→ edit
→ convert/use as generative source
→ build arrangement
```

Or:

```text
MIDI controller
→ record performance
→ edit timing
→ generate/shape sound
```

---

# 30. REMOVE FX / GET DRY

Remove FX attempts to strip baked-in effects such as reverb and delay from audio.

Use this when:

- the source is too wet;
- you need a drier stem;
- you want to reprocess ambience;
- you need a cleaner source for editing.

Do not assume AI dry extraction restores the mathematically original recording. Inspect artifacts.

---

# 31. STUDIO EXPORT

Studio supports export workflows including full songs, selected ranges, multitrack material and individual stems depending on the current interface/plan.

Current documentation identifies high-quality **32-bit WAV / 48 kHz** Premier Studio export capability, plus MP3 and stem workflows.

### Export strategy

```text
MASTER CHECK
 ↓
full mix export
 ↓
individual stems if needed
 ↓
MIDI if needed
 ↓
external DAW / archive
```

Keep a lossless production master whenever possible.

---

# 32. DOWNLOAD FORMATS + LIMITS

Current download documentation identifies:

- MP3 — available on all plans/web/mobile;
- WAV — Pro/Premier on web;
- mobile downloads default to MP3;
- video downloads where supported;
- stems where available;
- MIDI for Studio songs on eligible plans/workflows.

Current download policy states:

- Free users can have up to 7 lifetime trial downloads under the current policy;
- Pro: 20 downloads/month;
- Premier: 60 downloads/month;
- downloads reset on the billing date;
- unused monthly downloads do not roll over;
- downloading the same song again does not consume another song-download count;
- multiple formats of the same song count as one download;
- stems count as part of that song's download;
- failed/interrupted downloads do not count.

Policy changes are time-sensitive; verify current terms before relying on these limits.

---

# 33. COMMERCIAL RIGHTS VS COPYRIGHT

These concepts must never be collapsed into one statement.

### Commercial-use rights

Current Suno documentation says songs downloaded while subscribed to Pro/Premier are granted commercial-use rights under Suno's terms.

### Copyright

Commercial-use permission does **not** automatically guarantee copyright protection.

Copyright eligibility depends on jurisdiction and the human contribution involved.

### Practical rights stack

```text
Suno contractual commercial permission
        ≠
copyright ownership
        ≠
copyright registration
        ≠
exclusive ownership of every underlying element
```

### Third-party material

If you use someone else's lyrics, recordings, samples, voice, or other protected material, Suno's generation capability does not erase the underlying rights issue.

---

# 34. FREE-PLAN VS PAID-PLAN RIGHTS

Current Suno rights documentation states that free-plan songs are intended for personal/non-commercial use.

Paid subscription commercial rights generally apply to songs made while subscribed under the applicable terms; subscribing later does not automatically create retroactive commercial rights for previously free-plan creations.

Always check the current Terms of Service for a release-critical project.

---

# 35. LYRICIST / LYRIC EDITING

Suno's July 2026 lyrics improvements introduced:

- Lyricist for saving examples of a creator's lyric style/vibe;
- natural-language lyric editing;
- word-level variation/reference workflows;
- full-screen lyric editing;
- structure labels;
- autosave.

### Lyric engineering loop

```text
write
→ inspect rhythm
→ inspect rhyme
→ generate variation
→ choose strongest wording
→ lock structure
→ generate music
```

### Natural-language lyric edit examples

```text
Make this line more conversational.

Keep the meaning but use a tighter internal rhyme.

Make the final word rhyme with "fire" without changing the emotional meaning.

Make this line less literal and more visual.
```

---

# 36. STRUCTURE LABELS — USE THEM AS ARRANGEMENT INTENT

Common labels include:

```text
[Intro]
[Verse]
[Pre-Chorus]
[Chorus]
[Post-Chorus]
[Bridge]
[Breakdown]
[Interlude]
[Instrumental]
[Build]
[Drop]
[Outro]
```

These are best understood as **structural instructions**, not guaranteed hard commands.

Add musical intent when needed:

```text
[Verse — intimate, sparse, low vocal]
[Pre-Chorus — rising tension, drums enter]
[Chorus — wide, explosive, layered harmonies]
[Bridge — stripped, vulnerable, almost spoken]
```

---

# 37. EXCLUSION PROMPTING

Negative directions can be useful but should not become contradictory prompt soup.

### Good

```text
Avoid trap hi-hats, avoid EDM festival drops, avoid overly bright vocals.
```

### Bad

```text
not rock not pop not electronic not acoustic no drums no bass no synth no guitar no melody no chorus
```

A strong positive target usually works better than an enormous negative list.

### Rule

```text
POSITIVE TARGET > EXCESSIVE NEGATION
```

---

# 38. PROMPT DENSITY

There is no current official public hard limit establishing an exact number of "tokens" or instructions that Suno V6 can reliably obey.

Therefore:

**Do not invent a magic prompt-length number.**

Instead test instruction density:

```text
A = 1–3 dominant ideas
B = 4–7 ideas
C = 8–12 ideas
D = highly detailed prompt
```

Evaluate whether adding detail improves or decreases adherence.

The correct amount of detail is task-dependent.

---

# 39. THE HIERARCHY OF MUSICAL INSTRUCTIONS

When a prompt is overloaded, organize it conceptually:

```text
1. SONG IDENTITY
2. VOCAL IDENTITY
3. GENRE / ERA
4. RHYTHM / TEMPO FEEL
5. CORE INSTRUMENTS
6. ARRANGEMENT ARC
7. SECTION CONTRAST
8. MIX / SONIC CHARACTER
9. NEGATIVE CONSTRAINTS
```

Example:

```text
IDENTITY: dark emotional electropop
VOCAL: intimate low male vocal, restrained verses, urgent chorus
RHYTHM: midtempo four-on-the-floor pulse with syncopated percussion
INSTRUMENTS: analog synth bass, glassy pads, muted electric guitar
ARRANGEMENT: sparse verse → rising pre → huge chorus → stripped bridge → final chorus
MIX: wide chorus, controlled sub, crisp transients, warm saturation
AVOID: tropical percussion, comedy tone, EDM festival drop
```

---

# 40. PRODUCTION VOCABULARY → SUNO PROMPT LANGUAGE

| Production concept | Prompt translation |
|---|---|
| Transient | crisp attack, punchy drums |
| Dynamics | restrained verses, explosive chorus |
| Crest factor | punchy, dynamic, not flattened |
| Stereo width | wide chorus, narrow intimate verse |
| Mono compatibility | centered low end, controlled stereo bass |
| Sidechain | subtle kick-driven ducking |
| Saturation | warm analog saturation |
| Harmonics | rich upper harmonics |
| Low-end control | tight sub, controlled bass |
| Depth | intimate foreground, distant ambience |
| Density | sparse / layered / maximal |
| Headroom | open, uncluttered mix |
| Glue | cohesive mix-bus character |
| Air | airy top end |
| Presence | forward vocal |
| Mud | reduce low-mid congestion |
| Harshness | softened upper-mid edge |
| Punch | transient-forward drums |
| Movement | evolving textures / automation |

This vocabulary bridges human production thinking and generative prompting.

---

# 41. VOCAL PERFORMANCE VOCABULARY

Useful dimensions:

### Timbre

```text
breathy
raspy
gritty
silky
nasal
warm
bright
dark
husky
airy
```

### Delivery

```text
intimate
conversational
urgent
restrained
melancholic
defiant
fragile
commanding
whispered
anthemic
```

### Register

```text
low-register
mid-register
high-register
chest-heavy
head-voice leaning
falsetto
```

### Dynamics

```text
near-whisper verse
controlled pre-chorus
full-voice chorus
layered final chorus
```

Avoid stuffing every descriptor into every generation. Choose the few that define the intended performance.

---

# 42. ARRANGEMENT ENGINEERING

Describe arrangement as a trajectory, not merely a list of instruments.

### Weak

```text
synths, bass, drums, guitar, piano
```

### Stronger

```text
Sparse piano and low synth pulse in the verse; percussion gradually enters through the pre-chorus; chorus expands with layered synth chords, full drums and wide guitars; bridge strips back to vocal and atmosphere; final chorus returns with additional harmonies and counter-melody.
```

The second description tells the model **when** and **why** elements appear.

---

# 43. SAME-CHORUS / REPETITION PROBLEM

Repeated sections are not guaranteed to be acoustically identical across generations.

For consistency:

1. Keep lyrics exactly the same.
2. Keep Style identity stable.
3. Avoid unnecessary changes between sections.
4. Use editing workflows rather than regenerating the entire song when possible.
5. Use Take Lanes / Replace Section / Studio when available.
6. Compare multiple takes before selecting the final arrangement.

### Important distinction

```text
same lyrics
≠
same melody
≠
same performance
≠
same mix
```

Do not promise deterministic repetition from text alone.

---

# 44. THE PRODUCTION RESCUE LADDER

When a generation is almost right:

```text
LEVEL 0 — accept it

LEVEL 1 — Crop unwanted edges

LEVEL 2 — Extend a weak ending

LEVEL 3 — Replace the broken section

LEVEL 4 — Remaster for subtle refinement

LEVEL 5 — extract stems

LEVEL 6 — Studio repair / arrangement / effects

LEVEL 7 — external DAW

LEVEL 8 — full re-generation
```

Use the least destructive tool that fixes the problem.

---

# 45. GENERATION FAILURE DIAGNOSTIC

## Problem: wrong genre

Check:

- Style wording;
- reference inputs;
- My Taste;
- model;
- contradictory descriptors.

## Problem: wrong vocal

Check:

- Vocal Gender;
- voice descriptors;
- Voices;
- Style Persona;
- lyrics phrasing;
- model compatibility.

## Problem: chorus too small

Try:

- explicit arrangement growth;
- layered harmonies;
- wider instrumentation;
- stronger performance language;
- section-specific direction.

## Problem: mix too crowded

Try:

- fewer simultaneous instruments;
- sparse verses;
- controlled low mids;
- explicit separation of roles;
- Studio EQ/stems.

## Problem: instrumental changed when only vocals should change

Use a surgical workflow such as Add Vocals or Replace Section rather than recreating the entire song.

---

# 46. A/B TESTING — CONTROLLED SUNO EXPERIMENTS

For reliable conclusions:

```text
CONTROL
↓
change ONE variable
↓
generate multiple samples
↓
blind/listen
↓
score
↓
repeat
```

### Scorecard

| Metric | Score 1–10 |
|---|---:|
| Prompt adherence | |
| Vocal quality | |
| Vocal identity | |
| Melody | |
| Arrangement | |
| Groove | |
| Mix | |
| Emotional impact | |
| Artifact level | |
| Repeatability | |

### Record

- model;
- plan;
- date;
- prompt;
- lyrics;
- slider settings;
- reference inputs;
- My Taste state;
- Voice/Custom Model state;
- result IDs;
- subjective score;
- failure mode.

This turns anecdotal prompting into a reproducible knowledge base.

---

# 47. SCIENTIFIC TESTING OF A SLIDER

Example: testing Style Influence.

Keep fixed:

```text
model = V6
lyrics = identical
style = identical
reference = identical
My Taste = OFF
Voice = OFF
```

Vary only:

```text
Style Influence = low
Style Influence = medium
Style Influence = high
```

Repeat across several seeds/generations and record outcomes.

Never conclude "100% always does X" from one song.

---

# 48. PLAN / FEATURE MATRIX — CURRENT HIGH-LEVEL VIEW

| Capability | Free | Pro | Premier |
|---|---:|---:|---:|
| V6-MINI | ✓ | ✓ | ✓ |
| V6 | — | ✓ | ✓ |
| V6-WILD | — | ✓ | ✓ |
| Voices | ✓/availability varies by current rollout | ✓ | ✓ |
| Custom Models | — | ✓ | ✓ |
| Studio 2.0 | — | — | ✓ |
| Advanced Split | — | — | ✓ |
| Paid-song commercial-use rights | — | ✓ | ✓ |

This is intentionally high-level. Suno changes plan entitlements frequently; the current pricing/help pages should be treated as authoritative for purchase decisions.

---

# 49. MOBILE VS WEB

Current ecosystem differences can include:

- model availability;
- download format defaults;
- Studio availability;
- MIDI/Web MIDI;
- feature rollout timing;
- editing controls;
- social/share surfaces.

### Rule

Never write "Suno supports X" without considering whether the statement means:

```text
WEB
MOBILE
BOTH
STUDIO ONLY
PLAN LIMITED
ROLLOUT LIMITED
```

---

# 50. STUDIO PERFORMANCE / COMPATIBILITY

Current Studio guidance recommends Chrome for best performance and states that Safari does not support Web MIDI.

Studio is intended for desktop/laptop/tablet workflows and requires an adequately sized display; mobile phone use is not the target Studio environment.

If playback or timing behaves unexpectedly:

- use Chrome;
- close unnecessary browser load;
- inspect MIDI timing;
- check metronome;
- solo tracks;
- verify clip alignment;
- export a test before committing to a final workflow.

---

# 51. PLAYLIST / LIBRARY / OFFLINE FEATURES

Current 2026 updates include:

- improved playlist organization;
- playlist filters;
- adding/reordering songs;
- playlist search;
- pinned playlists on web;
- generated/custom playlist cover art;
- offline playlist listening on mobile.

These features matter because a serious production workflow needs asset organization, not just generation.

### Suggested library structure

```text
PROJECT — SONG NAME
├── Original
├── Best Takes
├── Vocals
├── Instrumentals
├── Stems
├── Remasters
├── Covers
├── Final
└── Archive
```

---

# 52. COVER ART / VISUAL WORKFLOW

Current Suno release notes describe web cover-art improvements allowing users to iterate on images with text prompts and create either an image or video.

Visual workflow:

```text
song identity
→ visual concept
→ reference image
→ text iteration
→ image/video
→ evaluate brand consistency
```

Do not treat artwork as an afterthought. The song's sonic identity and visual identity should communicate the same emotional world.

---

# 53. IMESSAGE / CARPLAY / ANDROID AUTO

Current 2026 release notes document:

- iMessage keyboard integration on iOS;
- CarPlay support;
- Android Auto support.

These are distribution/listening surfaces rather than core V6 production controls, but they belong in a complete ecosystem reference.

---

# 54. LEGAL / RIGHTS CHECKLIST FOR UPLOADS

Before uploading material, ask:

```text
Do I own or control this recording?
Do I have permission to use this voice?
Do I have permission to use these lyrics?
Do I have permission to use this sample?
Is this reference merely inspiration, or am I reproducing protected material?
Am I training a Custom Model only on material I have rights to?
Do my intended commercial uses comply with the current Suno terms?
```

Never use a technical feature as evidence of legal permission.

---

# 55. WHAT THE GUIDE MUST NEVER CLAIM

Do not claim any of the following without direct evidence:

- exact hidden model architecture;
- exact token limits;
- exact seed behavior unless exposed and verified;
- deterministic section-tag semantics;
- guaranteed vocal identity from a phrase;
- guaranteed copyright ownership;
- guaranteed identical regeneration;
- guaranteed priority ordering among multimodal inputs;
- secret commands;
- undocumented API behavior;
- future features;
- community folklore as official behavior.

---

# 56. CURRENT UNKNOWN / EXPERIMENTAL REGISTER

The following should remain explicitly marked until Suno publishes more detail or controlled testing establishes reliable behavior:

- exact internal weighting of simultaneous references;
- exact algorithm behind V6-WILD's increased unpredictability;
- exact mathematical mapping of Creative Slider percentages to model behavior;
- exact interaction hierarchy among My Taste, Voices, Style Personas and Custom Models in every combination;
- exact prompt-length thresholds;
- deterministic effects of individual section tags;
- deterministic melody preservation across generations;
- universal guarantees for stem separation quality;
- universal guarantees for dry extraction;
- exact future plan entitlements.

Unknown does not mean useless. It means **do not present an inference as a fact**.

---

# 57. CURRENT V6 MASTER WORKFLOW

```text
01. DEFINE THE SONG
    ↓
02. CHOOSE V6 / V6-WILD / V6-MINI
    ↓
03. WRITE THE MUSICAL IDENTITY
    ↓
04. WRITE / EDIT LYRICS
    ↓
05. DEFINE STRUCTURE
    ↓
06. ADD REFERENCES IF NEEDED
    ↓
07. CONFIGURE VOICE / PERSONA / MODEL IF NEEDED
    ↓
08. SET STYLE + EXCLUSIONS
    ↓
09. SET CREATIVE SLIDERS
    ↓
10. GENERATE MULTIPLE TAKES
    ↓
11. SCORE THE RESULTS
    ↓
12. SELECT THE BEST TAKE
    ↓
13. CROP / EXTEND / REPLACE IF NEEDED
    ↓
14. REMASTER IF THE CHANGE IS SUBTLE
    ↓
15. EXTRACT STEMS IF COMPONENT CONTROL IS NEEDED
    ↓
16. MOVE INTO STUDIO
    ↓
17. EDIT / MIDI / SYNTH / EFFECTS / AUTOMATION
    ↓
18. RECORD OR GENERATE REPLACEMENTS
    ↓
19. CHECK MIX + TRANSITIONS
    ↓
20. EXPORT LOSSLESS MASTER / STEMS / MIDI
    ↓
21. ARCHIVE PROJECT ASSETS
    ↓
22. VERIFY RIGHTS + COMMERCIAL ELIGIBILITY
    ↓
23. DISTRIBUTE
```

---

# 58. THE GOLDEN RULES OF SUNO V6

1. **Use V6 for control.**
2. **Use V6-WILD for discovery.**
3. **Use V6-MINI for fast iteration.**
4. **Describe musical outcomes, not imaginary secret commands.**
5. **Separate song identity from section-level direction.**
6. **Use positive musical language before excessive exclusions.**
7. **Change one major variable at a time when testing.**
8. **Do not regenerate an entire song to fix one broken section.**
9. **Use stems when you need component-level control.**
10. **Use Studio when the problem becomes production rather than generation.**
11. **Use Remaster for subtle refinement, not wholesale rewriting.**
12. **Treat Voices as vocal identity and Style Personas as musical identity.**
13. **Treat My Taste as a personalization variable in controlled experiments.**
14. **Curate Inspire playlists like reference datasets.**
15. **Train Custom Models only on material you have rights to.**
16. **Do not confuse commercial-use rights with copyright protection.**
17. **Do not confuse a working prompt with a guaranteed command.**
18. **Archive the exact prompt, model, settings and source material for important songs.**
19. **Retest old V5/V5.5 techniques under V6.**
20. **Official current documentation outranks memory.**

---

# 59. OFFICIAL SOURCE INDEX — CURRENT REFERENCE SET

Use Suno's current official documentation as the source of truth for changing product behavior.

- Current Models: https://help.suno.com/en/articles/13924737
- V6 FAQ: https://help.suno.com/en/articles/13924481
- What's New in V6: https://help.suno.com/en/articles/13924801
- Model Switching: https://help.suno.com/en/articles/13924993
- Song Length: https://help.suno.com/en/articles/13924929
- Creative Sliders: https://help.suno.com/en/articles/6141377
- Audio Uploads: https://help.suno.com/en/articles/6141569
- Add Vocals: https://help.suno.com/en/articles/6882817
- Voices: https://help.suno.com/en/articles/11362369
- Voices FAQ: https://help.suno.com/en/articles/11362433
- Custom Models: https://help.suno.com/en/articles/11362497
- My Taste: https://help.suno.com/en/articles/11362561
- Inspire: https://help.suno.com/en/articles/6882753
- Reuse Prompt: https://help.suno.com/en/articles/2551041
- Vocal Gender: https://help.suno.com/en/articles/10153473
- Remaster: https://help.suno.com/en/articles/8105281
- Studio 2.0: https://help.suno.com/en/articles/13670529
- Studio Effects / Plugins: https://help.suno.com/en/articles/13670785
- Studio 2.0 category: https://help.suno.com/en/categories/2701953-studio-2-0
- Making Music category: https://help.suno.com/en/categories/550017
- Rights & Ownership: https://help.suno.com/en/categories/550145
- Remix & Attribution: https://help.suno.com/en/categories/1365953
- Release Notes: https://suno.com/release-notes
- V6 Release: https://suno.com/release-notes/introducing-v6
- Studio Updates: https://suno.com/release-notes/studio-updates-sept26

---

# 60. LIVING-GUIDE MAINTENANCE PROTOCOL

Whenever Suno changes materially:

```text
1. Check official release notes.
2. Check current help articles.
3. Compare against this guide.
4. Mark changed behavior.
5. Mark retired behavior.
6. Add new controls/workflows.
7. Retest important claims.
8. Update the current-reference date.
9. Preserve historical notes separately.
10. Never silently overwrite uncertainty with assumptions.
```

### The guide is complete only in the evidence-based sense

A genuinely complete guide is not one that claims omniscience.

It is one that tells the creator:

```text
WHAT EXISTS
WHAT IT DOES
HOW TO USE IT
WHEN TO USE IT
WHAT IT COSTS
WHO CAN USE IT
WHAT IT CONNECTS TO
WHAT CAN GO WRONG
WHAT IS VERIFIED
WHAT IS EXPERIMENTAL
WHAT IS UNKNOWN
WHERE TO VERIFY IT
```

That is the standard this guide should continue to follow.

---

# END — V6 GAP CLOSURE

**LIL SYNN's Complete Suno V6 Guide is a living technical/creative reference, not a frozen tutorial.**

When Suno changes, this document should change with it.