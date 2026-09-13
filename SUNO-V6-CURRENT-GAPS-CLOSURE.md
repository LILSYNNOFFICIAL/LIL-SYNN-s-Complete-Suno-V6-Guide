# 🎵 SUNO V6 — CURRENT GAPS CLOSURE

> **LIL SYNN's Complete Suno V6 Guide — remaining current-reference coverage**
>
> **Audit date: September 13, 2026**
>
> This file is an additional layer of the guide. It exists so the meaning of **ALL / EVERYTHING** is applied to the areas that can be missed even after documenting the major V6 creation, editing, and Studio workflows.

---

# 1. WHAT “ALL” AND “EVERYTHING” MEAN — FINAL OPERATIONAL RULE

## ALL

For this guide, **ALL** means every currently documented and materially useful part of the current Suno V6 ecosystem that affects a creator's ability to:

- create music;
- write or edit lyrics;
- direct vocals, instruments, arrangement, mood, structure, and production character;
- choose or understand models;
- provide references and source material;
- transform existing songs;
- use voices, personalization, or Custom Models;
- generate production assets;
- separate and manipulate stems;
- work in Studio;
- edit, mix, automate, export, download, share, or organize work;
- understand plans, credits, downloads, rights, and restrictions;
- troubleshoot failures;
- test techniques scientifically;
- and distinguish documented behavior from experimental or community behavior.

## EVERYTHING

**EVERYTHING = ALL + the boundaries of the knowledge.**

That includes:

1. Official documentation.
2. Release-note changes.
3. Current UI/workflow behavior.
4. Plan and platform differences.
5. Reproducible techniques.
6. Community-discovered techniques, clearly labeled.
7. Historical/deprecated behavior.
8. Unknown or unverified behavior.
9. Testing procedures for uncertain behavior.
10. Rights/safety boundaries.
11. Failure modes and recovery procedures.
12. Direct links to authoritative sources.

**Never turn an observed prompt trick into a claimed hidden command. Never turn a community workaround into an official feature. Never turn a historical screenshot into proof of the current UI.**

---

# 2. CURRENT V6 FACT SHEET

| Item | Current documented state |
|---|---|
| v6 | Flagship V6 model; Pro/Premier |
| v6-wild | Exploratory/less predictable V6 variant; Pro/Premier |
| v6-mini | Faster/lighter V6 variant; all users |
| Maximum generation length | Up to 8 minutes for V6-family models |
| v6/v6-wild | Paid plans |
| v6-mini | All plans |
| Studio 2.0 | Premier |
| Custom Models | Pro/Premier; private |
| Advanced Stem Separation | Advanced Split is Premier; other separation modes have broader availability depending on current account/workflow |
| Voices | Current mobile and web ecosystem; availability/features depend on current plan/platform |

Source of truth: current Suno V6 documentation and release notes, not old V5/V5.5 tutorials.

---

# 3. MODEL SELECTION IS A CREATIVE DECISION

### v6

Use when the target is known and you want the most controlled V6-family result.

### v6-wild

Use when you want unexpected ideas, unusual textures, genre collision, or departures from the obvious interpretation.

### v6-mini

Use when speed and iteration volume matter. It is particularly useful for rejecting weak ideas before spending time on higher-control generations.

### Practical three-stage pipeline

```text
v6-mini → DISCOVER
v6-wild → DEVIATE
v6      → REFINe
```

This is a workflow recommendation, not a claim that one model is universally “better.”

---

# 4. SIMPLE MODE VS CUSTOM MODE — WHEN TO USE WHICH

## Simple Mode

Use Simple Mode when you want Suno to infer the appropriate workflow from natural language. It is useful for fast ideation and requests where the desired outcome matters more than manually configuring every field.

### Simple prompt structure

```text
CORE IDEA
+ GENRE / STYLE
+ VOCAL IDENTITY
+ MUSICAL PALETTE
+ ARRANGEMENT ARC
+ EMOTIONAL ARC
+ PRODUCTION CHARACTER
+ CRITICAL CONSTRAINT
```

## Custom Mode

Use Custom Mode when you need explicit control over lyrics, Style direction, vocal gender, advanced controls, references, or repeatable A/B tests.

### Controlled Custom test

