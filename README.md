# 🎵 LIL SYNN's Complete Suno V6 Guide

### The Advanced Suno V6 Creation, Prompting, Editing, Production, Audio Quality, Structure, AI-Assisted Songwriting and Troubleshooting Knowledge Base

<p align="center"><strong>The God Guide to Suno V6</strong><br>Creation • Lyrics • Style • Structure • Tags • Sliders • Advanced Options • Max Mode • References • Voices • Custom Models • Sounds • Sample • Mashup • Editing • Stems • Studio 2.0 • ChatGPT • Troubleshooting</p>

<p align="center"><img src="https://img.shields.io/badge/Suno-V6-black?style=for-the-badge"> <img src="https://img.shields.io/badge/V6--WILD-EXPERIMENTAL-8A2BE2?style=for-the-badge"> <img src="https://img.shields.io/badge/V6--MINI-FAST-00AEEF?style=for-the-badge"> <img src="https://img.shields.io/badge/Studio-2.0-blue?style=for-the-badge"> <img src="https://img.shields.io/badge/ChatGPT-Workflow-74AA9C?style=for-the-badge"> <img src="https://img.shields.io/badge/Status-Living%20Guide-orange?style=for-the-badge"></p>

> **Current-reference date:** September 13, 2026. Suno changes rapidly. Official Suno documentation takes priority over community techniques, old tutorials, screenshots, and remembered behavior.

---

## 🔗 QUICK NAVIGATION

