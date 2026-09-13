# 🎵 SUNO V6 CURRENT COVERAGE AUDIT — SEPTEMBER 2026

> Living extension of **LIL SYNN's Complete Suno V6 Guide**.
>
> This audit captures additional current Suno information that must be considered part of the guide's **ALL / EVERYTHING** scope. It is intentionally evidence-labeled so current official behavior is not mixed with historical or speculative behavior.

---

# 1. ALL / EVERYTHING — FINAL OPERATING DEFINITION

## ALL

**ALL** means every currently available, documented, materially useful, and reasonably verifiable Suno V6-family capability relevant to creating, editing, producing, exporting, organizing, publishing, or troubleshooting music: models, creation modes, controls, sliders, inputs, outputs, editing functions, personalization, voices, references, samples, stems, Studio, MIDI, effects, automation, licensing/usage information, plan restrictions, credits, downloads, mobile/web workflows, and established creation techniques.

## EVERYTHING

**EVERYTHING** means ALL of that **plus the surrounding evidence and boundaries**: official documentation, release notes, current UI behavior, reproducible techniques, community techniques when useful, migration/history, plan dependencies, compatibility, limitations, known failure modes, unknowns, deprecated behavior, and explicit distinctions between what Suno guarantees and what creators merely observe.

Everything does **not** mean inventing undocumented features, secret syntax, model internals, guaranteed prompt commands, or future functionality. Unknown remains unknown.

## Evidence labels

- **OFFICIAL** — current Suno Help documentation.
- **RELEASE NOTE** — current Suno release/update documentation.
- **REPRODUCIBLE** — repeatedly observed under controlled testing.
- **COMMUNITY** — reported by creators but not guaranteed by Suno.
- **EXPERIMENTAL** — useful hypothesis requiring testing.
- **HISTORICAL** — previously documented behavior that may no longer apply.
- **UNKNOWN** — insufficient evidence.

---

# 2. CURRENT V6 MODEL BASELINE

Suno currently documents three V6-family models:

| Model | Best use | Availability |
|---|---|---|
| **v6** | Control, precision, polished intentional creation | Pro / Premier |
| **v6-wild** | Exploration, surprise, unusual ideas | Pro / Premier |
| **v6-mini** | Fast/light creation and iteration | All users |
| **Custom Models** | Personalized creation from the creator's own music | Pro / Premier |

Suno's current documentation says the V6 family supports generations of up to **8 minutes**. **OFFICIAL.**

The model picker is in the Create form. Model selection persists until changed. Suno specifically warns that Voices, Custom Models, and My Taste should be used with a compatible model. **OFFICIAL.**

### Recommended model workflow

```text
v6-mini → rapid concept testing
       ↓
v6-wild → unexpected discovery
       ↓
v6 → controlled reconstruction/refinement
       ↓
Editor / Remaster / Stems
       ↓
Studio / external DAW
```

---

# 3. V6'S NATURAL-LANGUAGE WORKFLOW IS ITSELF A MAJOR FEATURE

V6 is not merely a new audio model. Suno explicitly describes V6 as understanding more of the language and building blocks musicians use, including vocals, instrumentation, structure, mood, references, and overall feel.

In Simple Mode, V6 can infer the appropriate creation workflow rather than requiring the creator to know whether to use a specific tool such as Cover, Remix, or Extend. **OFFICIAL.**

### Practical implication

Instead of thinking:

```text
Which button do I need?
```

think:

```text
What musical transformation do I actually want?
```

Then describe that transformation clearly.

Example:

```text
Keep the verse, melody and vocal character intact, but make the chorus much larger with gospel-style backing vocals, wider synths and a stronger emotional lift.
```

The model may select the appropriate supported workflow.

---

# 4. MULTI-INPUT CREATION

V6 can accept multiple supported references in a single creative request, including:

- Suno songs
- playlists
- audio uploads
- images
- video
- written instructions

**OFFICIAL.**

### Reference-role method

When combining inputs, explicitly assign their roles:

```text
SOURCE A → vocal character
SOURCE B → drum groove
SOURCE C → harmonic atmosphere
IMAGE → visual mood
VIDEO → movement / pacing inspiration
TEXT → story and lyrical concept
```