```text
LYRICS = CONSTANT
STYLE = CONSTANT
MODEL = CONSTANT
SLIDERS = CONSTANT
REFERENCE = CONSTANT

CHANGE ONE VARIABLE
→ GENERATE
→ COMPARE
→ RECORD RESULT
```

---

# 5. CREATIVE SLIDERS — TESTING MATRIX

Suno currently documents:

- **Weirdness:** Safe → Chaos; 50% is the normal midpoint.
- **Style Influence:** Loose → Strong.
- **Audio Influence:** available when working with audio input.
- **Variety:** current V6 guidance says it can alter/update Style prompting; Variety 0 preserves supplied Style tags most closely.

## Do not conflate these controls

```text
WEIRDNESS       = how far the interpretation may depart / explore
STYLE INFLUENCE = how strongly supplied style direction should matter
AUDIO INFLUENCE = how strongly supplied audio should matter
VARIETY         = output/style-direction variation behavior
```

These are conceptual interpretations for practical testing. They should not be described as exposed model-internal parameters.

## A/B matrix

Run a baseline first. Then vary one control at a time.

```text
A = baseline
B = Weirdness only
C = Style Influence only
D = Audio Influence only
E = Variety only
```

Do not conclude that a slider “always” causes a specific musical result from one pair of generations.

---

# 6. VARIETY = 0 AS A STYLE-PRESERVATION TEST

Current V6 FAQ guidance specifically identifies Variety 0 as the setting to use when you want to retain supplied Style tags.

Use this as a controlled baseline when diagnosing whether unexpected output came from:

- the Style prompt itself;
- model interpretation;
- personalization;
- or variation introduced by the Variety control.

A useful test is:

```text
Same model + same lyrics + same Style
→ Variety 0
→ higher Variety
```

---

# 7. MAX MODE — USE IT DELIBERATELY

Current V6 documentation describes Max Mode as costing more credits and being useful for tasks such as:

- songs longer than two minutes;
- covers where the result should stay close;
- style transfer;
- maintaining vocal consistency across a track;
- maintaining style consistency through longer material.

### Max Mode decision rule

```text
THROWAWAY IDEA → STANDARD
SHORT TEST → STANDARD
LONG / CONSISTENCY-SENSITIVE → CONSIDER MAX
CLOSE COVER / STYLE TRANSFER → CONSIDER MAX
```

Do not state an exact Max Mode credit multiplier unless the current Suno UI/documentation explicitly confirms it. Cost behavior can change.

---

# 8. AUDIO UPLOADS — CURRENT LIMITS

Current Suno documentation distinguishes plan-dependent upload duration:

- Basic/free: up to 60 seconds.
- Pro/Premier: up to 8 minutes.

Treat duration as a current product limit, not a permanent technical law. Recheck if Suno changes the upload policy.

### Upload preparation

Before upload:

1. Trim unnecessary silence.
2. Avoid clipping.
3. Use the cleanest source available.
4. Decide what you want preserved.
5. If possible, use isolated vocals when the goal is vocal identity.
6. Keep the original source file so you can compare results.

### Source-role declaration

```text
PRESERVE = rhythm
PRESERVE = melody
PRESERVE = vocal character
PRESERVE = overall vibe
CHANGE   = instrumentation
CHANGE   = genre
CHANGE   = lyrics
```

Do not leave the role of the upload ambiguous when precision matters.

---

# 9. VOICES — CURRENT WORKFLOW AND COMPATIBILITY DISCIPLINE

Current Suno materials describe Voices as a system for recording/uploading a voice and using it in creations. Voices are available on iOS and Android, and Suno has also documented the web creation workflow.

### Verification

Voice verification uses a displayed phrase and a vocal recording. A clean recording is preferable for reliable verification.

### Voice-source preparation

Best-practice conditions:

- quiet room;
- minimal echo;
- no clipping;
- clear pronunciation;
- consistent distance from microphone;
- clean vocal material when available.

Suno documentation also indicates that an uploaded recording can include background music and that Suno can isolate the vocal through stem processing, but clean/acapella material is the safer starting point when available.

### Compatibility rule

Voice/model compatibility has changed during Suno's rapid feature rollout. Therefore the guide should always record compatibility as **current and date-sensitive**, not permanent.

---

# 10. STYLE PERSONAS VS VOICES

Current documentation distinguishes the concepts:

```text
VOICES
└── includes voice-oriented creation
└── contains Style Personas within the current Voices area

OLD TOP-LEVEL PERSONAS ENTRY
└── replaced by Voices in the current Create experience
```

