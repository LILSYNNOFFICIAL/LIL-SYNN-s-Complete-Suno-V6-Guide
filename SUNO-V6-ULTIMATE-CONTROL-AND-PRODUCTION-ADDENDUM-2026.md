# 🎛️ SUNO V6 ULTIMATE CONTROL & PRODUCTION ADDENDUM — 2026

> **Companion to LIL SYNN's Complete Suno V6 Guide**
>
> **Verified reference date: September 13, 2026**
>
> This addendum implements the major control, testing, production, diagnostic, platform, rights, and workflow upgrades requested for the guide. It intentionally separates what Suno documents from what can be reproduced, what creators report, and what remains unknown.

---

# 1. EVIDENCE STANDARD

Use this hierarchy:

1. **OFFICIAL** — current Suno Help Center documentation.
2. **RELEASE NOTE** — current Suno release notes/product announcements.
3. **REPRODUCIBLE** — repeated controlled testing by the guide author.
4. **COMMUNITY** — creator reports that are useful but not guaranteed.
5. **EXPERIMENTAL** — plausible technique that needs more testing.
6. **UNKNOWN** — insufficient evidence.
7. **RETIRED** — historical behavior no longer current.

Never upgrade a COMMUNITY or EXPERIMENTAL technique into an OFFICIAL command merely because it worked once.

---

# 2. V6 CONTROL MATRIX

| Control / system | v6 | v6-wild | v6-mini | Practical use |
|---|---|---|---|---|
| Primary V6 generation | Yes | Yes | Yes | All creation |
| Controlled refinement | **Best fit** | Possible | Possible | v6 |
| Surprise / exploration | Good | **Best fit** | Good | v6-wild |
| Fast concept iteration | Good | Good | **Best fit** | v6-mini |
| Max Mode | Yes | Verify current UI | Verify current UI | Difficult/fidelity-sensitive work |
| Custom Models | Supported for eligible users | Supported for eligible users | Compatibility varies | Personalized sound |
| Multimodal references | Supported | Supported | V6-family capability; verify current UI | Reference-driven creation |
| Natural-language editing | Supported | Supported | Supported V6-family workflow | Surgical changes |
| Up to 8-minute generation | Yes | Yes | Yes | Long-form generation |

Suno currently describes v6 as its flagship model, v6-wild as the less predictable experimental variant, and v6-mini as the faster version available to all users. All three support up to eight minutes per generation. See: https://help.suno.com/en/articles/13924737 and https://help.suno.com/en/articles/13924801

### Model decision tree

```text
Do I know the musical target?
        |
       YES --------------------> v6
        |
       NO
        |
Do I want Suno to surprise me?
        |
       YES --------------------> v6-wild
        |
       NO
        |
v6-mini for rapid concept exploration
```

### Best production loop

```text
v6-mini → quick ideas
v6-wild → unusual discoveries
v6 → controlled refinement
Edit → stems → Studio 2.0 → QC → export
```

Do not confuse model selection with a quality ranking. The model is a **creative operating mode**: controlled, exploratory, or fast.

---

# 3. V6 PROMPT ANATOMY

A robust prompt can be understood as layers rather than one paragraph:

```text
IDENTITY
↓
ERA / PRODUCTION FAMILY
↓
VOCAL IDENTITY
↓
RHYTHM / GROOVE
↓
INSTRUMENT PALETTE
↓
HARMONIC CHARACTER
↓
ARRANGEMENT ARC
↓
PERFORMANCE
↓
EMOTIONAL ARC
↓
SPATIAL CHARACTER
↓
MIX CHARACTER
↓
MASTER CHARACTER
```

### Identity

Answer: **What is this song?**

```text
Dark electropop / alternative pop
```

### Vocal identity

Answer: **Who/what does the vocal feel like?**

```text
Intimate low-register male vocal, slightly husky, conversational verses, stronger chest voice in the chorus.
```

### Rhythm

Answer: **How does it move?**

```text
Midtempo, tight electronic groove, punchy kick, restrained syncopation.
```

### Arrangement

Answer: **How does energy change?**

```text
Sparse verses → rising pre-chorus → wide chorus → reduced bridge → expanded final chorus.
```

### Production