- [About](#-about)
- [V6 Model Family](#-v6-model-family)
- [What V6 Actually Adds](#-what-v6-actually-adds)
- [Advanced / Custom Creation](#-advanced--custom-creation)
- [Lyrics Box](#-lyrics-box)
- [Style Box](#-style-box)
- [Prompt Hierarchy](#-prompt-hierarchy)
- [Structure and Meta Tags](#-structure-and-meta-tags)
- [Creative Sliders](#-creative-sliders)
- [Advanced Options](#-advanced-options)
- [Max Mode](#-max-mode)
- [References and Multimodal Creation](#-references-and-multimodal-creation)
- [Voices](#-voices)
- [Custom Models](#-custom-models)
- [My Taste](#-my-taste)
- [Inspire](#-inspire)
- [Sample and Mashup](#-sample-and-mashup)
- [Suno Sounds](#-suno-sounds)
- [Same Chorus Every Time](#-same-chorus-every-time)
- [Audio Quality](#-audio-quality)
- [Lyrics Engineering](#-lyrics-engineering)
- [ChatGPT Workflow](#-chatgpt-as-your-suno-engineering-assistant)
- [Editing and Reuse Prompt](#-editing-and-reuse-prompt)
- [Remaster](#-remaster)
- [Stems](#-stems)
- [Studio 2.0](#-suno-studio-20)
- [Production Language](#-production-language)
- [Community Issues and Fixes](#-community-issues-and-fixes)
- [Scientific Testing](#-scientific-suno-testing)
- [Master Workflow](#-the-complete-v6-god-workflow)
- [Troubleshooting Decision Tree](#-troubleshooting-decision-tree)
- [Official Resources](#-official-suno-resources)
- [Accuracy Policy](#-accuracy-policy)

---

## 🎯 ABOUT

This is a living technical guide to Suno V6 for creators who want advanced control rather than a basic text-to-song tutorial.

It treats Suno as a **generative music production system**, not a deterministic programming language. The guide covers model selection, Custom creation, Lyrics and Style engineering, structure tags, Creative Sliders, Advanced Options, Max Mode, references, vocals, arrangement, production prompting, lyric engineering, AI-assisted songwriting, editing, stems, Remaster, Sounds, Sample, Mashup, Studio 2.0, repeatability, troubleshooting and systematic experimentation.

Suno's official V6 material describes V6 as its flagship model with stronger control and precision. The V6 family also introduces a more experimental `v6-wild` and a faster `v6-mini`. V6 supports text, audio, images and video in supported workflows and adds natural-language editing, mashups, sampling and more. citehttps://suno.com/release-notes/introducing-v6

**Evidence hierarchy used by this guide:**

1. **Official Suno documentation** — highest confidence.
2. **Direct reproducible experiments** — useful when clearly documented as observations.
3. **Community / Reddit reports** — useful for finding failure modes and experiments, but anecdotal.

A community technique may be extremely useful without being an official Suno feature. Nothing here should be interpreted as a hidden API, secret switch, guaranteed parser, deterministic command or promise of identical output unless Suno explicitly documents it.

---

# 🧬 V6 MODEL FAMILY

Suno currently documents three V6 family models:

| Model | Best use | Character | Availability |
|---|---|---|---|
| **v6** | Final controlled creation | Expressive, precise, polished | Pro / Premier |
| **v6-wild** | Discovery and experimentation | More varied, surprising, unconventional | Pro / Premier |
| **v6-mini** | Fast iteration | Lighter and faster | All users |

All three support up to **8 minutes per generation**. citehttps://help.suno.com/en/articles/13924801

```text
V6       = CONTROL + PRECISION + POLISH
V6-WILD  = EXPLORATION + SURPRISE + VARIATION
V6-MINI  = SPEED + TESTING + ITERATION
```

### V6

Use when you know what you want and need the strongest adherence to the creative brief.

### V6-WILD

Use when the goal is discovery rather than obedience. It is not a "higher quality" mode. It is deliberately less predictable and can produce unexpected arrangements, textures and genre combinations. Strong ideas discovered here can be brought back into controlled V6 work. citehttps://help.suno.com/en/articles/13924737

### V6-MINI

Use for quick concepts, rapid iteration, prompt testing and high-volume experimentation before spending more time on a final V6 generation.

### Model selection

The model picker is in the upper-right area of the Create form. Your selection remains active until changed. Suno also lists Custom Models in the model picker for eligible users. citehttps://help.suno.com/en/articles/13924993

---

# 🚀 WHAT V6 ACTUALLY ADDS

Suno's September 2026 V6 release notes describe several important capabilities that should be treated as first-class parts of the V6 workflow:

### 1. Natural-language section editing

You can describe a desired change to part of an existing song without necessarily rebuilding everything.

Example:

```text
Change the chorus so it is performed by a gospel choir while preserving the existing song identity and surrounding arrangement.
```

### 2. Multi-source mashups

V6 can combine elements from multiple sources in a single workflow.

Example:

```text
Take the vocal character from Source A, the drums from Source B, and build a new 80s synthwave arrangement around them.
```

### 3. Sampling and isolation

V6 workflows can use a selected musical moment as a starting point, including sampling a riff or isolating an instrument before building a new context around it.

### 4. Vibe-based creation

V6 can use an abstract description of a feeling or environment as the starting point.

```text
Make a song that feels like midnight on a rooftop after a breakup: lonely, neon-lit, intimate verses, huge but bittersweet chorus.
```

### 5. Multimodal creation

Supported V6 workflows can use text, audio, images and video as creative inputs.

### 6. Single-lyric edits

V6 can update an individual lyric without requiring the entire song to be rebuilt in supported editing workflows.

These capabilities are part of the documented V6 feature set, not merely community prompting tricks. citehttps://suno.com/release-notes/introducing-v6

---

# 🧠 ADVANCED / CUSTOM CREATION

Custom creation is where controlled prompting becomes most useful.

Think of the creation system as layers:

```text
MODEL
  ↓
STYLE / SONG IDENTITY
  ↓
LYRICS / SONG CONTENT
  ↓
SECTION-SPECIFIC PERFORMANCE CUES
  ↓
ADVANCED OPTIONS
  ↓
SLIDERS
  ↓
REFERENCES / AUDIO / IMAGE / VIDEO
  ↓
GENERATION
  ↓
SURGICAL EDITING
  ↓
STEMS / STUDIO / DAW
```

### Variable isolation

Do not change ten variables and then declare that the song improved.

If the vocal is right but drums are wrong, change the drum-related instruction.

If the chorus is excellent but the bridge is bad, preserve the chorus and repair the bridge.

If the arrangement is right but the mix is muddy, use production language, Remaster, stems or Studio rather than destroying the entire generation.

---

# ✍️ LYRICS BOX

The Lyrics Box is more than a place to paste words. In current Suno workflows it can contain lyrics, section labels and localized performance/arrangement direction. Suno's 2026 web lyrics improvements also added a more full-featured writing environment, Lyricist, natural-language editing, variations/references and structure labels. citehttps://suno.com/release-notes

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
[Intro | 8 bars | atmospheric synth swell | filtered drums | instrumental]

[Verse 1 | intimate lead vocal | sparse drums | low register | restrained delivery]

[Pre-Chorus | rising tension | bass opens | additional percussion | increasing vocal intensity]

[Chorus | full drums | wide synths | stacked harmonies | strong melodic hook | vocal forward]

[Verse 2 | pull back density | intimate vocal | new counter-melody]

[Pre-Chorus | larger build | rising harmony | controlled anticipation]

[Chorus | same core chorus melody and lyrics | full arrangement | stacked harmonies]

[Bridge | contrasting harmony | reduced drums | exposed vocal | emotional reset]

[Final Chorus | same core chorus identity | expanded harmonies | controlled lift | strong ending]

[Outro | instrumental release | final vocal phrase | clean ending]
```

This is **guidance**, not a programming language. Suno may interpret, ignore, reinterpret or occasionally sing descriptive text. Keep experimental syntax clearly labeled as experimental.

## One section, one job

Do not put a giant production manual into every lyric section.

Good:

```text
[Verse 1 | intimate lead | sparse drums | restrained delivery]
```

Bad:

```text
[Verse 1 | intimate lead | sparse drums | 117 BPM | exact EQ curve | compressor settings | huge cinematic stereo field | no distortion | no reverb | vocal centered at -1.2 dB | ...]
```

The second approach creates unnecessary instruction density and can compete with the actual lyric content.

---

# 🎨 STYLE BOX

The Style Box is the **song-wide musical identity layer**.

A useful hierarchy:

```text
PRIMARY GENRE
SECONDARY INFLUENCE
ERA / PRODUCTION FAMILY
VOCAL CHARACTER
CORE INSTRUMENTS
RHYTHM
ARRANGEMENT
DYNAMICS
ATMOSPHERE
MIX CHARACTER
MASTER CHARACTER
```

## Strong Style template

```text
Primary identity: [genre + subgenre + era/production family].
Vocal: [register + texture + delivery + emotional behavior].
Core instruments: [3–7 important instruments].
Rhythm: [groove + drum character + tempo feel].
Harmony: [major/minor/modal character if important].
Arrangement: [section arc and density progression].
Dynamics: [where the track grows, contracts, peaks and resolves].
Atmosphere: [emotional/environmental character].
Mix: [vocal position + width + low-end behavior + transient behavior].
Master: [open + controlled + dynamic + polished].
```

## Example: dark emotional electropop

```text
Dark emotional electropop with cinematic synth-pop influence, intimate expressive male lead vocal, warm analog polysynths, controlled sub bass, tight punchy electronic drums, sparse verses, rising pre-choruses, huge melodic choruses, layered vocal harmonies, wide stereo synth textures, strong dynamic contrast, vocal-forward center image, clean low end, defined kick and bass separation, restrained reverb, smooth open high end, preserved transient punch, polished modern commercial production without excessive loudness distortion.
```

## Example: intimate indie pop

```text
Intimate nocturnal indie pop, restrained emotional male vocal, close-mic presence, dry detailed vocal, warm electric piano, soft analog synth pads, round bass, understated electronic percussion, sparse arrangement, subtle stereo movement, gentle dynamic growth, natural human phrasing, controlled low end, clear midrange, minimal reverb, open smooth high end, emotionally vulnerable rather than theatrical.
```

## Example: aggressive electronic pop

```text
Dark high-energy electropop fused with modern electro house, tight four-on-the-floor kick, controlled sub bass, bright analog synth sequence, sharp transient percussion, selective distortion textures, dramatic pre-chorus tension, explosive but controlled chorus impact, wide stereo synth field, centered lead vocal, stacked harmonies, clean kick-bass separation, punchy drums, polished club mix, controlled high-end energy, strong dynamic contrast.
```

## Example: cinematic ballad

```text
Cinematic alternative pop ballad, intimate low-register male vocal, piano-led foundation, soft strings, distant atmospheric synths, subtle sub bass, restrained percussion entering gradually, sparse verse arrangement, emotionally rising pre-chorus, expansive chorus without excessive loudness, layered vocal harmonies, natural room ambience, vocal-forward center image, wide uncluttered stereo field, warm controlled low mids, smooth high end, preserved dynamics.
```

## Avoid prompt soup

Avoid:

```text
pop rock EDM hip hop R&B metal jazz cinematic orchestral hyperpop trap house techno folk
```

That gives the model too many competing destinations.

Prefer:

```text
PRIMARY GENRE + 1–2 SUPPORTING INFLUENCES + SPECIFIC MUSICAL ROLES
```

Concrete audible behavior beats generic praise words.

Replace:

```text
beautiful
amazing
professional
cinematic
high quality
```

with:

```text
vocal-forward
controlled low end
sparse verse
wide chorus
defined transients
restrained reverb
dry close vocal
preserved dynamic contrast
kick-bass separation
```

---

# 🧱 PROMPT HIERARCHY

When a Style prompt gets long, preserve the highest-value information first.

```text
1. PRIMARY GENRE
2. VOCAL IDENTITY
3. CORE INSTRUMENTS
4. RHYTHM
5. ARRANGEMENT
6. DYNAMICS
7. ATMOSPHERE
8. MIX CHARACTER
9. MASTER CHARACTER
```

If you need to shorten a prompt, remove redundancy before removing identity.

```text
sad + heartbreaking + melancholic + somber + emotionally devastating
```

can often become:

```text
dark melancholic emotional
```

---

# 🏷️ STRUCTURE AND META TAGS

Community users commonly experiment with:

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

### Vocal vocabulary

```text
[Male Vocal]
[Female Vocal]
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

### Instrument vocabulary

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

### Dynamics

```text
[Soft]
[Quiet]
[Restrained]
[Build]
[Rising]
[Full]
[Explosive]
[Breakdown]
[Strip Back]
[Final Lift]
```

### Performance

```text
[Intimate Vocal]
[Powerful Vocal]
[Breathy Vocal]
[Dry Vocal]
[Emotional Delivery]
[Controlled Delivery]
[Legato]
[Staccato]
[Melismatic]
[Harmonized]
[Octave Harmony]
```

**Important:** these are not a complete official Suno programming language. Basic structural labels are safer than exotic invented commands.

### Safe custom-tag principle

Use normal musical language:

```text
[Verse | intimate low-register vocal | sparse drums | warm bass]
```

Do not assume Suno has a hidden parser for invented pseudo-code such as:

```text
[VOCAL_LOCK: TRUE](MAX)
```

Community pseudo-code, XML-like tags, weighting syntax and elaborate control languages are experiments unless Suno documents them.

---

# 🎛️ CREATIVE SLIDERS

Suno's Creative Sliders include **Weirdness**, **Style Influence**, and **Audio Influence** when audio is used. V6 also introduces **Variety**, which can update style prompting. Suno specifically says that reducing Variety to `0` preserves full control over supplied style tags. citehttps://help.suno.com/en/articles/13924481

These are behavioral controls, not quality scores.

## Variety

Variety controls how much Suno varies its outputs and updates the style prompting.

For controlled A/B testing:

```text
VARIETY = 0%
```

For exploration, increase deliberately.

Do not assume 0% is universally best. It is best understood as a **control-oriented starting point**.

## Weirdness

Weirdness moves the generation from safer interpretation toward more unusual output. Suno describes 50% as the normal expected result in its slider documentation.

Practical experimental ranges:

```text
20–40% = controlled
~50%   = balanced
60%+   = deliberate experimentation
```

These are recommendations, not official presets.

## Style Influence

Style Influence controls how closely the generation follows the Style input.

A practical starting range for strict Style adherence:

```text
80–95%
```

Maximum influence cannot repair a badly written Style Box. It can simply make Suno follow the bad prompt more strongly.

## Audio Influence

Audio Influence controls how strongly a generation relates to supplied audio.

Preservation-oriented testing:

```text
85–100%
```

Transformation-oriented testing:

```text
start lower and increase only as needed
```

Do not automatically assume 100% is ideal.

## Personalization

Personalization can incorporate your broader musical taste. It is useful for normal creation but can introduce another variable during controlled A/B testing.

For scientific prompt tests:

```text
PERSONALIZATION = OFF
```

---

# ⚙️ ADVANCED OPTIONS

## Vocal Gender

Suno documents Vocal Gender in Advanced Options for Custom Mode. Use the dedicated control when available and then describe vocal character in Style.

Do not rely exclusively on a lyric tag like `[Male Vocal]` if the interface provides an actual vocal-gender control.

## Exclude

Exclude is designed to tell Suno what you do **not** want.

Example:

```text
STYLE:
minimal electronic pop with piano, warm synth pad, controlled bass and tight electronic drums.

EXCLUDE:
banjo, ukulele, acoustic guitar, brass section, orchestral choir, trap hi hats, distorted guitar
```

Use Exclude to remove persistent unwanted elements, while using positive Style language to describe the desired replacement.

## Advanced Options philosophy

Treat each option as a variable.

Do not simultaneously change:

```text
Model
Style
Lyrics
Variety
Weirdness
Style Influence
Audio Influence
Exclude
Max Mode
```

and then attempt to diagnose the result.

---

# 🚀 MAX MODE

Suno describes Max Mode as giving V6 more resources and costing more credits. Suno specifically recommends it for:

- songs longer than two minutes
- covers where staying close to the original matters
- transferring style from one song to another
- maintaining vocal/style consistency through a track

For quick ideas and short songs, standard mode is sufficient. citehttps://help.suno.com/en/articles/13924481

### Practical controlled starting profile

```text
MODEL: V6
VARIETY: 0%
WEIRDNESS: 30–40%
STYLE INFLUENCE: 85–95%
AUDIO INFLUENCE: 90–100% when preservation matters
PERSONALIZATION: OFF during experiments
MAX MODE: ON for important long or consistency-sensitive generations
```

These are **starting points**, not Suno presets.

---

# 🖼️ REFERENCES AND MULTIMODAL CREATION

V6 supports creation using text, audio, images and video in supported workflows. citehttps://suno.com/release-notes/introducing-v6

Give every reference a job.

| Input | Best conceptual use |
|---|---|
| Text | Concept, story, mood, musical intent |
| Audio | Musical material, performance, sonic reference |
| Image | Mood, atmosphere, visual inspiration |
| Video | Visual/motion context where supported |
| Existing Suno song | Musical source for edit/remix/sample workflows |

### Image prompting

Do not merely ask Suno to describe an image.

Better:

```text
Use the image as a visual mood reference only. Translate its nocturnal lighting, isolation, muted colors and cinematic tension into a dark emotional electropop arrangement. Do not turn the visual description into literal lyrics. Preserve an intimate human vocal and build toward a large melodic chorus.
```

### Reference discipline

Do not throw every possible input into one generation simply because the interface permits it.

Each reference should answer:

```text
WHAT should Suno borrow?
WHAT should Suno ignore?
WHY is this reference here?
```

---

# 🎤 VOICES

Suno's Voices system lets creators add their own voice to Suno-generated songs. Suno's documentation says a clean acapella recording works best, although recordings with background music can also be accepted because Suno can isolate the vocal. citehttps://help.suno.com/en/articles/11362369

Voices replaced the old Personas button in Create, while Style Personas remain available within Voices. citehttps://help.suno.com/en/articles/11362433

### Voice-quality principles

```text
clean source
minimal background noise
consistent vocal performance
clear pitch information
avoid heavy reverb
avoid extreme distortion
```

### Important model note

Suno's current Voices documentation was originally tied to v5.5. Do not assume every Voice capability automatically applies to every V6 workflow. Always check the current model compatibility shown by Suno.

---

# 🧬 CUSTOM MODELS

Custom Models let eligible Pro and Premier users build personalized models from their own music.

Current documentation states:

- up to **3** Custom Models
- at least **6 songs** required
- Bulk Upload is available
- you must own the rights to the uploaded songs
- models are private and cannot be shared
- model creation takes roughly **2–5 minutes** after the required tracks are supplied

citehttps://help.suno.com/en/articles/11362497

### Custom Model strategy

Do not feed a Custom Model random tracks simply because they are available.

Build the training set around the identity you actually want:

```text
same artistic identity
same production philosophy
same vocal aesthetic
same genre neighborhood
consistent quality
minimal unrelated experiments
```

A Custom Model is not a replacement for good prompting. It is another layer of identity conditioning.

---

# 🧠 MY TASTE

My Taste is available to all users and learns from what you enjoy on Suno, including genres and moods. The Style Magic Wand can use that information to create personalized Style descriptions. citehttps://help.suno.com/en/articles/11362561

### My Taste is useful when

- you want faster personalized ideation
- you like Suno to incorporate your broader preferences
- you are brainstorming rather than scientifically testing prompts

### My Taste is less useful when

- running controlled A/B tests
- trying to measure the effect of one prompt change
- trying to reproduce a result without personalization variables

For controlled testing:

```text
PERSONALIZATION = OFF
```

---

# 💡 INSPIRE

Inspire can use a playlist of your songs as a source of creative direction. Suno recommends relatively short playlists, roughly three to five songs, when you want more control.

Use Inspire to communicate **your musical neighborhood**, not to create an indiscriminate pile of references.

---

# 🧪 SAMPLE AND MASHUP

Suno's Sample and Mashup features were introduced in January 2026.

**Mashup** combines two songs into a new result.

**Sample** lets you select a section of sound as the starting point for a new idea.

Suno's release notes describe workflows such as taking a snippet from a song, a melody from a voice memo, or another musical fragment and using it as a starting point. citehttps://suno.com/release-notes/meet-our-new-create-features-sample-mashup

### Sample workflow

```text
FIND BEST MUSICAL MOMENT
↓
SELECT SAMPLE REGION
↓
IDENTIFY WHAT MUST SURVIVE
↓
DESCRIBE NEW MUSICAL CONTEXT
↓
GENERATE
↓
COMPARE
↓
EDIT / ASSEMBLE
```

### Mashup workflow

```text
SOURCE A = element you love
SOURCE B = element you love
↓
DEFINE THE JOB OF EACH SOURCE
↓
DESCRIBE THE NEW MUSICAL IDENTITY
↓
MASHUP
↓
SURGICALLY EDIT BAD SECTIONS
```

---

# 🔊 SUNO SOUNDS

Suno Sounds is an experimental/beta feature for generating individual audio material such as sound effects, instrument samples, ambient sounds and loops. It is available from Create through **Sounds**. citehttps://help.suno.com/en/articles/10625537

Supported concepts include:

```text
ONE SHOT = a single short sound
LOOP     = a repeating musical/audio clip
```

For loops, BPM can be specified.

### Useful prompts

```text
Dark cinematic riser, metallic texture, 8 seconds, tension increasing smoothly, no percussion.
```

```text
Warm analog synth bass loop, 110 BPM, minor key, deep but controlled sub, clean transient attack.
```

```text
Short cinematic impact, low-frequency hit with restrained metallic tail, no melody, clean ending.
```

Sounds is especially useful for Studio and DAW workflows where you need individual building blocks rather than another complete song.

---

# 🎵 SAME CHORUS EVERY TIME

There is no documented V6 switch that guarantees an identical chorus melody, vocal performance, harmony and production every time.

Generative music is not a fixed sequencer.

The strongest approach is:

1. Use identical chorus lyrics.
2. Use consistent section labels.
3. Explicitly describe the chorus as the recurring hook.
4. Reduce unnecessary variation.
5. Preserve the best generated chorus through editing rather than repeatedly rebuilding the whole song.

Example:

```text
The chorus is the primary recurring hook. Every chorus should preserve the same core melody, vocal phrasing, harmonic movement, rhythmic hook and arrangement identity. Do not invent a new chorus melody for later repetitions. Keep the emotional delivery consistent unless the lyrics explicitly request a controlled final lift.
```

If exact sample-identical repetition is required, use Studio or a DAW to duplicate the successful audio region.

---

# 🔥 AUDIO QUALITY

A better model does not guarantee a professional mix.

Many perceived quality problems are arrangement problems:

- too many layers
- excessive low-mid energy
- constant maximum density
- competing vocals
- competing instruments
- excessive effects
- uncontrolled dynamics
- weak section contrast

Use production language that describes audible behavior.

```text
vocal-forward center image
clean controlled low end
defined kick and bass separation
punchy transients
restrained reverb
wide stereo ambience
clear vocal articulation
smooth open high end
preserved dynamic contrast
polished commercial production without excessive loudness distortion
```

### Distant vocal

```text
close-mic lead vocal, vocal-forward center image, clear diction, restrained room ambience, dry intimate verses, present vocal articulation, backing vocals behind the lead.
```

### Muddy mix

```text
clean low-mid separation, controlled sub bass, defined kick transient, clear bass fundamental, uncluttered midrange, wide supporting instruments without masking the vocal, restrained ambience.
```

### Flat arrangement

```text
sparse verse, gradual pre-chorus lift, increased harmonic density before the chorus, wider chorus instrumentation, bridge reduction, final chorus expansion, strong dynamic contrast without excessive loudness.
```

### Overproduced arrangement

```text
minimal supporting layers, intentional negative space, uncluttered midrange, restrained effects, no constant wall of sound, lead vocal remains the focal point, dynamics driven by arrangement rather than excessive compression.
```

---

# 📝 LYRICS ENGINEERING

A lyric can be technically polished and still fail as a song.

Evaluate:

```text
CONCEPT
ORIGINALITY
EMOTIONAL TRUTH
IMAGERY
HOOK STRENGTH
SINGABILITY
SYLLABLE DENSITY
RHYME QUALITY
NARRATIVE PROGRESSION
MEMORABILITY
```

## Avoid AI-writing fingerprints

Watch for:

- generic heartbreak language
- predictable rhyme pairs
- repeated emotional conclusions
- vague metaphors
- filler written only to satisfy rhyme
- excessive symmetry
- fake specificity
- phrases that could belong to thousands of songs

### Surgical rewrite method

Do not automatically rewrite an entire song.

```text
Identify weak line.
↓
Explain why it fails.
↓
Preserve rhyme family and syllable feel.
↓
Generate 5 replacements.
↓
Choose the strongest.
↓
Reinsert into original song.
```

---

# 🤖 CHATGPT AS YOUR SUNO ENGINEERING ASSISTANT

ChatGPT is most useful when treated as a collaborator, critic, arranger and prompt engineer rather than a lyric vending machine.

## The 10/10 loop

```text
DRAFT
↓
RATE IT OUT OF 10
↓
IDENTIFY EVERYTHING PREVENTING 10/10
↓
FIX ONLY THOSE PROBLEMS
↓
RE-RATE
↓
REPEAT
↓
FINAL HUMAN REVIEW
```

### Master ChatGPT prompt

```text
You are my professional songwriter, record producer, vocal producer, arranger and Suno V6 prompt engineer.

I will give you a song idea, lyric fragments or an existing draft.

Your job is to help me develop it into a professional song without erasing its identity.

FIRST: Understand the story, narrator, emotional conflict, setting and intended listener reaction.

SECOND: Ask important questions if information is missing.

THIRD: Build the song structure and explain the emotional job of each section.

FOURTH: Write or improve lyrics while preserving distinctive phrases and avoiding generic AI songwriting.

FIFTH: Create conventional Suno structure tags with concise section-specific instructions.

SIXTH: Create a separate Suno V6 Style Box describing genre hierarchy, vocal character, instrumentation, rhythm, arrangement, dynamics, atmosphere and mix direction.

SEVENTH: Recommend Advanced Options including Vocal Gender, Exclude, Variety, Weirdness, Style Influence, Audio Influence and Max Mode when relevant.

EIGHTH: Rate lyrics, structure and Style out of 10.

NINTH: Explain exactly what prevents anything from being a 10/10.

TENTH: Revise only the weak areas.

ELEVENTH: Rate again.

Do not give me a fake 10/10 just to be agreeable.
Do not use generic filler.
Do not overload the Lyrics Box with unnecessary production instructions.
Do not treat community tricks as guaranteed commands.
Do not contradict the lyric's emotional intention.
Do not rewrite distinctive lines unless there is a clear reason.
```

## Ask ChatGPT to interview you first

```text
Before writing anything, interview me about the story, narrator, relationship, emotional arc, setting, point of view, genre, vocal identity, intended audience, chorus idea, title, words I refuse to use, lyrical themes I want to avoid and the emotional reaction I want from the listener. Ask one or two questions at a time and use my answers to build the song.
```

## A/B testing

```text
Create Version A with a restrained chorus and Version B with a larger chorus.
Keep lyrics identical.
Keep genre identical.
Change only arrangement and vocal dynamics.
Explain exactly what changed.
Tell me which version better communicates the lyric's emotional idea and why.
```

## Troubleshooting prompt

```text
Suno V6 problem:
The verse sounds excellent.
The first chorus is excellent.
The second chorus becomes too loud and changes melody.
The final chorus becomes shouted and adds unwanted ad-libs.

Do not rewrite the whole song.
Diagnose likely causes.
Separate high-confidence advice from experimental community techniques.
Give me one change at a time to test.
Provide exact Style Box and Lyrics Box replacements for the affected section only.
```

---

# ✂️ EDITING AND REUSE PROMPT

Do not think of generation as the only workflow.

Suno provides editing workflows including Replace Section, Extend and Reuse Prompt.

### Replace Section

Use when most of the song is correct and one area is wrong.

```text
GOOD SONG
+ BAD SECTION
= REPLACE ONLY THE BAD SECTION
```

This is especially powerful for chorus consistency, unwanted ad-libs, wrong instrumentation and weak bridges.

### Extend

Use Extend when continuing a song beyond its existing ending. Make the desired destination clear and avoid unnecessarily repeating huge amounts of instruction.

### Reuse Prompt

Reuse Prompt can take an existing song's creation details and let you modify Lyrics, Style and Title to create a new version. citehttps://help.suno.com/en/articles/2417409

### Surgical editing principle

```text
If 90% is right, do NOT destroy the 90% to repair the 10%.
```

---

# 🎚️ REMASTER

Remaster is intended for subtle sonic refinement while retaining the song's identity. Current Suno documentation describes model selection and Variation strength, with variation controls ranging from close-to-original refinement to more noticeable change. citehttps://help.suno.com/en/articles/8105281

Use Remaster when:

- structure is right
- lyrics are right
- performance is right
- the sonic presentation needs refinement

Do not use Remaster to fix a fundamentally bad composition.

If the chorus melody is wrong, a better mix does not make the melody correct.

---

# 🧩 STEMS

Suno's updated Stem Separation provides three approaches:

### Auto Split

Classic automatic separation into **12 stem categories**.

### Split from Mix

Extract a selected instrument or voice into one stem while producing everything else as the other stem.

### Advanced Split

Choose what to extract from a list of nearly **100 instruments**. Current release notes identify Advanced Split as a Premier feature. citehttps://suno.com/release-notes/advanced-stems

### Stem repair workflow

```text
PERFECT VOCAL
+ BAD GUITAR
↓
SEPARATE STEMS
↓
KEEP VOCAL
↓
REPLACE / REPAIR GUITAR
↓
REASSEMBLE
```

Stems are a major reason not to regenerate an entire song when only one component is wrong.

---

# 🎛️ SUNO STUDIO 2.0

Studio 2.0 turns Suno Studio into a much deeper production environment. Suno documents:

- MIDI
- piano roll editing
- musical typing
- external MIDI input
- wavetable synthesis
- audio effects
- custom plugins generated through chat
- automation
- stem separation
- recording
- take lanes / alternates
- tempo and time-signature controls
- chat-based production operations

Studio 2.0 is available to Premier users. Suno recommends Google Chrome for best performance; Web MIDI is not currently supported by Safari. Mobile devices are not supported for Studio. citehttps://help.suno.com/en/articles/13670529

## Studio Chat

Studio's Chat Bar is a natural-language production interface.

Examples:

```text
Make the drums punchier.
```

```text
Add a moody synth pad under the chorus.
```

```text
Give me three alternate takes of this section.
```

Studio Chat can see the project and selected context and can perform supported operations conversationally. citehttps://help.suno.com/en/articles/13670721

## MIDI

Studio 2.0 MIDI tracks hold notes instead of recorded audio. The notes drive the instrument loaded on the track.

Features include:

```text
piano roll
quantize
velocity editing
pitch bend
modulation
musical typing
chord modes
arpeggiator
external MIDI controllers
```

citehttps://help.suno.com/en/articles/13670593

## Wavetable synth

The Wavetable synth can produce basses, leads, pads, plucks and evolving textures. It can be controlled manually or prompted through Studio Chat.

Example:

```text
Create a glassy synth pad that slowly evolves into a soft wobble, with a warm stereo image and restrained high-frequency movement.
```

Suno also documents the ability to capture a wavetable from timeline audio or upload your own wavetables. citehttps://help.suno.com/en/articles/13670657

## Audio effects

Studio 2.0 includes effects such as:

```text
Compressor
EQ
Reverb
Convolution
Delay
Distortion
Gate
```

It supports sidechain compression and real-time processing. Studio does **not** support conventional VST or Audio Units plugins. citehttps://help.suno.com/en/articles/13670785

## Automation

Automation can control track volume, pan and plugin/effect parameters over time.

Example uses:

```text
volume swell into chorus
filter opening into drop
delay throw on final vocal word
reverb increase during bridge
panning movement on synth texture
```

citehttps://help.suno.com/en/articles/13674305

## Recording

Studio can record audio and MIDI directly onto the timeline. It also provides count-in, pre-roll and latency calibration tools. citehttps://help.suno.com/en/articles/13671041

## Studio timing caution

Suno's current Studio documentation notes that some generated material can still fall slightly before or behind the beat. Use the metronome and inspect timing rather than assuming every generation is perfectly locked. citehttps://help.suno.com/en/articles/13670529

---

# 🔊 PRODUCTION LANGUAGE

Use vocabulary that describes audible results.

### VOCAL

```text
close-mic
vocal-forward
centered lead
clear diction
breathy
raspy
intimate
restrained
controlled grit
stacked harmonies
subtle doubles
wide backing vocals
call and response
```

### DRUMS

```text
punchy transient
soft attack
tight kick
four-on-the-floor
half-time groove
swinging percussion
syncopated groove
restrained hi-hats
live-feeling percussion
```

### BASS

```text
controlled sub bass
round bass
punchy bass
clean kick-bass separation
mono low end
warm low mids
```

### SYNTHS

```text
analog polysynth
warm pad
glassy lead
arpeggiated sequence
dark drone
wide stereo texture
filtered sweep
soft granular texture
```

### DYNAMICS

```text
sparse verse
gradual build
rising tension
full chorus
controlled lift
bridge reduction
final expansion
negative space
preserved contrast
```

### MIX

```text
vocal-forward center
wide supporting layers
uncluttered midrange
controlled low end
restrained reverb
short room ambience
open high end
punchy transients
preserved dynamics
```

---

# ⚠️ COMMUNITY ISSUES AND FIXES

Community advice is experimental unless Suno documents it.

## V6 sounds flat or muffled

Try:

```text
vocal-forward center image, clear vocal articulation, controlled low mids, defined kick and bass separation, clean transient response, restrained ambience, smooth open high end, uncluttered arrangement, preserved dynamic contrast.
```

## Vocal sounds distant

```text
close-mic lead vocal, centered and present, clear diction, dry intimate verse vocal, restrained room ambience, backing vocals behind the lead, instruments supporting rather than masking the vocal.
```

## Final chorus gets too loud or screams

Try:

```text
[Final Chorus | same core melody | controlled emotional lift | steady vocal intensity | no unnecessary belting | consistent dynamic range | centered lead vocal]
```

Avoid excessive escalation language if it produces unwanted escalation:

```text
climax
explosive
peak
massive
screaming
```

This is an experiment, not an official rule.

## Chorus melody drifts

Use identical lyrics, consistent `[Chorus]` labels and preservation language. If it still drifts, stop regenerating the entire song and preserve the best chorus through editing, stems or Studio.

## Instrument disappears

Make its role explicit:

```text
Core electric guitar remains present throughout the arrangement as a supporting harmonic and textural layer. Keep it audible beneath the vocal in verses and wider in choruses.
```

## BPM is ignored

Treat exact BPM language as a target unless the workflow provides an explicit tempo control.

Reinforce feel:

```text
four-on-the-floor
half-time
slow swung groove
double-time
steady club pulse
driving eighth-note pulse
```

## Unwanted instruments appear

Use Exclude plus positive Style direction.

## Suno sings instructions

Simplify bracketed text. Prefer conventional section headers and short descriptors.

## Lyrics UI changes your text

Maintain a master lyric in an external plain-text document. Treat UI behavior during rollouts as potentially changing.

## Structure gets shuffled

Start with:

```text
[Verse]
[Pre-Chorus]
[Chorus]
[Bridge]
[Final Chorus]
```

Add complexity only after the basic structure works.

## Generation ends while the vocal is still singing

Check:

```text
duration
section density
syllable density
number of sections
ending instructions
```

Use Extend or restructure instead of repeatedly forcing an overcrowded generation.

## Reference is too literal

Reduce Audio Influence and test a more interpretive generation.

## Old prompt stopped working

Do not assume prompt portability across models. Rebuild a clean V6 prompt and compare variables one at a time.

---

# 🧪 SCIENTIFIC SUNO TESTING

When a problem appears, create a controlled experiment.

```text
TEST 1
Same lyrics
Same Style
Same model
Same sliders
Change one variable

TEST 2
Same everything
Change one slider

TEST 3
Same everything
Change one Style sentence

TEST 4
Same everything
Change one Lyrics section tag
```

Record:

```text
model
Style version
Lyrics version
Variety
Weirdness
Style Influence
Audio Influence
Personalization
Exclude
Max Mode
reference source
specific failure being tested
```

If two versions differ in many variables, you do not have an experiment.

You have two different songs.

---

# 🧭 THE COMPLETE V6 GOD WORKFLOW

```text
1. DEFINE THE SONG IDEA
        ↓
2. DEFINE THE EMOTIONAL DESTINATION
        ↓
3. DEVELOP / CRITIQUE THE LYRICS
        ↓
4. CHECK SINGABILITY + SYLLABLE DENSITY
        ↓
5. DESIGN SONG STRUCTURE
        ↓
6. WRITE SECTION-SPECIFIC CUES
        ↓
7. BUILD THE STYLE BOX
        ↓
8. CHOOSE MODEL
        ↓
9. CHOOSE ADVANCED OPTIONS
        ↓
10. SET SLIDERS
        ↓
11. ADD ONLY NECESSARY REFERENCES
        ↓
12. GENERATE
        ↓
13. LISTEN CRITICALLY
        ↓
14. IDENTIFY THE SINGLE BIGGEST FAILURE
        ↓
15. CHANGE ONE VARIABLE
        ↓
16. REGENERATE / EDIT
        ↓
17. PRESERVE GREAT SECTIONS
        ↓
18. STEM / REMASTER / STUDIO WHEN APPROPRIATE
        ↓
19. FINAL MIX / MASTER REVIEW
        ↓
20. HUMAN ARTISTIC REVIEW
```

### The core rule

**Do not regenerate what you can surgically repair.**

Once a great section exists, protect it.

---

# 🧯 TROUBLESHOOTING DECISION TREE

```text
THE SONG IS BAD
        |
        +-- Is the IDEA bad? --> Fix concept/story/hook
        |
        +-- Are the LYRICS bad? --> Rewrite/critique with ChatGPT
        |
        +-- Is the STRUCTURE bad? --> Simplify section tags
        |
        +-- Is the STYLE bad? --> Rewrite Style Box
        |
        +-- Is the VOCAL bad? --> Change vocal direction / section cues
        |
        +-- Is the ARRANGEMENT bad? --> Add section-specific arrangement language
        |
        +-- Is the MIX bad? --> Production language / Remaster / Studio
        |
        +-- Is ONE SECTION bad? --> Replace Section
        |
        +-- Is the CHORUS inconsistent? --> Preserve best chorus / edit / stems
        |
        +-- Is the REFERENCE too dominant? --> Reduce Audio Influence
        |
        +-- Is the STYLE ignored? --> Increase Style Influence / simplify Style
        |
        +-- Is the output too chaotic? --> Reduce Weirdness / Variety
        |
        +-- Is the output too safe? --> Increase Weirdness / Variety deliberately
        |
        +-- Is the problem musical precision? --> Move to Studio / DAW
```

---

# 📚 COMMUNITY RESEARCH

Reddit and creator communities are useful for discovering failure cases, experiments and techniques that official documentation does not describe.

Useful research categories include:

- V6 prompting experiments
- structure/meta tag experiments
- chorus consistency experiments
- vocal intensity experiments
- Lyrics Box behavior
- audio-quality complaints
- unusual prompting systems
- editing workflows

Useful existing community discussions from the original guide include:

- https://www.reddit.com/r/SunoAI/comments/1wcyryw/unofficial_suno_v6_prompting_guide_what_has_been/
- https://www.reddit.com/r/SunoAI/comments/1wchwdp/v6_requires_tighter_prompting/
- https://www.reddit.com/r/SunoAI/comments/1wdysw9/suno_v6_solved_got_the_singing_back_flat_rushed/
- https://www.reddit.com/r/SunoAI/comments/1wbubyq/v6_is_garbage_and_a_joke/
- https://www.reddit.com/r/SunoAI/comments/1pap675/a_list_of_song_section_tags_to_help_improve_your/
- https://www.reddit.com/r/SunoAI/comments/1mym1dm/the_guide_to_meta_tags_in_suno_ai_take_control_of_your_sound/
- https://www.reddit.com/r/SunoAI/comments/1um25j7/i_dont_like_the_new_lyric_box/
- https://www.reddit.com/r/SunoAI/comments/1uq2iaa/the_new_lyric_prompt_box/

**Rule:** use community posts to discover a hypothesis, reproduce it, isolate the variable, and keep it only if it improves your actual generation.

---

# 📖 OFFICIAL SUNO RESOURCES

## V6

- Official V6 release: https://suno.com/release-notes/introducing-v6
- V6 FAQ: https://help.suno.com/en/articles/13924481
- Current V6 models: https://help.suno.com/en/articles/13924737
- What's New in V6: https://help.suno.com/en/articles/13924801
- How to change models: https://help.suno.com/en/articles/13924993
- Suno Release Notes: https://suno.com/release-notes

## Creation

- Custom Mode: https://help.suno.com/en/articles/3726721
- Use Your Own Lyrics: https://help.suno.com/en/articles/2415873
- Creative Sliders: https://help.suno.com/en/articles/6141377
- Vocal Gender: https://help.suno.com/en/articles/10153473
- Exclude: https://help.suno.com/en/articles/3161921
- Inspire: https://help.suno.com/en/articles/6882753
- My Taste: https://help.suno.com/en/articles/11362561
- Voices: https://help.suno.com/en/articles/11362369
- Voices FAQ: https://help.suno.com/en/articles/11362433
- Personas: https://help.suno.com/en/articles/3484161
- Custom Models: https://help.suno.com/en/articles/11362497
- Suno Sounds: https://help.suno.com/en/articles/10625537
- Sample + Mashup: https://suno.com/release-notes/meet-our-new-create-features-sample-mashup

## Editing

- Replace Section: https://help.suno.com/en/articles/3271873
- Remaster: https://help.suno.com/en/articles/8105281
- Song Editor: https://help.suno.com/en/articles/6141505
- Reuse Prompt / lyric and voice changes: https://help.suno.com/en/articles/2417409

## Stems

- Advanced Stem Separation: https://suno.com/release-notes/advanced-stems

## Studio

- Studio 2.0: https://help.suno.com/en/articles/13670529
- Studio Chat: https://help.suno.com/en/articles/13670721
- MIDI: https://help.suno.com/en/articles/13670593
- Wavetable: https://help.suno.com/en/articles/13670657
- Audio Effects and Plugins: https://help.suno.com/en/articles/13670785
- Automation: https://help.suno.com/en/articles/13674305
- Recording: https://help.suno.com/en/articles/13671041
- Studio updates: https://suno.com/release-notes/studio-updates-sept26

## Create

- Suno Create: https://suno.com/create

---

# 🛡️ ACCURACY POLICY

This guide uses three evidence levels.

### Level 1 — Official

Directly documented by Suno.

### Level 2 — Reproducible

Observed through controlled experiments and clearly labeled as an observation.

### Level 3 — Community

Reported by Reddit or other creators and explicitly labeled anecdotal/experimental.

When Suno changes the model or interface, older techniques can stop working.

Avoid casually using:

```text
guaranteed
always
never
exactly
locked
deterministic
100% consistent
```

Generative music systems can respond differently to the same prompt.

---

# 🏆 MASTER V6 CONTROLLED PRESET

Use this as a **starting point**, not a universal best configuration:

```text
MODEL: V6
VARIETY: 0% for controlled testing
WEIRDNESS: 25–40%
STYLE INFLUENCE: 85–95%
AUDIO INFLUENCE: 85–100% when preservation matters
PERSONALIZATION: OFF during A/B testing
MAX MODE: ON for important long / consistency-sensitive generations
```

If the output is too sterile:

```text
increase exploration
```

If the reference dominates too much:

```text
reduce Audio Influence
```

If Style is ignored:

```text
simplify Style
increase Style Influence
```

If output is chaotic:

```text
reduce Weirdness / Variety
```

If the arrangement is wrong:

```text
EDIT THE ARRANGEMENT
```

Do not spend endless credits changing sliders when the real problem is a bad section.

---

# 🏁 FINAL WORD

The strongest Suno V6 users are not the people who memorize the most tags.

They are the people who:

- understand what they are trying to make
- communicate musical intent clearly
- write strong lyrics
- use Style for identity
- use Lyrics for song content and local behavior
- use tags as guidance rather than magic commands
- understand what each slider actually changes
- use references deliberately
- isolate variables when testing
- recognize when a generation contains something valuable
- stop regenerating when editing is the smarter move
- use stems and Studio to finish the record

Use Suno to generate possibilities.

Use editing to preserve the best possibilities.

Use Studio or a DAW when exact musical control matters more than probabilistic generation.

Use ChatGPT to brainstorm, interview, critique, score, revise, arrange, engineer prompts and troubleshoot.

And keep asking:

```text
WHAT WOULD MAKE THIS A 10?
```

Then fix that shit.

---

## 🔄 GUIDE STATUS

**Living guide — V6 / September 2026**

This document should be updated whenever Suno changes:

```text
models
creation modes
sliders
Advanced Options
Lyrics Box
Style behavior
references
Voices
Custom Models
Sounds
Sample / Mashup
editing
stems
Studio
pricing / plan availability
or documented model behavior
```

Official Suno documentation should always be checked before treating a previously documented workflow as current.