When reading an old tutorial that says “Personas,” determine whether it means the historical top-level feature or the current Style Persona capability inside Voices.

---

# 11. CUSTOM MODELS — DATASET DISCIPLINE

Current documentation states that Pro/Premier users can create up to three private Custom Models using at least six songs and that the creator must own the rights to uploaded songs.

### Better dataset

```text
TRACK 1 ─┐
TRACK 2 ─┤
TRACK 3 ─┤
TRACK 4 ─┼→ SAME ARTISTIC IDENTITY
TRACK 5 ─┤
TRACK 6 ─┘
```

If the six tracks are radically unrelated, the resulting personalized model may be less useful for a narrow artistic target.

### Dataset checklist

- rights owned/authorized;
- representative material;
- coherent artistic identity;
- technically usable recordings;
- no accidental unrelated tracks;
- enough variety within the intended identity to avoid training on one narrow accident.

Custom Models are private; do not describe them as shareable model assets unless current Suno documentation says otherwise.

---

# 12. MY TASTE — GLOBAL PERSONALIZATION CONTROL

My Taste learns from a user's preferences and can influence creation through Style Augmentation/Magic Wand behavior.

### Experimental-control rule

When comparing prompts, keep My Taste in the same state.

```text
TEST A → My Taste ON
TEST B → My Taste ON
```

or

```text
TEST A → My Taste OFF
TEST B → My Taste OFF
```

Do not switch it between tests and then attribute the difference to the prompt.

---

# 13. INSPIRE — PLAYLIST AS CREATIVE REFERENCE

Inspire can use a playlist as an inspiration source in Custom Mode.

For tighter control, use a small, coherent reference playlist rather than an enormous collection of unrelated music.

### Reference playlist design

```text
3–5 songs
↓
shared emotional / production identity
↓
explicitly state what should be original
↓
generate
```

A reference playlist is not a license to reproduce another creator's copyrighted material.

---

# 14. LYRICIST AND THE NEW LYRIC WORKFLOW

Current lyric tooling includes:

- Lyricist examples;
- natural-language editing;
- variations and references;
- full-screen lyric editing;
- structure labels;
- autosave.

### Separate writing from performance

```text
LYRIC TOOL
→ wording / rhyme / structure / revision

MUSIC MODEL
→ melody / phrasing / instrumentation / performance
```

This separation makes debugging easier. If the lyric is wrong, fix the lyric. If the performance is wrong, use a musical edit workflow rather than rewriting the entire lyric unnecessarily.

---

# 15. SINGLE-LYRIC EDITS

V6 supports updating an individual lyric without rebuilding the entire song in the applicable editing workflow.

Use this when:

- one word is wrong;
- one line is awkward;
- a pronunciation needs changing;
- the existing performance is otherwise valuable.

Do not use a whole-song regeneration when the requested repair is genuinely local unless you want a new interpretation.

---

# 16. EXTEND / CROP / REUSE PROMPT / ADJUST SPEED — WORKFLOW MAP

These tools solve different problems.

| Tool | Use it when |
|---|---|
| Extend | Continue the song beyond the current material |
| Crop | Remove unwanted material / isolate a useful range |
| Reuse Prompt | Reuse the creative setup from another song |
| Adjust Speed | Change playback/song speed without treating it as a full rewrite |
| Replace Section | Rebuild a localized section |
| Remaster | Refine sound/texture/balance with subtle variation |
| Cover | Perform a more significant transformation |

### Local-repair principle

```text
WHOLE SONG GOOD + ONE SECTION BAD
→ Replace Section

WHOLE SONG GOOD + SONIC POLISH NEEDED
→ Remaster

WHOLE SONG GOOD + NEED MORE LENGTH
→ Extend

WHOLE SONG GOOD + NEED SMALL TIMING/SPEED CHANGE
→ Adjust Speed
```

Always verify the exact current UI path because Suno changes menu organization.

---

# 17. REMASTER — DO NOT CONFUSE WITH A REWRITE

Current Remaster documentation describes three variation levels:

- Subtle;
- Normal (default);
- High.

Remaster is intended for sound/mix/balance/texture/clarity improvements rather than drastic lyric or style transformation.

### Practical choice

```text
Subtle → preserve original very closely
Normal → modest refinement
High   → more audible variation
```