Answer: **How should the finished record feel?**

```text
Dry close vocal, controlled sub bass, clear low mids, wide chorus, restrained reverb, defined transients.
```

---

# 4. INSTRUCTION HIERARCHY

There is no official Suno document saying that prompts obey a rigid deterministic hierarchy. Treat the following as a **working production model**, not a hidden implementation detail.

When instructions conflict, prioritize the musical information that is most important to the result:

```text
SONG IDENTITY
    ↓
CORE VOCAL / MUSICAL INTENT
    ↓
LYRICS + SECTION STRUCTURE
    ↓
STYLE / ARRANGEMENT DIRECTION
    ↓
REFERENCES
    ↓
CREATIVE CONTROLS
    ↓
LOCAL EDIT REQUEST
    ↓
POST-GENERATION PRODUCTION
```

### Conflict example

Bad:

```text
Minimal intimate acoustic verse with huge distorted drums, enormous orchestral choir, dense EDM bass and sparse instrumentation.
```

Better:

```text
Verse: intimate acoustic guitar, close vocal, sparse percussion.
Chorus: introduce huge drums, wide synths and stacked harmonies.
```

**Rule:** put simultaneous characteristics in the same section only when you genuinely want them simultaneously.

---

# 5. NEGATIVE PROMPTING / AVOIDANCE

Negative prompting is **not documented as a deterministic exclusion language**. Treat exclusion wording as an experimental technique.

Useful forms to test:

```text
avoid excessive reverb
without a huge choir
keep the vocal dry
no distorted guitars
instead of trap drums, use tight electronic drums
```

### Preferred strategy

A positive replacement is often more actionable than a bare prohibition:

```text
Avoid: “no muddy bass.”

Prefer: “controlled sub bass with clean kick-bass separation.”
```

### A/B test

```text
A = positive description only
B = positive + avoidance
C = positive + replacement instruction
```

Keep the model, lyrics, references and sliders fixed.

If B works once and fails later, label the technique **EXPERIMENTAL**, not guaranteed.

---

# 6. CREATIVE SLIDER LABORATORY

Suno currently documents Weirdness, Style Influence and Audio Influence. Current V6 documentation also describes Variety as a style-prompt variation control. See https://help.suno.com/en/articles/6141377 and https://help.suno.com/en/articles/13924481

## Test protocol

Never change multiple major controls during a diagnostic test.

### Weirdness matrix

| Trial | Weirdness | Other variables |
|---|---:|---|
| A | 0–20% | Fixed |
| B | 40–50% | Fixed |
| C | 60–70% | Fixed |
| D | 80–100% | Fixed |

Question: **Does the output become more surprising, less coherent, or simply different?**

### Style Influence matrix

```text
Loose → Medium → Strong
```

Use the same prompt and score:

- style fidelity
- genre coherence
- instrument adherence
- vocal adherence
- unwanted reinterpretation

### Audio Influence matrix

```text
Low → Medium → High
```

Score:

- source rhythm retention
- melody retention
- timbral similarity
- unwanted source artifacts
- creative reinterpretation

### Variety matrix

```text
0 → low → medium → high
```

Variety 0 is particularly useful as a controlled baseline when you want supplied Style tags retained as consistently as possible.

### Max Mode experiment

```text
Standard vs Max
```

Use a difficult task where the difference matters:

- >2-minute song
- close cover
- style transfer
- consistency-sensitive vocal

Do not use Max Mode for every disposable test simply because it exists.

---

# 7. REMASTER VARIATION LAB

Remaster is for sonic refinement rather than rewriting the entire musical identity.

Current Suno documentation exposes Model and Variation Strength controls. See https://help.suno.com/en/articles/8105281

Use a matrix such as:

```text
Original
↓
Subtle remaster
↓
Normal remaster
↓
Higher variation
```

Score:

- vocal identity
- melody retention
- arrangement retention
- clarity
- mix balance
- unwanted changes

If the musical composition itself is wrong, Remaster is usually the wrong tool.

---

# 8. REPRODUCIBILITY PROTOCOL

A technique is not “proven” because one generation worked.

## Minimum controlled test