Then specify what must remain original.

This is safer and more controllable than providing several references without explaining their function.

---

# 5. MASHUP / SAMPLE / ISOLATION

V6 officially supports new workflows for combining elements from multiple sources and for sampling/isolation.

Examples documented by Suno include:

```text
Take vocals from source A.
Take drums from source B.
Add new lyrics.
Rebuild the result as 80s synthwave.
```

and:

```text
Sample the riff at 0:45.
Isolate the guitar.
Build a new beat around it.
```

**OFFICIAL.**

### Creative rule

Describe the **role** of the extracted material, not only the fact that it exists:

```text
Use the isolated guitar as the recurring hook.
Keep it recognizable but build a new rhythm section around it.
```

---

# 6. SINGLE-LYRIC EDITING

V6 can update a single lyric without rebuilding the entire song.

Example:

```text
Change the lyric from “love” to “light.”
```

**OFFICIAL.**

### Use this when

- one word is wrong
- one line needs a correction
- a rhyme needs replacement
- a name needs changing
- a clean/radio edit is required
- the song is already strong and a full regeneration would be wasteful

### Do not use full regeneration when the requested change is genuinely local.

This is one of the most important V6 efficiency principles:

```text
LOCAL PROBLEM → LOCAL EDIT
GLOBAL PROBLEM → GLOBAL REGENERATION
```

---

# 7. LYRICIST + NATURAL-LANGUAGE LYRIC EDITING

Suno's July 2026 lyric improvements introduced a more complete writing environment.

Current documented capabilities include:

- **Lyricist** — save examples of lyrics to guide future lyric creation with a similar vibe.
- **Natural-language lyric editing** — ask for changes conversationally.
- **Variations** — generate alternatives around highlighted text.
- **References** — use highlighted text as inspiration for something new.
- **Full-screen editor**.
- **Song structure labels**.
- **Autosave**.

**RELEASE NOTE / OFFICIAL.**

### Lyric revision workflow

```text
Draft
 ↓
Identify weak line
 ↓
Request several alternatives
 ↓
Compare rhyme / meter / meaning
 ↓
Choose one
 ↓
Regenerate only what is necessary
```

---

# 8. VOCAL GENDER

Suno's current help documentation says creators can guide a song toward a male or female voice style. In Simple Mode, the terms **male** or **female** can be used in the description.

**OFFICIAL.**

This should be treated as **voice-style guidance**, not as a guarantee of a specific human identity.

Useful direction can combine gender guidance with audible characteristics:

```text
female alto vocal, intimate delivery, breathy upper register
```

or:

```text
male low-register vocal, restrained conversational delivery, warm chest resonance
```

---

# 9. VOICES — CURRENT POSITION IN THE SYSTEM

Voices lets creators record/use their own voice in Suno songs. Suno announced Voices on iOS and Android in August 2026 and said it was available to try on free plans with additional paid-plan functionality.

**RELEASE NOTE / OFFICIAL.**

### Voice preparation

Best-practice guidance:

- quiet recording environment
- minimal room reflection
- no clipping
- clear pronunciation
- clean vocal source where possible
- consistent microphone technique

Suno's Voice workflow can work with background music and can isolate the vocal when needed, but a clean vocal/acapella source is preferable when available.

### Rights

Only use voices you have permission to use. A technical ability to reproduce a voice does not itself establish legal permission.

---

# 10. MY TASTE

Suno documents **My Taste** as a personalization system that learns from what the user enjoys on Suno and uses that information to provide a more personalized experience.

**OFFICIAL.**

### Practical consequence

When comparing generations, remember that personalization can become another variable.

For controlled experiments:

```text
Keep model fixed.
Keep prompt fixed.
Keep sliders fixed.
Keep references fixed.
Record whether personalization features are active.
```

Do not attribute every output difference to prompt wording if another personalization layer may have changed.

---

# 11. INSPIRE

Suno documents **Inspire** as a way to create a new song based on the style of a playlist.

**OFFICIAL.**

Conceptually:

```text
playlist identity
      ↓
Inspire
      ↓
new song
```