If the artistic identity needs major transformation, use Cover/editing rather than expecting Remaster to perform a complete rewrite.

---

# 18. ADD VOCALS — SOURCE / STYLE / ADHERENCE

Add Vocals can add a custom vocal layer to an uploaded instrumental or generated instrumental/stem workflow.

Current documentation identifies an **Audio Strength** control that affects adherence to the existing instrumental.

### Workflow

```text
INSTRUMENTAL
↓
DESCRIBE VOCAL + MUSICAL DIRECTION
↓
SET AUDIO STRENGTH
↓
GENERATE VOCAL LAYER
↓
COMPARE AGAINST ORIGINAL INSTRUMENTAL
```

If the instrumental is being damaged too much, test higher adherence rather than changing ten prompt variables at once.

---

# 19. STEM SEPARATION — THREE MODES

Current Advanced Stem Separation documentation identifies:

### Auto Split

Classic separation into 12 broad stem categories. Best for quick, general separation.

### Split from Mix

Extract one selected instrument or voice and produce that element plus the remainder.

### Advanced Split

Select from a much larger instrument vocabulary, approaching 100 instruments. Current documentation identifies this as a Premier feature.

### Decision tree

```text
FAST GENERAL SEPARATION → Auto Split
ONE TARGET ELEMENT      → Split from Mix
DETAILED INSTRUMENT LIST→ Advanced Split
```

Stem separation is not perfect isolation. Listen for artifacts before using a stem as a final master source.

---

# 20. STUDIO 2.0 — CURRENT CAPABILITY MAP

Studio 2.0 is a browser-based production environment available to Premier users.

Current documented areas include:

- multitrack timeline editing;
- MIDI import/record/edit;
- musical typing;
- MIDI controller/Web MIDI workflows;
- audio effects;
- custom plugins;
- Wavetable Synth;
- automation;
- Chat Bar;
- take lanes/recording/editing workflows;
- advanced stems;
- dry/remove-FX workflows;
- export of mixes/stems and supported MIDI/audio formats.

Chrome is recommended. Web MIDI is not currently available on Safari.

Studio is not a VST/Audio Units host. Treat it as its own production environment rather than assuming arbitrary desktop DAW plugins can be loaded directly.

---

# 21. STUDIO EFFECTS — CURRENT BUILT-IN SET

Current Studio 2.0 documentation lists:

- Compressor, including sidechain support;
- EQ;
- Reverb;
- Convolution;
- Delay;
- Distortion;
- Gate.

Effects run in real time. Chains can be reordered, bypassed, and managed through the Studio interface; current documentation also describes saving/loading presets and custom plugins created with the Chat Bar.

### Production chain example

```text
GATE
→ EQ
→ COMPRESSOR
→ DISTORTION (if needed)
→ DELAY
→ REVERB
```

This is an example signal-flow concept, not a universal “correct” order.

---

# 22. STUDIO CHAT BAR — CURRENT BPM-AWARE BEHAVIOR

The September 2, 2026 Studio update specifically made the Chat Bar aware of BPM and able to process tempo changes. It also improved response reliability and added undo for prompt edits.

When testing Chat Bar behavior, record:

- project BPM;
- tempo changes;
- selected track/clip;
- requested operation;
- current effects;
- whether the instruction created, edited, or arranged material.

This turns vague experimentation into a reproducible production log.

---

# 23. STUDIO PLUGIN MANAGEMENT

Current September 2026 Studio behavior includes:

```text
Mac: Cmd-D   = duplicate plugin
PC:  Ctrl-D  = duplicate plugin
Option-drag = duplicate between tracks
Drag/drop   = move/copy plugins between tracks
```

The exact modifier behavior should be rechecked if Suno changes the editor, but these shortcuts are currently documented in the September update.

---

# 24. WAVETABLE SYNTH

Studio's Wavetable Synth can be used for:

- bass;
- leads;
- pads;
- chords;
- synthesized textures.

Presets can be designed through the Chat Bar.

The September 2026 update reports improved high-frequency fidelity and reduced aliasing.

### Better synth instructions

Describe:

```text
SOURCE CHARACTER
+ REGISTER
+ ENVELOPE
+ FILTER BEHAVIOR
+ MODULATION
+ SATURATION / DISTORTION
+ ROLE IN ARRANGEMENT
```