```text
TEST ID:
DATE:
MODEL:
PLAN:
MODE:
LYRICS VERSION:
STYLE VERSION:
REFERENCE INPUTS:
VOICE:
CUSTOM MODEL:
WEIRDNESS:
STYLE INFLUENCE:
AUDIO INFLUENCE:
VARIETY:
MAX MODE:
TASK:
VARIABLE CHANGED:
OUTPUT IDS:
OBSERVATIONS:
FAILURES:
CONCLUSION:
CONFIDENCE:
```

## Confidence levels

**High:** repeated across multiple independent generations with one variable changed.

**Medium:** repeated trend but significant generative variance remains.

**Low:** one/few successful examples.

**Unknown:** no reliable evidence.

### Reproducibility rule

```text
ONE SUCCESS
≠
CAUSALITY
```

A useful technique should survive repetition.

---

# 9. SUNO MYTHBUSTERS

## Myth: “A tag is a secret command.”

**Verdict:** UNKNOWN unless Suno documents it or controlled tests establish a repeatable effect.

## Myth: “Exact punctuation guarantees a melody.”

**Verdict:** UNKNOWN.

## Myth: “Writing a DAW EQ setting in lyrics applies that EQ.”

**Verdict:** Not a substitute for actual Studio processing.

## Myth: “One perfect prompt always recreates the same song.”

**Verdict:** False as a general deterministic guarantee. Generative variance remains.

## Myth: “Higher Weirdness means higher quality.”

**Verdict:** False. It means a different exploration point; quality depends on the task.

## Myth: “V6-WILD is simply a worse v6.”

**Verdict:** False framing. It is explicitly intended for more unpredictable exploration.

## Myth: “Commercial rights mean copyright is guaranteed.”

**Verdict:** False. Suno explicitly distinguishes commercial-use rights from copyright protection.

## Myth: “A voice feature means permission to clone anyone.”

**Verdict:** False. Technical capability does not establish authorization.

## Myth: “Old V5 prompt recipes automatically work in V6.”

**Verdict:** Unsupported. Retest them under V6.

---

# 10. VOCAL ENGINEERING — FULL TAXONOMY

Describe vocals across independent dimensions:

```text
IDENTITY
REGISTER
TEXTURE
ARTICULATION
DELIVERY
EMOTION
PHRASING
RHYTHMIC BEHAVIOR
HARMONY
DENSITY
DISTANCE
SPATIAL CHARACTER
EFFECT CHARACTER
```

### Register

```text
low / baritone / tenor / alto / high / chest-dominant / head-dominant / falsetto
```

### Texture

```text
clean / husky / breathy / raspy / grainy / warm / airy / dark / bright / intimate
```

### Delivery

```text
conversational / restrained / urgent / detached / pleading / whispered / explosive / rhythmic / legato / clipped
```

### Phrasing

```text
long sustained phrases
short clipped phrases
behind-the-beat delivery
forward rhythmic delivery
melismatic
syllabic
```

### Harmony

```text
double
thirds
octaves
stacked harmonies
call-and-response
choir-like layers
gang vocal
```

### Vocal diagnostic

```text
Wrong identity?
→ change vocal description / Voice / model

Wrong emotion?
→ change delivery + section direction

Wrong phrasing?
→ change lyric syllable density / section direction

Wrong harmony?
→ change local harmony direction

Wrong balance?
→ stems / Studio

Wrong pronunciation?
→ lyric edit / localized edit / remaster test
```

Suno's current documentation supports guiding male/female vocal direction in Custom Mode through Vocal Gender and style wording. See https://help.suno.com/en/articles/10153473

---

# 11. WHY SUNO DID THAT — DIAGNOSTIC TREE

```text
OUTPUT IS WRONG
│
├── Wrong VOCAL
│   ├── Identity problem → Voice / prompt / model
│   ├── Delivery problem → section direction
│   ├── Phrasing problem → lyric structure
│   └── Mix problem → stems / Studio
│
├── Wrong ARRANGEMENT
│   ├── Whole-song identity → Style/model
│   ├── One section → Replace Section
│   ├── Density problem → section direction
│   └── Instrument balance → stems / Studio
│
├── Wrong LYRICS
│   ├── One word → lyric edit
│   ├── One section → localized edit
│   └── Entire concept → rewrite/regenerate
│
├── WRONG SONIC CHARACTER
│   ├── Small refinement → Remaster
│   ├── Individual element → stems
│   └── Mix/production → Studio
│
└── WHOLE SONG MISSED THE BRIEF
    ├── simplify prompt
    ├── change model
    ├── change reference strategy
    └── regenerate
```