Treat playlist-level influence as inspiration rather than assuming it reproduces a particular source song.

---

# 12. SUNO SOUNDS

Suno Sounds is documented as an **experimental** feature for generating individual audio materials such as:

- one-shots
- loops
- sound effects
- instrument samples
- ambient noises

For loops, BPM can be specified.

**OFFICIAL / EXPERIMENTAL.**

### Sounds → Studio workflow

```text
Generate sound
 ↓
Select useful one-shot/loop
 ↓
Bring into production workflow
 ↓
Layer / process / automate
 ↓
Export
```

Do not confuse Sounds with a full song generator. It is a sound-material generation tool.

---

# 13. STEM SEPARATION — CURRENT COST/TYPE MATRIX

Suno currently documents three stem-separation modes:

| Mode | Result | Availability | Current documented cost |
|---|---|---|---|
| **Auto Split** | Up to 12 stem categories | Pro / Premier | 50 credits/extraction |
| **Split from Mix** | Selected instrument/voice + complement | Pro / Premier | 10 credits/stem |
| **Advanced Split** | Nearly 100 selectable instruments | Premier | 10 credits/stem |

**OFFICIAL.**

Examples of use:

```text
Need quick broad stems → Auto Split
Need one vocal/instrument isolated → Split from Mix
Need surgical instrument extraction → Advanced Split
```

### Important distinction

Stem separation is not the same as recovering the original multitrack recording. It is source separation and can contain artifacts.

---

# 14. REMASTER

Suno's current documentation describes Remaster as a way to create subtle variations of an existing clip and provides control over the final sound.

**OFFICIAL.**

### Remaster decision rule

Use Remaster when:

- composition is already good
- performance is already good
- the overall result is close
- the problem is primarily sonic/presentation-related

Do not use Remaster as the first solution when the composition itself is wrong.

```text
Bad composition → regenerate/edit
Good composition + weak presentation → consider Remaster
```

---

# 15. STUDIO 2.0 — CURRENT PRODUCTION SCOPE

Studio 2.0 is a browser-based generative DAW and is available to **Premier** subscribers.

Current documented feature areas include:

- MIDI import
- MIDI recording
- MIDI editing
- musical typing
- MIDI controller support
- Chat Bar
- generated instruments/vocals
- custom plugins
- synth presets
- audio effects
- sidechain compression
- convolution reverb
- wavetable synth
- automation
- advanced stem separation
- clip editing
- Take Lanes
- recording
- Remove FX / Get Dry
- project/library access
- export

**OFFICIAL / RELEASE NOTE.**

### Studio mental model

```text
Suno generation
      ↓
Studio editing
      ↓
MIDI / synth / effects
      ↓
automation
      ↓
stems / multitrack
      ↓
export
```

---

# 16. STUDIO MIDI

Studio supports importing, recording, editing, and playing MIDI. Musical typing allows a computer keyboard to act as an input device. External MIDI/Web MIDI can also be used where supported.

Suno has also documented audio-to-MIDI and MIDI-to-audio workflows.

### Practical MIDI workflow

```text
Create / import MIDI
 ↓
Edit notes in piano roll
 ↓
Use MIDI as musical material
 ↓
Generate/assign audio
 ↓
Mix and automate
```

MIDI is fundamentally different from rendered audio: notes remain editable rather than being fixed waveform material.

---

# 17. STUDIO WAVETABLE SYNTH

Studio 2.0 includes a wavetable synth intended for:

- basses
- leads
- pads
- chords
- additional synth layers

Suno documents Chat Bar support for designing synth presets.

### Layering strategy

Use the synth to fill a specific missing role rather than automatically adding more sound:

```text
Song lacks sub support → add controlled bass
Song lacks chorus width → add pad layer
Song lacks hook reinforcement → add lead
Song lacks harmonic movement → add chord layer
```

---

# 18. STUDIO AUDIO EFFECTS

Current Studio documentation/release material identifies effect families including:

- Compressor
- Convolution
- Delay
- Distortion
- EQ
- Gate
- Reverb

Studio 2.0 also documents sidechain compression and custom effect creation through Chat Bar.