Example:

```text
Dark mono synth bass, short attack, controlled resonance,
low-pass movement opening slightly in the chorus, restrained
saturation, stable low end, supporting the kick rather than masking it.
```

---

# 25. MIDI — AUDIO VS MUSICAL INSTRUCTIONS

Studio supports MIDI import, recording, and editing. Musical typing can provide keyboard-based MIDI input, and Web MIDI can connect compatible controllers where supported.

### Key distinction

```text
MIDI = editable musical instructions
AUDIO = rendered sound
```

A MIDI performance can therefore be edited note-by-note before rendering/using it as part of a production workflow.

---

# 26. STUDIO EXPORT

Current Studio documentation describes export of:

- full songs;
- selected ranges;
- multitrack material;
- supported WAV/MP3 formats;
- individual stems as WAV;
- MIDI for supported Studio-created material.

Premier Studio documentation describes high-quality 32-bit/48 kHz export capabilities for multitracks/stems.

If an export is missing an expected format, first check the current project/export state and current Studio documentation; Suno has already fixed export bugs during the current rollout.

---

# 27. STUDIO PERFORMANCE / BROWSER REQUIREMENTS

Current Studio guidance recommends Google Chrome for best performance and identifies a minimum 768px screen width for Studio use. Mobile is not the supported Studio environment.

Practical troubleshooting order:

```text
CHECK BROWSER
→ CHECK SCREEN SIZE
→ CLOSE HEAVY TABS
→ RELOAD PROJECT
→ VERIFY AUDIO/MIDI ROUTING
→ TEST EXPORT
→ CHECK CURRENT SUNO STATUS / DOCS
```

Do not diagnose a browser-specific Studio problem as a V6 model failure.

---

# 28. CURRENT MOBILE / WEB FEATURE DIFFERENCES

Suno's feature rollout is not synchronized across every platform.

Examples of documented mobile/web differences include:

- Voices reaching iOS/Android through a mobile update;
- iOS Notes and Voice Memos sharing integrations;
- Android Auto / CarPlay support;
- mobile playlist functionality;
- offline playlist listening;
- web-only or initially web-first playlist controls;
- Studio being a web production environment rather than a mobile production app.

### Rule

When documenting a feature, always record:

```text
FEATURE
PLATFORM
PLAN
MODEL (if relevant)
DATE
SOURCE
```

---

# 29. COVER ART / VISUAL CREATION

Current Suno cover-art tooling supports iterative image creation/editing with text prompts and can produce image or video outputs in supported web workflows.

Use visual iteration like musical iteration:

```text
CONCEPT
→ REFERENCE
→ PROMPT
→ RESULT
→ CHANGE ONE MAJOR VARIABLE
→ REPEAT
```

Keep visual identity consistent across:

- song art;
- playlist art;
- profile image;
- profile banner;
- optional video output.

---

# 30. PLAYLISTS AS PRODUCTION ORGANIZATION

Current playlist functionality can be used as a lightweight project-management layer.

Suggested structure:

```text
PROJECT — IDEAS
PROJECT — SHORTLIST
PROJECT — VOCALS
PROJECT — MIX CANDIDATES
PROJECT — FINALISTS
PROJECT — RELEASE
PROJECT — ARCHIVE
```

Current documented playlist improvements include adding/reordering songs, searching within playlists, pinning playlists on web, filtering by creator/source type, playlist shuffle on web, and offline listening on mobile.

Offline listening should not be confused with offline generation.

---

# 31. DOWNLOADS — CURRENT POLICY CHECKPOINT

Current Suno download documentation distinguishes plan-dependent download allowances and rights.

The current policy documentation states, among other things:

- Free users have limited trial downloads under the current policy;
- Pro has a monthly download allowance;
- Premier has a larger monthly allowance;
- download allowance resets on the billing date and does not roll over;
- re-downloading the same song does not consume another allowance;
- multiple formats for the same song count as one download;
- stems count as part of the song's download;
- failed/interrupted downloads do not count;
- additional downloads may be purchasable.

Because Suno changed the policy around September 3, 2026, always use the current download-policy article when quoting exact counts for a user's account.

---

# 32. RIGHTS: COMMERCIAL USE ≠ COPYRIGHT

Current Suno rights documentation distinguishes platform-granted commercial use rights from copyright protection.

Important principles:

```text
COMMERCIAL USE PERMISSION
≠
AUTOMATIC COPYRIGHT PROTECTION
```

Copyright eligibility depends on applicable law and jurisdiction, including questions about human authorship.

Also remember:

- user-written lyrics remain the user's own material under Suno's stated terms;
- third-party lyrics require appropriate permission;
- paid-plan commercial-use treatment depends on when/how the song was created and the applicable current terms;
- subscribing later does not automatically turn older free-plan creations into retroactively commercial-rights-eligible works.

Do not give legal advice as though these platform rules override local law.

---

# 33. SOURCE MATERIAL / MODERATION CHECKPOINT

V6 documentation says Suno applies safeguards to uploaded audio and lyrics.

If an upload or transformation fails, classify the failure before assuming a software bug:

```text
FORMAT?
DURATION?
SIZE?
PLAN?
MODEL?
RIGHTS / SAFETY SCREENING?
TEMPORARY SERVICE ISSUE?
ACTUAL BUG?
```

This prevents endless prompt changes when the real problem is an account, source, or policy constraint.

---

# 34. REMIX PERMISSIONS AND ATTRIBUTION

Current Suno documentation treats remixing broadly, including workflows such as Cover, Extend, Reuse Prompt, and Adjust Speed.

Remix permissions are not identical to ownership.

A public/remixable work can remain attributable to its original version. When working with another creator's material, verify permission and current remix settings rather than assuming that technical access equals legal permission.

Historical songs may have different default remix settings than newer songs.

---

# 35. REUSE PROMPT — PERMISSION CHECK

Reuse Prompt can carry creative setup from another song. If another creator's lyrics are involved, permission requirements still apply.

Use Reuse Prompt to transfer **creative configuration**, not to bypass rights attached to source lyrics or recordings.

---

# 36. HOOKS — CURRENT ECOSYSTEM FEATURE

Hooks are a short-form visual surface for Suno songs/remixes. Suno's release note describes Hooks as free to create and as a way to pair a creator's own video with a Suno song/remix.

This is adjacent to V6 rather than a V6 model control, but it belongs in an “everything Suno creator workflow” guide because it connects finished music to short-form visual publishing.

---

# 37. LISTEN & RANK

Listen & Rank has been used as a Suno engagement/discovery feature in which users rate clips and can receive credits under the applicable program.

Treat this as a platform/community feature rather than a V6 generation control.

Because incentive rules can change, do not hard-code permanent credit amounts without checking the current feature page.

---

# 38. MOBILE CREATION SURFACES

Current Suno mobile updates have included:

- Voices;
- Vocal Gender;
- Create-memory behavior for the last prompt;
- Lyrics Model Selector;
- profile management;
- playlist improvements;
- Android Auto / CarPlay;
- iOS Notes/Voice Memos sharing;
- specialized mobile creation experiences.

Mobile should be treated as a first-class Suno surface, but not assumed to expose every web/Studio capability.

---

# 39. CURRENT RELEASE-NOTE AUDIT PROTOCOL

Because the product is moving quickly, a guide claiming “everything” needs a maintenance protocol.

### Audit order

```text
1. V6 model/help pages
2. Making Music help category
3. Studio 2.0 category
4. Release Notes
5. Downloads / Terms / Rights
6. Mobile updates
7. Current UI tests
8. Community reports
9. Guide update
```

### High-risk facts to retest every audit

- model availability;
- model retirement;
- maximum generation length;
- upload limits;
- slider names and ranges;
- Max Mode behavior/cost;
- Voice compatibility;
- Custom Model requirements;
- stem options;
- Studio export formats;
- download counts;
- commercial-use language;
- remix permissions;
- mobile/web differences.

---

# 40. SCIENTIFIC SUNO TESTING PROTOCOL

When a behavior is uncertain, use a controlled test rather than intuition.

## Test record

```text
DATE:
PLATFORM:
PLAN:
MODEL:
MODE:
LYRICS:
STYLE:
REFERENCES:
WEIRDNESS:
STYLE INFLUENCE:
AUDIO INFLUENCE:
VARIETY:
MAX MODE:
MY TASTE:
VOICE:
CUSTOM MODEL:
SOURCE AUDIO:
RESULT:
OBSERVATION:
CONFIDENCE:
```

## Confidence labels