### The smallest-fix principle

Always ask:

> **What is the smallest tool that can fix the actual defect without destroying something that already works?**

---

# 12. GENERATION → RESCUE → PRODUCTION

```text
IDEA
↓
GENERATE
↓
AUDITION
↓
IS THE SONG GOOD?
├── NO → diagnose → regenerate with one controlled change
└── YES
    ↓
IS THE PROBLEM LOCAL?
├── YES → Edit / Replace Section / lyric change
└── NO
    ↓
IS IT AN ELEMENT PROBLEM?
├── YES → stems
└── NO
    ↓
IS IT A PRODUCTION PROBLEM?
├── YES → Studio
└── NO
    ↓
SONIC CHARACTER PROBLEM?
├── YES → Remaster test
└── NO
    ↓
QC → EXPORT → RELEASE
```

Never use mastering language to solve a songwriting problem.

---

# 13. STUDIO 2.0 — FULL PRODUCTION MAP

Suno Studio 2.0 is a browser-based production environment for Premier subscribers. Suno documents MIDI, audio effects, a wavetable synth, automation, recording, Chat Bar generation, custom plugins and more. See https://help.suno.com/en/articles/13670529

```text
SONG
↓
TIMELINE
├── AUDIO
├── MIDI
├── TAKE LANES
└── RECORDING
↓
EDITING
├── CLIPS
├── WARP
├── PIANO ROLL
└── ARRANGEMENT
↓
SOUND DESIGN
├── WAVETABLE
├── EFFECTS
└── CUSTOM PLUGINS
↓
AUTOMATION
↓
MIX
↓
EXPORT
```

### Browser guidance

Suno recommends Google Chrome for Studio; Web MIDI is not currently available in Safari. Studio is a desktop-oriented environment rather than the mobile Suno app experience.

### Built-in effects

Current Studio documentation lists:

- Compressor
- EQ
- Reverb
- Convolution
- Delay
- Distortion
- Gate

Compressor includes sidechain support; Convolution uses sampled acoustic profiles/impulse responses. See https://help.suno.com/en/articles/13670785

### Custom plugins

Studio can create custom plugins through the Chat Bar. These are **Suno Studio plugins**, not conventional VST/AU plugins. Current documentation says custom plugins can support presets, automation and MIDI Learn.

### Plugin movement

The September 2, 2026 update added drag-and-drop plugin movement/copying and quick duplication with Cmd-D/Ctrl-D. See https://about.suno.com/release-notes/studio-updates-sept26

---

# 14. STUDIO MIDI DEEP DIVE

Studio MIDI supports:

```text
IMPORT
RECORD
DRAW
MOVE
RESIZE
QUANTIZE
VELOCITY
PITCH BEND
MODULATION
INSTRUMENT SWAP
```

Audio can be dragged onto a MIDI track for transcription in supported workflows. MIDI can also be used as a musical source for generated audio.

### Musical typing

The computer keyboard can act as a MIDI controller, with chord mode and arpeggiator support.

### External MIDI

Web MIDI can connect supported controllers for playing, recording, MIDI Learn and transport functions. Safari currently lacks Web MIDI support in Studio; Chrome is recommended.

---

# 15. WAVETABLE SYNTH DEEP DIVE

The wavetable synth is useful for:

```text
BASS
LEAD
PAD
PLUCK
CHORD
TEXTURE
```

Describe the sound using:

```text
SOURCE CHARACTER
FILTER MOVEMENT
ENVELOPE
PITCH BEHAVIOR
WIDTH
MODULATION
DISTORTION / SATURATION
DYNAMIC BEHAVIOR
```

The September 2026 Studio update improved high-frequency wavetable fidelity and reduced aliasing. Treat the update as current release-note evidence rather than a permanent promise.

---

# 16. AUTOMATION

Automation is for **time-dependent change**.