### Production principle

Effects should solve a purpose:

```text
EQ → spectral balance
Compression → dynamics control
Gate → unwanted low-level material control
Delay → rhythmic/spatial repetition
Reverb → acoustic/spatial depth
Distortion → harmonic density/character
Convolution → modeled space/impulse response character
```

---

# 19. STUDIO AUTOMATION

Automation allows effect parameters to change over time.

Useful automation targets include:

- effect amount
- filter movement
- reverb send
- delay level
- dynamics behavior
- transitions
- build/drop intensity

### Musical automation principle

```text
Static sound = stable identity
Automation = movement

Movement should support arrangement, not merely demonstrate a plugin.
```

---

# 20. STUDIO CHAT BAR

Studio Chat Bar can be used to:

- generate instruments and vocals
- create custom plugins
- design synth presets
- help with sessions
- make production changes through natural-language interaction

The September 2026 Studio update also added understanding of BPM/tempo changes, undo for prompt edits, plugin copy/duplicate improvements, improved wavetable fidelity, and faster playback/project loading.

**RELEASE NOTE.**

### Chat Bar principle

Describe the musical outcome first:

```text
Make the bass tighter and leave more space for the kick.
```

rather than relying solely on implementation vocabulary:

```text
Change compressor threshold.
```

Use implementation terms when you already know the technical target.

---

# 21. STUDIO RECORDING / TAKE LANES / CLIP WORKFLOW

Current Studio help materials include dedicated workflows for recording, editing clips, Take Lanes, and removing effects/getting dry material.

### General recording workflow

```text
Record
 ↓
Review take
 ↓
Compare takes
 ↓
Choose/comp takes where appropriate
 ↓
Edit timing/content
 ↓
Process
 ↓
Automate
 ↓
Export
```

Take Lanes should be treated as a performance-selection workflow rather than a replacement for the entire arrangement system.

---

# 22. EXPORT MATRIX

Current Suno documentation says available download formats depend on plan and location/workflow.

| Format | Current documented availability |
|---|---|
| **MP3** | Song downloads on all plans; web and mobile |
| **WAV** | Pro/Premier; web |
| **Video** | Songs can be downloaded as video files |
| **Stems** | Individual stem files when available |
| **MIDI** | Songs created in Suno Studio; Premier |

**OFFICIAL.**

Studio provides additional production-oriented export options, including high-quality multitrack/stem workflows for eligible users.

### Rule

Do not assume every format appears on every device, plan, song, or feature. Suno explicitly notes that available options can vary.

---

# 23. DOWNLOAD LIMITS — CURRENT NUMBERS

Suno currently documents:

| Plan | Download allowance |
|---|---:|
| **Free** | Up to 7 lifetime trial downloads |
| **Pro** | 20/month |
| **Premier** | 60/month |

Pro/Premier allowances reset on the billing date and do not roll over.

Additional documented rules:

- re-downloading the same song does not consume another download
- multiple formats for the same song count as one song download
- stems are included with that song's download
- failed/interrupted downloads do not count
- additional downloads can be purchased
- Studio workflows are not affected by these download limits

**OFFICIAL.**

---

# 24. V6 GENERATION CREDIT ECONOMICS

Suno's current V6 FAQ states that V6 generations retain the same basic generation cost as prior models: **two songs for 10 credits**.

The FAQ also warns that providing many images/videos in prompts can increase credit cost.

**OFFICIAL.**

### Efficiency rule

Use cheap iteration for discovery and reserve expensive/credit-intensive operations for decisions that survived testing.

```text
Explore → select → refine → edit → export
```

Do not repeatedly spend credits solving a problem that could have been diagnosed with one controlled test.

---

# 25. SONG DURATION

Current V6-family documentation states that v6, v6-wild, and v6-mini can generate up to **8 minutes in one generation**.

Extend remains the tool for continuing a song beyond the generated material.

**OFFICIAL.**

### Duration strategy

```text
Short idea → generate normally
Long complete arrangement → use duration intentionally
Song needs more material → Extend
Song has unwanted material → Crop/edit
```

---