```text
OFFICIAL
REPRODUCIBLE
LIKELY
COMMUNITY
EXPERIMENTAL
UNKNOWN
```

The more variables that change at once, the weaker the conclusion.

---

# 41. A/B TESTING — CHANGE ONE VARIABLE

Bad test:

```text
new lyrics + new Style + new model + new sliders + new reference
```

Good test:

```text
everything identical
ONLY Style changed
```

### Score dimensions

Use a consistent scale for:

- lyric adherence;
- vocal identity;
- melody/hook;
- rhythm/groove;
- arrangement;
- instrumentation;
- dynamics;
- mix clarity;
- emotional impact;
- unwanted artifacts.

This turns “I think version B is better” into evidence.

---

# 42. PROMPT FAILURE DIAGNOSTIC

When a generation misses the target, identify the failure class first.

```text
WRONG GENRE?
→ fix Style identity

WRONG VOCAL?
→ fix vocal identity/delivery

WRONG STRUCTURE?
→ simplify and strengthen section direction

WRONG ENERGY?
→ fix dynamic/arrangement language

TOO RANDOM?
→ reduce exploratory controls / simplify references

TOO GENERIC?
→ add audible specifics

ONE SECTION BAD?
→ local editing / Replace Section

MIX PROBLEM?
→ stems / Studio / Remaster
```

Do not respond to every failure by making the prompt longer.

---

# 43. PROMPT OVERLOAD FAILURE

More words do not automatically mean more control.

### Symptoms

- contradictory instructions;
- generic adjective pileups;
- too many exact technical values;
- unrelated references;
- impossible simultaneous constraints.

### Repair

```text
REMOVE DUPLICATES
↓
REMOVE CONTRADICTIONS
↓
KEEP MUSICAL IDENTITY
↓
KEEP THE TOP 3–7 PRIORITIES
↓
TEST AGAIN
```

---

# 44. PRODUCTION RESCUE WORKFLOW

When a nearly-good song has one or two serious problems:

```text
DO NOT REGENERATE EVERYTHING FIRST

1. Identify the exact failure.
2. Try single-lyric editing if it is wording.
3. Try Replace Section if it is localized musical behavior.
4. Try Remaster if it is primarily sonic polish.
5. Extract stems if the issue is an individual layer.
6. Move into Studio if detailed production control is required.
7. Regenerate the whole song only when the underlying concept is wrong.
```

This preserves valuable performances.

---

# 45. SAME-CHORUS / CONSISTENCY PRINCIPLE

Exact repetition is not guaranteed merely because the same words appear twice.

For stronger recurring sections:

- make the hook structurally clear;
- keep important lyrical anchors stable;
- avoid unnecessary conflicting directions between repeated sections;
- use local editing when one occurrence is wrong;
- use Max Mode where current Suno guidance says consistency-sensitive long-form tasks benefit from it.

Treat “same chorus” as a **consistency goal**, not a guaranteed command.

---

# 46. GENRE PROMPTING — BUILD FROM AUDIBLE BEHAVIOR

Instead of relying on genre names alone, describe:

```text
GENRE
+ RHYTHMIC FEEL
+ DRUM BEHAVIOR
+ BASS ROLE
+ HARMONIC LANGUAGE
+ INSTRUMENT PALETTE
+ VOCAL DELIVERY
+ ARRANGEMENT ARC
+ MIX CHARACTER
```

This is more robust than a list of fashionable adjectives.

---

# 47. REFERENCE ENGINEERING

References should have explicit roles.

### Good

```text
Reference A = drum groove
Reference B = vocal mood
Reference C = synth palette
Reference D = emotional atmosphere
```

### Weak

```text
Use all these songs and make it sound exactly like them.
```

The first gives Suno a compositional problem. The second creates an ambiguous imitation request and does not explain priority.

---

# 48. SOURCE-ROLE MATRIX FOR MULTIMODAL CREATION

| Source | Primary job |
|---|---|
| Text | explicit intent |
| Song | musical reference |
| Playlist | broader taste/reference field |
| Audio | source material/performance/sonic cue |
| Image | atmosphere/visual narrative |
| Video | motion/pacing/visual narrative |

Always state which source is authoritative when they conflict.

---

# 49. CURRENT STUDIO CREATIVE LOOP