Use it for:

- volume swells
- panning movement
- filter sweeps
- effect intensity
- delay/reverb changes
- transitions
- chorus lift
- breakdown reduction

### Automation thinking

```text
VERSE
low effect intensity
↓
PRE-CHORUS
increase movement
↓
CHORUS
maximum width / effect
↓
BRIDGE
pull back
↓
FINAL CHORUS
largest controlled movement
```

Do not automate a parameter merely because you can. Automate when the movement contributes to musical storytelling.

---

# 17. RECORDING / TAKE LANES / TIMING

Studio can record audio or MIDI directly onto the timeline. Recording includes count-in/pre-roll options and latency calibration. See https://help.suno.com/en/articles/13671041

Every generation provides two versions; Take Lanes provide a non-destructive place to compare and promote alternatives.

### Timing check

Suno has acknowledged that some Studio generations can fall slightly before or behind the beat. Use the metronome, solo the relevant track, and inspect the timeline before assuming the generation is musically locked.

---

# 18. STUDIO SHORTCUT MASTER TABLE

Current official shortcut reference: https://help.suno.com/en/articles/13680385

| Action | Mac | Windows |
|---|---|---|
| Play/Pause | Space | Space |
| Record | Shift-R | Shift-R |
| Metronome | Shift-C | Shift-C |
| Loop | Cmd-L | Ctrl-L |
| Add Track | Shift-T | Shift-T |
| Save Project | Cmd-S | Ctrl-S |
| Undo | Cmd-Z | Ctrl-Z |
| Redo | Cmd-Shift-Z / Cmd-Y | Ctrl-Shift-Z / Ctrl-Y |
| Solo focused track | Shift-S | Shift-S |
| Mute focused track | Shift-M | Shift-M |
| Chat | 1 | 1 |
| Bottom panel | 2 | 2 |
| Lanes | 3 | 3 |
| Library | 4 | 4 |
| Automation | Shift-A | Shift-A |
| Duplicate | Cmd-D | Ctrl-D |
| Zoom in | Cmd-= | Ctrl-= |
| Zoom out | Cmd-- | Ctrl-- |
| Split | Cmd-E | Ctrl-E |
| Quantize | Shift-Q | Shift-Q |
| Keyboard shortcuts | Shift-? | Shift-? |

Always verify the live official shortcut reference because UI shortcuts can change.

---

# 19. WEB / iOS / ANDROID FEATURE MATRIX

**Verified September 13, 2026. Rollouts can change independently by platform.**

| Capability | Web | iOS | Android | Notes |
|---|---:|---:|---:|---|
| V6 creation | ✓ | ✓ | ✓ | Current V6 family |
| v6-wild | ✓ | ✓ | ✓ | Paid access |
| v6-mini | ✓ | ✓ | ✓ | All users |
| Voices | ✓ | ✓ | ✓ | Mobile Voices rollout announced Aug 7, 2026 |
| Studio 2.0 | ✓ | — | — | Browser-based production environment |
| Web MIDI | ✓ | — | — | Safari currently lacks Web MIDI |
| MIDI production | ✓ | — | — | Studio |
| Full Studio effects | ✓ | — | — | Studio |
| Download formats | Varies | Varies | Varies | Plan/device dependent |

Mobile and web features are subject to staged rollout. Use Suno's release notes for current availability: https://about.suno.com/release-notes

The official mobile-app documentation identifies Suno apps for iOS and Android: https://help.suno.com/en/articles/3134337

---

# 20. RIGHTS / COMMERCIAL RELEASE DECISION TREE

Suno's current paid-subscription documentation says songs **downloaded while subscribed** receive commercial-use rights, while commercial-use rights do not guarantee copyright protection. See https://help.suno.com/en/articles/9601665

Current download documentation says Pro receives 20 monthly downloads, Premier receives 60, paid allowances reset on the billing date, and unused monthly allowances do not roll over. Studio workflows are not subject to those download limits. See https://help.suno.com/en/articles/13926209

### Decision tree