# 26. COVER ART / VISUAL CREATION

Suno's July 2026 release notes documented image iteration using text prompts. An image can be dropped into Suno and modified with text, producing either an image or a video.

Supported visual contexts include:

- songs
- playlists
- profile images
- profile banners

**RELEASE NOTE.**

### Visual prompt principle

Treat visual editing like musical editing:

```text
LOCK what must remain.
CHANGE only what needs changing.
STATE prohibited changes when necessary.
```

For iterative artwork, explicitly identify:

```text
SUBJECT LOCK
CLOTHING LOCK
POSE LOCK
BACKGROUND LOCK
ACCESSORY LOCK
COLOR LOCK
CAMERA LOCK
ONLY CHANGE: [specific requested change]
```

---

# 27. PLAYLISTS AND OFFLINE MOBILE LISTENING

Suno's August 2026 updates added playlist improvements and offline playlist listening on mobile.

Documented playlist improvements include:

- shuffle on web
- quick add to library
- filters for playlists made by you, Suno, or another creator
- adding/reordering songs
- grid/list library views
- playlist search
- pinning playlists on web
- playlist cover art generation

Offline playlists on mobile allow saved playlists to be listened to without network connectivity.

**RELEASE NOTE.**

These are library/discovery capabilities, but they belong in an exhaustive Suno guide because they affect how finished work is organized and reviewed.

---

# 28. MOBILE CREATION / iMESSAGE

Suno added an iMessage keyboard integration for iOS in July 2026.

The documented workflow allows users to:

1. update the Suno app
2. add/find Suno in iMessage extensions
3. record using voice or type lyrics
4. select styles
5. create a song
6. send the resulting song through iMessage

**RELEASE NOTE.**

This is platform-specific and should not be treated as a universal web/Android workflow.

---

# 29. SPECIALIZED MOBILE CREATION

Suno introduced a mobile soccer-anthem creation flow in July 2026.

The documented workflow asks four questions about a team and creates a song around those answers.

**RELEASE NOTE.**

This demonstrates an important principle for the guide: Suno includes specialized guided creation experiences that may not appear as generic Create-mode controls.

---

# 30. COPYRIGHT / RIGHTS / SAFEGUARDS

Suno states that V6 development includes safeguards around uploaded audio and lyrics, including screening intended to address unauthorized use and abuse.

**OFFICIAL / RELEASE NOTE.**

### Creator rule

Before uploading material, verify that you have the necessary rights or permissions.

This applies particularly to:

- audio uploads
- lyrics
- samples
- reference recordings
- voices
- Custom Model training material

Do not interpret a technical feature's availability as a license to use someone else's copyrighted material.

---

# 31. CUSTOM MODEL RIGHTS REQUIREMENT

Suno's current documentation says Custom Models require songs for which the creator owns the rights. The current documented limit is up to **three private Custom Models**, built from at least **six songs**.

Custom Models are private and cannot be shared between users.

**OFFICIAL.**

### Dataset principle

For a useful personal model, dataset consistency generally matters more than random variety.

```text
coherent identity
+ consistent production
+ representative examples
= more useful personalized model
```

---

# 32. A/B TESTING — COMPLETE V6 PROTOCOL

For serious experimentation:

### Lock

- model
- lyrics
- Style
- references
- duration
- input audio
- Variety
- Weirdness
- Style Influence
- Audio Influence
- Max Mode status

### Change exactly one variable

Example:

```text
Trial A → Weirdness 35%
Trial B → Weirdness 50%
```

Do not simultaneously change:

```text
Weirdness + Style Influence + lyrics + genre + reference
```

because the experiment becomes uninterpretable.

### Score

Use a fixed rubric:

| Dimension | Score |
|---|---:|
| Vocal identity | /10 |
| Melody | /10 |
| Lyrics delivery | /10 |
| Arrangement | /10 |
| Groove | /10 |
| Sound design | /10 |
| Mix | /10 |
| Emotional impact | /10 |
| Hook | /10 |
| Overall | /10 |

---

# 33. RESCUE WORKFLOW

When a generation contains one excellent section and several weak sections:

```text
DO NOT immediately throw away the entire song.

1. Identify the strongest section.
2. Preserve it.
3. Crop/extend/edit as appropriate.
4. Replace the weakest section.
5. Use stems if separation is useful.
6. Move to Studio for production fixes.
7. Remaster only after the musical structure is correct.
```

### Decision hierarchy

```text
Composition problem → Edit/regenerate
Performance problem → Vocal/edit workflow
Arrangement problem → Replace/Extend/Edit
Balance problem → Stems/Studio
Sonic polish problem → Remaster/Studio
Final mastering problem → Studio/external DAW
```

---

# 34. WHAT NOT TO ASSUME

Never automatically assume:

- a bracketed tag is a deterministic command
- a prompt adjective has a fixed technical meaning
- an old V5/V5.5 trick remains identical in V6
- a community workaround is official
- a feature exists on every plan
- a feature is identical on web and mobile
- a voice result is guaranteed to match a particular person
- stem separation recreates original multitracks
- Remaster fixes composition
- higher Weirdness is always better
- higher Style Influence is always better
- more prompt text means more control
- more references automatically mean better results
- a successful one-off generation proves causality

---

# 35. CURRENT RELEASE-TRACKING RULE

Because Suno changes rapidly, this guide should be audited against official sources whenever a major model, Studio, Create, Voices, licensing, download, or plan change occurs.

### Audit checklist

```text
1. Check Current Models.
2. Check v6 FAQ.
3. Check Making Music help category.
4. Check Studio 2.0 help category.
5. Check Release Notes.
6. Check downloads/terms.
7. Search for changed feature names.
8. Mark historical behavior.
9. Add new controls.
10. Retest community techniques.
11. Update reference date.
12. Remove claims that are no longer supported.
```

---

# 36. MASTER V6 PRINCIPLE

The complete Suno workflow is not:

```text
Prompt → Generate → Done
```

It is:

```text
IDEA
 ↓
LYRICS / CONCEPT
 ↓
STYLE IDENTITY
 ↓
MODEL SELECTION
 ↓
REFERENCES / INPUTS
 ↓
CREATIVE CONTROLS
 ↓
GENERATION
 ↓
LISTEN
 ↓
SCORE
 ↓
EDIT
 ↓
REPLACE / EXTEND / CROP
 ↓
REMASTER
 ↓
STEM SEPARATION
 ↓
STUDIO PRODUCTION
 ↓
MIDI / SYNTH / EFFECTS / AUTOMATION
 ↓
MIX REVIEW
 ↓
EXPORT
 ↓
ORGANIZE / PLAYLIST / PUBLISH
```

The purpose of the guide is therefore not merely to teach prompts. It is to document the **entire current Suno creation and production system**, including its capabilities, limits, evidence, and changing behavior.

---

# 37. OFFICIAL CURRENT REFERENCE SET

- Current Models — `https://help.suno.com/en/articles/13924737`
- v6 FAQ — `https://help.suno.com/en/articles/13924481`
- Model switching — `https://help.suno.com/en/articles/13924993`
- Song duration — `https://help.suno.com/en/articles/13924929`
- Making Music — `https://help.suno.com/en/categories/550017`
- Release Notes — `https://suno.com/release-notes`
- Introducing v6 — `https://suno.com/release-notes/introducing-v6`
- V6 announcement — `https://suno.com/blog/introducing-v6`
- Downloads — `https://help.suno.com/en/articles/13926209`
- Download types — `https://help.suno.com/en/articles/13926081`
- Stems — `https://help.suno.com/en/articles/13925185`

---

# 38. FINAL SCOPE STATEMENT

**This audit is part of LIL SYNN's Complete Suno V6 Guide.**

Whenever a future update says **ALL** or **EVERYTHING**, interpret those words using the definitions at the top of this document:

> **ALL = every currently available and materially useful Suno V6-family capability and knowledge that can be responsibly documented.**
>
> **EVERYTHING = ALL of that, plus the evidence, limitations, compatibility, history, uncertainty, testing methodology, and boundaries necessary to understand what is actually known.**

The guide should expand when new verified information appears and should contract when obsolete or unsupported claims are discovered.