```text
SONG / AUDIO SOURCE
↓
STEMS OR CLIPS
↓
MIDI / GENERATED CLIP / SAMPLE
↓
ARRANGEMENT
↓
EFFECTS
↓
AUTOMATION
↓
TAKE / EDIT / REPLACE
↓
EXPORT
```

Studio should be thought of as the production layer after generative ideation, not as an alternative to all generation workflows.

---

# 50. FINAL “EVERYTHING” CHECKLIST

Before declaring the guide current, confirm coverage of:

- [x] V6
- [x] V6-WILD
- [x] V6-MINI
- [x] model selection
- [x] model migration/retirement
- [x] Simple Mode
- [x] Custom Mode
- [x] Style engineering
- [x] lyric engineering
- [x] structure tags
- [x] Weirdness
- [x] Style Influence
- [x] Audio Influence
- [x] Variety
- [x] Max Mode
- [x] references
- [x] multimodal inputs
- [x] audio uploads
- [x] Voices
- [x] Style Personas
- [x] Custom Models
- [x] My Taste
- [x] Inspire
- [x] Lyricist
- [x] Sounds
- [x] Sample
- [x] Mashup
- [x] Extend
- [x] Crop
- [x] Reuse Prompt
- [x] Adjust Speed
- [x] Song Editor
- [x] Replace Section
- [x] Add Vocals
- [x] Remaster
- [x] stem separation
- [x] Studio 2.0
- [x] Studio Chat
- [x] Studio MIDI
- [x] Musical Typing
- [x] Wavetable Synth
- [x] Effects
- [x] Custom Plugins
- [x] Automation
- [x] Recording/editing/take workflows
- [x] Studio export
- [x] browser/platform considerations
- [x] playlists
- [x] offline playlist listening
- [x] cover art/video creation
- [x] mobile creation surfaces
- [x] iOS integrations
- [x] Android integrations
- [x] Hooks
- [x] Listen & Rank
- [x] downloads
- [x] credits
- [x] commercial-use distinction
- [x] copyright distinction
- [x] remix permissions
- [x] attribution
- [x] source-material rights
- [x] moderation/safeguards
- [x] troubleshooting
- [x] A/B testing
- [x] reproducibility
- [x] community-vs-official evidence discipline
- [x] living-guide maintenance protocol

---

# 51. OFFICIAL CURRENT SOURCE LIBRARY

Use these as the authoritative starting points for future audits:

- V6 FAQ: https://help.suno.com/en/articles/13924481
- Current V6 models: https://help.suno.com/en/articles/13924737
- What's new in V6: https://help.suno.com/en/articles/13924801
- Introducing V6: https://suno.com/release-notes/introducing-v6
- V6 blog: https://suno.com/blog/introducing-v6
- Release notes: https://suno.com/release-notes
- Studio 2.0: https://help.suno.com/en/articles/13670529
- Studio 2.0 release: https://suno.com/release-notes/studio-2
- Studio September 2026 updates: https://suno.com/release-notes/studio-updates-sept26
- Studio effects/plugins: https://help.suno.com/en/articles/13670785
- Advanced/current stem documentation: https://suno.com/release-notes/advanced-stems
- Creative Sliders: https://help.suno.com/en/articles/6141377
- Audio Uploads: https://help.suno.com/en/articles/6141569
- Voices: https://help.suno.com/en/articles/11362433
- Custom Models: https://help.suno.com/en/articles/11362497
- My Taste: https://help.suno.com/en/articles/11362561
- Inspire: https://help.suno.com/en/articles/6882753
- Remaster: https://help.suno.com/en/articles/8105281
- Add Vocals: https://help.suno.com/en/articles/6882817
- Reuse Prompt: https://help.suno.com/en/articles/2551041
- Downloads policy: https://help.suno.com/en/articles/13926209
- Download formats: https://help.suno.com/en/articles/13926081
- Commercial-use guidance: https://help.suno.com/en/articles/9601665

---

# 52. MAINTENANCE RULE

This guide is a **living knowledge base**, not a frozen manual.

When Suno changes:

```text
NEW FEATURE
→ identify affected sections
→ update official facts
→ preserve historical notes where useful
→ label retired behavior
→ retest uncertain techniques
→ update audit date
→ update source links
```

The word **EVERYTHING** therefore means “everything currently knowable, useful, evidenced, and relevant,” not “everything Suno might invent tomorrow.”

---

# END — CURRENT GAPS CLOSURE