```text
SONG READY FOR RELEASE?
        ↓
WHAT PLAN / DOWNLOAD STATUS?
        ↓
WAS IT DOWNLOADED WHILE THE PAID COMMERCIAL RIGHTS APPLY?
        ↓
DO YOU OWN / HAVE PERMISSION FOR ALL INPUT MATERIAL?
        ↓
ANY THIRD-PARTY LYRICS / VOICES / SAMPLES / RECORDINGS?
        ↓
CHECK THOSE RIGHTS SEPARATELY
        ↓
COMMERCIAL USE
        ↓
COPYRIGHT QUESTION?
        ↓
CHECK THE LAW / COPYRIGHT OFFICE FOR YOUR JURISDICTION
```

### Important distinctions

```text
COMMERCIAL USE RIGHT
≠
COPYRIGHT GUARANTEE

DOWNLOAD ACCESS
≠
OWNERSHIP OF THIRD-PARTY INPUTS

VOICE TECHNOLOGY
≠
PERMISSION TO USE A PERSON'S VOICE
```

Do not give legal advice from a music-generation prompt. For a commercial release, retain records of plan status, download status, source permissions, collaborators, lyrics ownership, and final files.

---

# 21. DOWNLOAD MANAGEMENT

Current documented download rules include:

| Plan | Current allowance |
|---|---:|
| Free | Up to 7 lifetime trial downloads for eligible accounts; trial downloads are non-commercial |
| Pro | 20/month |
| Premier | 60/month |

One song counts once regardless of how many supported formats are downloaded; stems from the same song are included in that song's download accounting. Failed/interrupted downloads do not count. Additional download purchases can be available.

See https://help.suno.com/en/articles/13926081 and https://help.suno.com/en/articles/13926209

---

# 22. CREATOR'S OPERATING SYSTEM

This is the master methodology for the entire guide.

```text
01 — IDEA
    Define the emotional and musical target.

02 — MODEL
    v6 = control
    v6-wild = discovery
    v6-mini = speed

03 — LYRIC ARCHITECTURE
    Build singable sections and a memorable hook.

04 — STYLE ARCHITECTURE
    Describe audible behavior rather than adjective soup.

05 — REFERENCES
    Assign each reference a specific role.

06 — CONTROLS
    Set sliders intentionally.

07 — GENERATE
    Produce candidates.

08 — AUDITION
    Listen without immediately rewriting everything.

09 — DIAGNOSE
    Identify the single largest defect.

10 — CONTROLLED ITERATION
    Change one major variable.

11 — SELECT
    Preserve the strongest musical information.

12 — SURGICAL EDIT
    Fix bad words, lines, sections or moments locally.

13 — STEMS
    Separate elements when individual control is required.

14 — STUDIO
    Edit, record, MIDI-edit, synthesize, process and automate.

15 — MIX
    Balance vocal, rhythm section, low end, mids and space.

16 — MASTER / REMASTER
    Refine final sonic character without destroying good musical information.

17 — QC
    Check artifacts, timing, clipping, transitions, lyrics, endings and metadata.

18 — RIGHTS
    Verify plan/download status and source permissions.

19 — EXPORT
    Save the final files and working assets.

20 — ARCHIVE
    Preserve prompt, lyrics, source files, versions and production notes.
```

### Exit criteria

Do not move forward merely because the song is “pretty good.” Ask:

```text
✓ Does the song communicate the intended emotion?
✓ Is the hook memorable?
✓ Is the vocal believable and appropriate?
✓ Does the arrangement support the lyric?
✓ Are bad sections repaired rather than unnecessarily regenerated?
✓ Is the low end controlled?
✓ Are there audible artifacts?
✓ Is the ending intentional?
✓ Does the final export match the intended use?
✓ Are rights/source records complete?
```

---

# 23. MASTER PRODUCTION RESCUE TABLE

| Problem | First tool to try | Escalate to |
|---|---|---|
| One wrong word | Lyric edit | Replace Section |
| One bad line | Lyric/local edit | Replace Section |
| One bad vocal phrase | Local edit | Replace Section |
| Whole section wrong | Replace Section | Regenerate |
| Wrong instrument balance | Stems | Studio |
| Muddy mix | Stems / Studio | External DAW |
| Need dry source | Remove FX | Stem extraction |
| Sonic character slightly wrong | Remaster | Rebuild |
| Need exact note edits | Studio MIDI | External DAW |
| Need dynamic movement | Automation | External DAW |
| Entire concept wrong | New generation | New model/reference strategy |

---

# 24. PRODUCTION CHECKLIST

## Generation

- [ ] Model selected intentionally.
- [ ] Lyrics version recorded.
- [ ] Style version recorded.
- [ ] References assigned roles.
- [ ] Slider values recorded.
- [ ] Max Mode decision recorded.

## Editing

- [ ] Local defects identified.
- [ ] Best take preserved.
- [ ] Replace Section used where appropriate.
- [ ] Remaster used only for sonic refinement.

## Studio

- [ ] Timing checked against metronome.
- [ ] MIDI checked if used.
- [ ] Effects checked for unwanted artifacts.
- [ ] Automation checked.
- [ ] Plugin chain documented.
- [ ] Export settings verified.

## Release

- [ ] Final WAV/MP3 verified.
- [ ] Stems archived if needed.
- [ ] Lyrics finalized.
- [ ] Artwork/metadata finalized.
- [ ] Rights/source records complete.
- [ ] Commercial-use eligibility checked.
- [ ] Copyright assumptions kept separate from Suno commercial-use rights.

---

# 25. OFFICIAL CURRENT RESOURCE INDEX

### V6

- Current Models: https://help.suno.com/en/articles/13924737
- v6 FAQ: https://help.suno.com/en/articles/13924481
- What's New in v6: https://help.suno.com/en/articles/13924801
- Model Switching: https://help.suno.com/en/articles/13924993
- Introducing v6: https://suno.com/release-notes/introducing-v6

### Creation

- Creative Sliders: https://help.suno.com/en/articles/6141377
- Custom Models: https://help.suno.com/en/articles/11362497
- Voices: https://help.suno.com/en/articles/11362369
- Vocal Gender: https://help.suno.com/en/articles/10153473
- Suno Sounds: https://help.suno.com/en/articles/10625537
- Audio Uploads: https://help.suno.com/en/articles/6141569

### Studio

- Studio 2.0: https://help.suno.com/en/articles/13670529
- Studio 2.0 category: https://help.suno.com/en/categories/2701953-studio-2-0
- Effects / Plugins: https://help.suno.com/en/articles/13670785
- Recording: https://help.suno.com/en/articles/13671041
- Keyboard Shortcuts: https://help.suno.com/en/articles/13680385
- Studio September update: https://about.suno.com/release-notes/studio-updates-sept26
- Studio release: https://suno.com/release-notes/studio-2

### Editing / Production

- Song Editor: https://help.suno.com/en/articles/6141505
- Replace Section: https://help.suno.com/en/articles/3271873
- Extend: https://help.suno.com/en/articles/2409601
- Crop: https://help.suno.com/en/articles/3166529
- Remix: https://help.suno.com/en/articles/6050497
- Reuse Prompt: https://help.suno.com/en/articles/2551041
- Remaster: https://help.suno.com/en/articles/8105281
- Advanced Stems: https://help.suno.com/en/articles/13925185
- Remove FX: https://help.suno.com/en/articles/13671105
- Studio Export: https://help.suno.com/en/articles/13925249

### Rights / Downloads

- Paid Subscription Rights: https://help.suno.com/en/articles/9601665
- Download Limits: https://help.suno.com/en/articles/13926209
- Download Types: https://help.suno.com/en/articles/13926081
- Downloads / Models / Terms FAQ: https://help.suno.com/en/articles/13614785
- Rights & Ownership category: https://help.suno.com/en/categories/550145

### Current product history

- Suno Release Notes: https://about.suno.com/release-notes
- Suno Blog: https://about.suno.com/blog

---

# 26. FINAL RULE

The guide's goal is not to make Suno look deterministic.

The goal is to make the **creator more deterministic**.

```text
BETTER OBSERVATION
        ↓
BETTER DIAGNOSIS
        ↓
SMALLER CHANGE
        ↓
LESS WASTED GENERATION
        ↓
BETTER SONG
        ↓
BETTER PRODUCTION
```

**Use Suno for generation. Use controlled experimentation for knowledge. Use Studio for production. Use your ears for truth.**
