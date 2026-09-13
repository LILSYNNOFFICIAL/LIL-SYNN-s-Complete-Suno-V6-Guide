# 🎵 SUNO V6 EVERYTHING EXPANSION

> **Living addendum to LIL SYNN's Complete Suno V6 Guide**
>
> **Reference date: September 13, 2026**
>
> This file exists to capture the current V6-family information, production workflows, controls, limitations, compatibility notes, testing methodology, and practical techniques that should be treated as part of the guide's "ALL / EVERYTHING" scope.

---

# 1. THE OPERATING DEFINITION OF “ALL” AND “EVERYTHING”

## ALL

**ALL** means every currently available and materially useful piece of Suno V6-family knowledge that belongs in a serious creator's reference: documented models, creation modes, controls, sliders, options, inputs, outputs, editing tools, production tools, Studio functions, voice/personalization systems, prompt/lyric techniques, plan restrictions, credit behavior, licensing/usage information, troubleshooting, migration behavior, and reproducible workflows.

## EVERYTHING

**EVERYTHING** means ALL of the above **plus the boundaries around the knowledge**: what Suno officially confirms, what can be reproduced in controlled tests, what is community-discovered, what is anecdotal, what is plan-dependent, what has changed, what is deprecated, and what is unknown or not guaranteed.

This definition deliberately excludes invented secret commands, fabricated controls, unsupported claims about model internals, and assumptions presented as facts.

## Evidence labels

Use these labels throughout the guide:

- **OFFICIAL** — documented by Suno.
- **RELEASE NOTE** — documented in Suno's product/update history.
- **REPRODUCIBLE** — observed repeatedly under controlled conditions.
- **COMMUNITY** — useful reports that are not guaranteed by Suno.
- **EXPERIMENTAL** — plausible technique requiring testing.
- **UNKNOWN** — insufficient evidence.
- **RETIRED** — historical behavior no longer available for new generation.

**Rule:** a prompt technique can be useful without being a guaranteed command. A section tag can influence a generation without being a formal programming language.

---

# 2. CURRENT V6 FAMILY

| Model | Purpose | Availability | Practical strategy |
|---|---|---|---|
| **v6** | Controlled creation and refinement | Pro / Premier | Default for intentional final work |
| **v6-wild** | Discovery and experimentation | Pro / Premier | Generate unusual ideas, then refine winners in v6 |
| **v6-mini** | Fast/light iteration | All users | Test concepts and iterate quickly |
| **Custom Models** | Personalized model trained on your music | Pro / Premier | Build a private model around music you own |

All three V6-family models support up to **8 minutes per generation** according to current Suno documentation.

### V6 decision tree

```text
Know exactly what you want?
        │
      YES ──→ v6
        │
      NO
        ↓
Want surprising ideas?
        │
      YES ──→ v6-wild
        │
      NO
        ↓
v6-mini for rapid exploration
```

### Discovery loop

```text
v6-wild
  ↓
find an unusual hook / groove / texture / arrangement
  ↓
identify the useful musical property
  ↓
rebuild deliberately in v6
  ↓
edit / replace / remaster
```

---

# 3. MODEL MIGRATION AND RETIRED MODELS

Suno's current V6 FAQ states that pre-V6 models have been retired for new creation. Existing songs remain available and unchanged; they can still be listened to, shared, remastered, and covered. New iterations use current V6-family models.

Existing custom models are automatically upgraded so V6 powers the custom model going forward. Songs made previously with older custom models remain available and are not rewritten.

### Migration rule

Never assume a V5/V5.5 tutorial is a V6 instruction manual.

When importing an older technique:

1. Recreate the same prompt.
2. Keep the lyrics unchanged.
3. Keep the model fixed.
4. Keep slider values fixed.
5. Generate multiple trials.
6. Record what changed.
7. Keep only techniques that survive V6 testing.

---

# 4. CREATION MODES: SIMPLE VS CUSTOM

## Simple Mode

Simple Mode is the natural-language route. V6 can infer the appropriate creation/editing workflow from the request and can work with multiple supported references in a single creative direction.

Use it when the goal matters more than controlling every UI field.

### Simple prompt architecture

```text
WHAT IT IS
+ HOW IT SHOULD FEEL
+ VOCAL IDENTITY
+ IMPORTANT INSTRUMENTS
+ ARRANGEMENT ARC
+ PRODUCTION CHARACTER
+ IMPORTANT CONSTRAINT
```

Example:

```text
Dark emotional electropop about realizing you caused the breakup. Intimate low-register male vocal, dry close verses, tense rising pre-chorus, enormous bittersweet melodic chorus, warm analog synths, tight electronic drums, controlled sub bass, layered harmonies, modern polished production. Keep the verses sparse so the chorus feels dramatically larger.
```

## Custom Mode

Use Custom Mode when the song needs deliberate separation of:

- lyrics
- Style
- section direction
- structural tags
- controlled experiments
- repeated A/B tests

### Recommended Custom workflow

```text
Lyrics first
↓
Style identity second
↓
Section cues third
↓
Slider configuration
↓
Generate two candidates
↓
Score them
↓
Change ONE variable
↓
Generate again
```

---

# 5. STYLE PROMPT ENGINEERING

A Style prompt should describe **audible behavior**, not merely adjectives.

## High-value dimensions

1. Genre
2. Subgenre
3. Era / production family
4. Vocal type
5. Vocal delivery
6. Tempo / groove
7. Drum behavior
8. Bass behavior
9. Harmonic character
10. Instrument palette
11. Arrangement density
12. Dynamic arc
13. Texture
14. Spatial character
15. Mix priorities
16. Emotional trajectory

### Strong

```text
Dark electropop, intimate low-register male vocal, restrained verses, rising pre-choruses, huge melodic chorus, punchy electronic drums, controlled sub bass, warm analog synth pads, bright arpeggiator accents, stacked chorus harmonies, dry close vocal, wide chorus image, restrained reverb, clean low-mid separation, emotionally devastating but controlled.
```

### Weak

```text
Amazing professional beautiful cinematic high quality emotional catchy cool song.
```

### Prompt compression

If a prompt becomes bloated, remove duplicate adjectives before removing musical identity.

```text
sad + heartbreaking + melancholic + somber
```

can become:

```text
dark melancholic and emotionally devastating
```

---

# 6. VOCAL ENGINEERING

Describe vocals in dimensions that can be heard:

```text
REGISTER
TEXTURE
DELIVERY
DISTANCE
EMOTIONAL INTENSITY
HARMONY
PHRASING
DENSITY
```

### Useful vocabulary

**Register:** low, baritone, tenor, alto, high, head voice, chest-dominant.

**Texture:** breathy, husky, raspy, clean, grainy, intimate, resonant, airy, metallic, warm.

**Delivery:** conversational, restrained, urgent, detached, pleading, whispered, explosive, rhythmic, legato, clipped.

**Distance:** close-mic, intimate, dry, room-like, distant, washed, front-and-center.

**Harmony:** doubles, thirds, octave, stacked harmony, call-and-response, gang vocal, choir-like layer.

### Vocal direction hierarchy

If the vocal is wrong, fix identity before polishing effects:

```text
Vocal type
↓
Register
↓
Delivery
↓
Emotion
↓
Harmony
↓
Spatial character
```

### Common failure

Too many vocal adjectives can conflict. Prefer a coherent identity:

```text
intimate husky low-register male vocal with restrained conversational delivery
```

rather than ten contradictory vocal descriptors.

---

# 7. LYRIC ENGINEERING

Lyrics influence more than meaning. They provide material that the model interprets alongside musical direction.

## Structural labels

Useful labels include:

```text
[Intro]
[Verse 1]
[Pre-Chorus]
[Chorus]
[Post-Chorus]
[Verse 2]
[Bridge]
[Breakdown]
[Build]
[Drop]
[Instrumental]
[Solo]
[Final Chorus]
[Outro]
```

Treat labels as **guidance**, not deterministic code.

## Section-level direction

Good:

```text
[Verse 1 | intimate vocal | sparse drums | restrained delivery]
```

Risky overload:

```text
[Verse 1 | exact EQ | exact compressor ratio | exact LUFS | exact stereo position | exact reverb decay | exact dB level | exact transient response]
```

Use Suno for musical direction. Do not pretend a lyric tag is a DAW automation lane.

## Chorus engineering

A strong chorus generally needs:

- a central hook
- repeatable phrasing
- melodic emphasis
- increased energy
- enough space for the hook to be heard
- some relationship to the verse without becoming identical

## Bridge engineering

A bridge can create contrast through:

- harmony
- instrumentation
- rhythm
- perspective
- vocal intensity
- density
- texture
- lyrical revelation

---

# 8. CREATIVE SLIDERS

Suno documents three major creative controls:

## Weirdness

**Safe → Chaos**.

Think of Weirdness as a controlled move away from the most expected interpretation.

Practical test matrix:

| Weirdness | Use |
|---|---|
| Low | Reliable, conventional result |
| Mid | Balanced exploration |
| High | Unusual arrangements / textures |
| Very high | Discovery and controlled chaos |

Suno's documentation describes **50%** as the normal midpoint.

## Style Influence

**Loose → Strong**.

Use stronger influence when the supplied style identity needs to remain dominant. Use looser influence when you want the model to reinterpret the concept.

## Audio Influence

This appears when working from an audio upload. It controls how strongly the uploaded audio should influence the result.

### Slider testing rule

Never change Weirdness, Style Influence, and Audio Influence simultaneously when diagnosing a problem. Otherwise you cannot know which control caused the change.

---

# 9. VARIETY

Suno's current V6 FAQ states that the **Variety** slider changes/updates style prompts to introduce more variety in outputs.

If you need maximum control over supplied Style tags, set **Variety to 0**.

### Practical interpretation

```text
Variety 0
→ preserve supplied style direction as much as possible

Higher Variety
→ permit more variation / reinterpretation of style direction
```

This is not the same control as Weirdness. Test them independently.

---

# 10. MAX MODE

Max Mode tells V6 to spend more on getting the generation right and costs more credits.

Suno specifically recommends Max Mode for:

- songs longer than two minutes
- covers where staying close to the original matters
- style transfer
- keeping vocals consistent across a full track
- maintaining style consistency across a longer generation

### Standard vs Max

```text
Quick idea / short experiment → Standard
Longer / consistency-sensitive / close-cover task → Max
```

Do not waste Max Mode on every throwaway experiment.

---

# 11. MULTIMODAL INPUTS AND REFERENCES

Current V6 documentation says supported workflows can use multiple references including:

- Suno songs
- Suno playlists
- audio uploads
- images
- video

V6 can interpret the desired feeling, instrumentation, structure, references, and overall direction.

## Reference strategy

Do not throw many unrelated references into one request and expect perfect prioritization.

Instead explain the role of each reference:

```text
Reference A → vocal character
Reference B → drum groove
Reference C → synth texture
Reference D → overall emotional atmosphere
```

Then state what must remain original.

---

# 12. AUDIO UPLOADS

Audio can be used as a source for creative transformation and reference-driven workflows.

### Practical preparation

Before uploading:

- trim irrelevant silence
- use the cleanest source available
- avoid unnecessary clipping
- identify the important section
- know whether you want rhythm, melody, timbre, performance, or overall vibe preserved

If the audio is meant to be a vocal source, a clean vocal/acapella-style recording is generally preferable when available.

### Audio-reference test

Run:

```text
Low Audio Influence
Medium Audio Influence
High Audio Influence
```

while holding every other variable constant.

---

# 13. VOICES

Voices allow a creator to use a recorded/uploaded voice as part of Suno creation.

Current Suno materials say Voices replaced the old top-level Personas entry in the Create menu, while Style Personas remain available inside Voices.

Voice verification uses a displayed phrase and compares the spoken recording with the uploaded vocal recording.

### Voice quality checklist

- record in a quiet environment
- avoid room echo
- avoid clipping
- use a clean vocal recording when possible
- keep pronunciation clear during verification
- test Audio Influence when trying to preserve the voice character

### Rights rule

Only use voices you have the right to use. Do not treat voice cloning as permission to imitate a person you do not have authorization to use.

### Important compatibility warning

Suno's current documentation has historically changed Voice/model compatibility as the feature evolved. Always verify the current model picker and current Voices help article before treating a model-compatibility statement as permanent.

---

# 14. CUSTOM MODELS

Current Suno documentation says Pro/Premier users can create up to **three private Custom Models** using at least **six songs** they own the rights to. Bulk Upload is supported. Model creation is described as taking roughly **2–5 minutes**.

Custom Models are private and cannot be shared between users.

## Dataset strategy

The model is only as useful as the music used to teach it.

Prefer a coherent dataset when the goal is consistency:

```text
same artist identity
same production philosophy
same vocal identity
same genre family
same era / aesthetic
```

Avoid a random six-song dataset if the goal is a recognizable personal sound.

### Dataset checklist

```text
✓ Own all rights
✓ At least 6 tracks
✓ Consistent identity
✓ Good source quality
✓ Representative examples
✓ Avoid accidental unrelated material
```

---

# 15. MY TASTE / PERSONALIZATION

Personalization features can affect how Suno approaches a creator's preferred sound.

Treat personalization as a **global preference layer**, not a substitute for a precise Style prompt.

For controlled experiments:

1. Keep personalization state constant.
2. Change only the prompt variable being tested.
3. Record the state alongside the generation.

If comparing two prompts, do not change the prompt and personalization at the same time.

---

# 16. INSPIRE / LYRICIST

Current Suno creation tools include personalization and lyric-writing assistance such as Inspire and Lyricist.

### Lyricist strategy

Use saved examples as references for:

- tone
- imagery
- cadence
- emotional vocabulary
- structural habits

Do not assume a reference guarantees stylistic copying. Treat it as guidance.

### Human-in-the-loop lyric workflow

```text
AI draft
↓
human selects strongest lines
↓
human removes clichés
↓
human strengthens hook
↓
human checks narrative continuity
↓
Suno performance generation
↓
edit only what failed
```

---

# 17. SUNO SOUNDS

Suno Sounds is an experimental/beta creation area for generating audio assets such as:

- one-shots
- loops
- sound effects
- instrument samples
- ambient sounds

Loops can include BPM direction.

### Use Sounds for

- transitions
- risers
- impacts
- atmosphere
- custom percussion
- texture layers
- unusual instrument samples

Do not assume every generated Sound is a full-song asset; treat it as a production component.

---

# 18. SAMPLING / ISOLATION

V6 supports workflows where a creator can sample or isolate material and build a new musical result around it.

Useful mental model:

```text
SOURCE
↓
IDENTIFY USEFUL MOMENT
↓
ISOLATE / SAMPLE
↓
DESCRIBE DESIRED NEW CONTEXT
↓
GENERATE
↓
EDIT / ARRANGE
```

When sampling material, keep rights and permissions in mind.

---

# 19. MASHUP

V6 can combine multiple source elements in a single request.

A powerful approach is to assign each source a role:

```text
Source 1 → vocals
Source 2 → drums
Source 3 → guitar texture
Source 4 → harmonic atmosphere
```

Then specify the desired destination:

```text
Combine the vocal character of Source 1 with the rhythmic foundation of Source 2, use Source 3 as a texture, and rebuild the arrangement as dark modern electropop.
```

Avoid vague instructions like:

```text
Mix these songs together.
```

Tell Suno **what to take from what**.

---

# 20. EXTEND

Use Extend when a song contains a section worth continuing.

### Best use cases

- continue an unfinished song
- add a final chorus
- create an outro
- extend an instrumental
- repair a song that ends too early

### Extension strategy

Describe the intended next section rather than simply saying "continue":

```text
Continue into a larger final chorus with expanded harmonies, additional percussion and a stronger emotional lift, then resolve into a short atmospheric outro.
```

---

# 21. CROP

Crop is the opposite of extending: remove unwanted material and preserve the useful section.

Use Crop before rebuilding when the source contains:

- a bad intro
- an unwanted ending
- an accidental section
- excess silence
- a weaker passage around an otherwise strong performance

Think:

```text
Crop = preserve the good material before further processing.
```

---

# 22. REUSE PROMPT

Reuse Prompt is valuable for controlled iteration because it preserves the creative setup so you can modify only the variable you want to test.

### Example

Generation A:

```text
Style = dark electropop
Weirdness = 40
Style Influence = 70
```

Generation B:

```text
Same everything
Weirdness = 55
```

This is much more informative than rewriting the entire prompt from scratch.

---

# 23. SONG EDITOR / NATURAL-LANGUAGE EDITING

V6 introduces natural-language editing workflows capable of making targeted changes to existing songs.

The core principle is:

```text
Preserve what works.
Change only what is requested.
```

### Good edit request

```text
Keep the verse, instrumentation and vocal performance unchanged. Replace only the chorus with a larger melodic chorus featuring stacked harmonies and stronger drums.
```

### Bad edit request

```text
Make the whole song better.
```

The second request changes too many degrees of freedom.

---

# 24. SINGLE-LYRIC EDITING

V6 supports changing one lyric or line without rebuilding the entire song.

Use this for:

- correcting a word
- fixing a name
- changing a phrase
- correcting a typo
- replacing a lyric that is emotionally wrong

This is one of the most important **surgical editing** principles in V6: do not regenerate an entire song when only one line is wrong.

---

# 25. REPLACE SECTION

Replace Section is the surgical repair tool.

### Rescue workflow

```text
FULL SONG
↓
identify defective section
↓
replace only that section
↓
compare old/new transition
↓
keep the strongest result
```

### Replacement request anatomy

```text
SECTION: [which section]
KEEP: [what must remain consistent]
CHANGE: [what is wrong]
TARGET: [desired replacement behavior]
```

Example:

```text
Replace only the final chorus. Keep the lead vocal identity and harmonic progression. Increase the emotional intensity, add stacked harmonies and wider synths, and preserve the existing tempo and overall song identity.
```

---

# 26. ADD VOCALS

Add Vocals is designed for adding vocal material to existing musical content.

Use it when the instrumental is already strong and the missing element is the vocal layer.

### Practical workflow

```text
Strong instrumental
↓
define vocal identity
↓
provide lyric/performance direction
↓
add vocal
↓
inspect timing and phrasing
↓
edit / stem-process if needed
```

Do not attempt to solve an arrangement problem by adding more vocals.

---

# 27. REMASTER

Remaster should be treated as a **version-selection tool**, not a magic quality button.

Compare:

- vocal clarity
- transient definition
- low-end control
- harshness
- stereo image
- balance
- emotional character
- artifacts

Keep the original if the remaster damages something important.

### A/B rule

Never decide a remaster is better because it is simply louder. Match perceived loudness before judging.

---

# 28. ADVANCED STEM SEPARATION

Suno's current advanced stem tooling includes multiple separation levels.

The current documented capabilities include:

- **Auto Split** — broad multi-category separation.
- **Split from Mix** — isolate a selected element against the remainder.
- **Advanced Split** — much finer instrument-level separation, with nearly 100 instruments documented for Premier.

### Stem rescue workflow

```text
Song
↓
Advanced Stem Separation
↓
identify defective stem
↓
mute / replace / process
↓
rebalance
↓
export
```

Stems are especially useful when generation is good overall but one component is problematic.

---

# 29. STUDIO 2.0

Suno Studio 2.0 is a browser-based production environment for Premier subscribers.

It adds:

- MIDI
- piano roll
- musical typing
- external MIDI input
- wavetable synth
- automation
- built-in effects
- custom plugins
- Studio Chat
- advanced stem separation
- recording
- Take Lanes
- clip editing
- exports

### Environment

Current Suno documentation recommends Google Chrome. Studio requires a desktop, laptop or tablet with at least **768px screen width**; mobile devices are not supported. Minimum hardware requirements include CPU SIMD support (SSE4.1 or Neon) and at least 4 GB RAM.

Safari currently does not support Web MIDI in Studio.

---

# 30. STUDIO CHAT

Studio Chat is a natural-language collaborator inside Studio and is currently described as beta in Suno's Studio documentation.

It can be used to:

- generate audio clips
- generate instruments
- generate vocals
- arrange material
- design custom plugins
- design synth presets
- ask project questions
- tidy sessions

### Better Chat requests

Give Studio a task, musical context, and constraints:

```text
Create an 8-bar warm analog synth bass line at the project's tempo. Keep it sparse during the verse and leave space for the kick and lead vocal.
```

Avoid ambiguous commands when timing matters.

---

# 31. STUDIO MIDI

Studio 2.0 supports MIDI tracks and a piano roll.

### MIDI capabilities

- import MIDI
- record MIDI
- edit notes
- draw notes
- move/resize notes
- quantize
- change velocity
- adjust pitch bend
- adjust modulation
- use musical typing
- use chord mode
- use arpeggiator
- connect external MIDI hardware through Web MIDI
- generate audio from MIDI
- transcribe audio into MIDI in supported workflows

### MIDI mental model

```text
MIDI = instructions for notes
Audio = recorded/generated sound
```

This distinction makes MIDI useful for changing the instrument without recreating the musical performance.

---

# 32. AUDIO ↔ MIDI

Studio supports workflows where audio can be placed onto a MIDI track for transcription into notes, and MIDI can be used to generate an audio cover/result.

Use this when you want to extract the musical skeleton of an existing part and then change its sound or develop it further.

### Typical workflow

```text
Audio riff
↓
Audio → MIDI
↓
edit notes
↓
change instrument
↓
generate / play new audio
```

Treat automatic transcription as a starting point. Inspect rhythm, pitch, and artifacts.

---

# 33. WAVETABLE SYNTH

Studio's wavetable synth can be used for:

- bass
- leads
- pads
- chords
- textures

The synth can be controlled through MIDI and can use Chat to help design presets.

### Synth design vocabulary

```text
oscillator
wavetable position
filter
resonance
envelope
attack
decay
sustain
release
LFO
modulation
unison
detune
stereo width
saturation
```

Use these terms when asking Studio Chat for a deliberately designed synth patch.

---

# 34. STUDIO EFFECTS

Current built-in effects include:

- Compressor
- EQ
- Reverb
- Convolution
- Delay
- Distortion
- Gate

Effects operate in ordered chains.

### Chain principle

```text
SOURCE
↓
EQ
↓
COMPRESSOR
↓
DISTORTION / SATURATION
↓
DELAY
↓
REVERB
```

This is only an example. Order changes the sound.

### Sidechain

Studio's current product materials include sidechain compression. Use it for controlled ducking such as:

```text
kick → ducks bass
vocal → ducks competing music
```

### Important limitation

Studio is **not compatible with conventional VST or Audio Units plugins**. Use built-in effects, custom Studio plugins, or export to a conventional DAW when third-party plugin formats are required.

---

# 35. CUSTOM STUDIO PLUGINS

Studio Chat can design custom effects from natural-language descriptions.

Example:

```text
Build a warm tape saturation effect with gentle compression, subtle pitch wobble, and a controllable mix parameter. Keep it musical rather than heavily distorted.
```

The resulting plugin can be saved, revised conversationally, and used like Studio effects.

### Plugin iteration

```text
Build
↓
listen
↓
identify one problem
↓
ask for one change
↓
listen again
```

Do not request ten changes at once when diagnosing the effect.

---

# 36. STUDIO AUTOMATION

Automation changes track or plugin parameters over time.

Examples:

- volume swells
- pan movement
- filter sweeps
- reverb throws
- delay changes
- effect intensity
- transitions

MIDI Learn can connect compatible hardware controls to Studio parameters.

### Automation principle

Static mix:

```text
parameter = one value
```

Dynamic mix:

```text
parameter = function of time
```

Automation is how a production evolves instead of remaining static.

---

# 37. STUDIO RECORDING

Studio can record audio and MIDI clips onto the timeline when compatible hardware/input is available.

Use recording for:

- vocals
- instruments
- scratch tracks
- MIDI performance
- replacement parts

### Recording checklist

```text
Input selected
↓
levels checked
↓
monitoring checked
↓
metronome/tempo confirmed
↓
record
↓
inspect timing
↓
choose take
```

---

# 38. TAKE LANES

Studio 2.0 uses Take Lanes to hold alternate generated versions.

This is useful because generation naturally creates alternatives.

### Take-selection strategy

Score each take for:

1. hook
2. vocal performance
3. timing
4. arrangement
5. emotional impact
6. artifacts
7. transition quality

Do not automatically choose the first generation.

---

# 39. CLIP EDITING

Studio's arrangement editor can be used to inspect and edit clips on the timeline.

Use it for:

- arranging sections
- trimming
- timing adjustments
- working with audio clips
- editing MIDI clips
- creating transitions

For major musical changes, use Suno's generative tools first; for precise timeline changes, use Studio editing.

---

# 40. REMOVE FX / GET DRY

Studio includes a Remove FX workflow that uses AI to strip baked-in effects such as reverb and delay from audio.

This is useful when:

```text
source vocal has too much reverb
↓
Get Dry
↓
process clean-ish source
↓
add controlled new effects
```

Treat the result as processed audio rather than assuming perfect mathematical recovery of the original dry recording.

---

# 41. STUDIO LIBRARY

Studio includes access to the Suno Library through its interface.

This supports moving between:

- songs
- liked material
- stems
- uploads
- workspaces
- Studio projects

Use the Library as the source of truth for moving existing Suno material into Studio.

---

# 42. STUDIO EXPORT

Current Studio documentation says Studio can export:

- full songs
- selected ranges
- multitrack projects
- individual stems

Studio supports 32-bit WAV and MP3 export paths, with individual stems available as WAV.

Suno's Studio 2.0 announcement also describes Premier Studio export of high-quality **32-bit / 48 kHz** multitracks and stems without the normal download limitations.

### Export strategy

For archival / further production:

```text
Prefer WAV
↓
Prefer multitrack/stems when further mixing is planned
↓
Keep original project
↓
Create final delivery master separately
```

Use MP3 for convenient listening copies rather than as the preferred archival master.

---

# 43. DOWNLOADS, CREDITS AND PLAN LIMITS

Current Suno download documentation describes different monthly/lifetime download limits by plan and distinguishes normal song downloads from Studio workflows.

Current documented figures include:

- Free: up to 7 lifetime trial downloads for personal/non-commercial use.
- Pro: 20 downloads per month.
- Premier: 60 downloads per month.

The current download documentation states that the counter resets on the billing date and does not roll over. Re-downloading the same song does not count as another download, and multiple formats of the same song count as one download. Stems count as part of the song's download. Failed/interrupted downloads do not count.

Studio workflows are not affected by the normal song-download counter.

### Credit economy

Suno's current V6 FAQ states that standard V6 generations have the same credit cost as previous models: each generation produces two songs for 10 credits. Large numbers of images/videos in prompts can increase cost.

Max Mode costs more credits.

---

# 44. COMMERCIAL RIGHTS / TERMS

Always distinguish:

```text
Suno's stated rights to your generated output
        ≠
permission to use someone else's copyrighted input
        ≠
ownership of every underlying musical idea
        ≠
legal copyright protection in every jurisdiction
```

Suno's current terms/update materials state that songs downloaded under paid plans retain commercial rights according to Suno's terms, while free-trial downloads are not commercially eligible.

**Always consult the current Suno Terms of Service for the exact legal language before relying on a commercial-rights conclusion.**

### Rights checklist

Before commercial release:

- verify the plan under which the song was generated
- verify the song was eligible for commercial use under current terms
- verify rights to uploaded audio
- verify rights to Custom Model training material
- verify rights to voices used
- verify third-party samples/references
- verify cover/remix permissions
- retain project/export records

---

# 45. COVER / REMIX / PUBLISH PERMISSIONS

Publishing a song and allowing other users to Remix or Cover it are separate choices from merely keeping it private.

If a song containing your Voice is shared/published with remix/cover permissions enabled, other creators may be able to create derivative Suno works that include the voice according to Suno's current sharing rules.

Review Publish options carefully before enabling remix/cover access.

---

# 46. COVER ART AND VISUALS

Suno's current product updates include iterative cover-art generation from images and text prompts, with image or video output in supported web workflows.

Use iterative visual prompting the same way you use musical prompting:

```text
Base image
↓
identify one change
↓
edit
↓
verify unchanged elements
↓
repeat
```

Do not request a dozen unrelated visual changes at once if preserving identity is important.

---

# 47. PRODUCTION VOCABULARY FOR SUNO PROMPTING

Translate technical production goals into audible language.

| Production goal | Prompt language |
|---|---|
| Strong transient attack | punchy, defined transients |
| Soft attack | rounded, gentle transient |
| Low-end separation | clean kick-bass separation |
| Vocal presence | forward, intimate vocal |
| Less room | dry, close vocal |
| More space | open, spacious, controlled ambience |
| Wider chorus | wide stereo image |
| Dense chorus | layered, full arrangement |
| Contrast | sparse verse, expanded chorus |
| Smooth top end | silky, controlled highs |
| Aggressive sound | saturated, driven, gritty |
| Dynamic performance | preserved dynamics |
| Pumping | sidechain-driven movement |
| Tight drums | controlled, punchy percussion |

### Do not confuse prompt language with post-production controls

Saying "-14 LUFS" does not guarantee that Suno will produce an exact -14 LUFS master. Exact engineering specifications should be measured and corrected in Studio or a DAW.

---

# 48. MIX / MASTER PROMPTING

Prompt for **character**, not impossible measurement precision.

### Good

```text
Clean controlled low end, vocal-forward mix, punchy kick, defined snare transient, restrained reverb, wide but stable chorus, smooth highs, preserved dynamic contrast.
```

### Less useful

```text
Exactly -14.0 LUFS, exactly -1 dBTP, exactly 3.2 ms attack, exactly 4.7:1 compression ratio.
```

Use precise numeric engineering inside a production tool that actually exposes those controls.

---

# 49. REPEATABILITY / SAME CHORUS

Suno is generative. Identical instructions do not guarantee identical audio.

When consistency matters, use:

- the same model
- the same source
- the same lyrics
- the same Style
- the same slider values
- the same references
- the same editing path
- surgical section replacement rather than full regeneration

### Same-hook strategy

```text
Create best chorus
↓
keep strongest version
↓
use it as the reference for later work
↓
replace only surrounding sections when possible
```

Do not expect a regenerated chorus to be sample-identical merely because the words are identical.

---

# 50. PROMPT FAILURE MODES

## Prompt soup

Too many genres produce unclear identity.

## Contradictory instructions

Example:

```text
minimal sparse arrangement + huge dense wall of sound throughout
```

## Adjective overload

```text
beautiful amazing professional epic cinematic emotional catchy powerful incredible
```

## Solving mixing problems in lyrics

A lyric field is not a full DAW mixer.

## Too many exclusions

A prompt dominated by "no / don't / avoid" can become less useful than a positive description of the desired result.

## Changing everything at once

You lose the ability to learn what caused the improvement.

## Overusing Max Mode

Use it when the task benefits from the additional cost.

## Trusting one generation

Generative music requires comparison.

---

# 51. SCIENTIFIC SUNO TESTING

Treat prompt engineering like an experiment.

## Controlled variables

Record:

```text
Model
Lyrics
Style
Weirdness
Style Influence
Audio Influence
Variety
Max Mode
References
Input audio
Generation date
```

## One-variable test

```text
A = baseline
B = one change
C = same change repeated
```

If B improves and C also improves, confidence increases.

## Replication rule

Never promote a one-off lucky generation into a "guaranteed technique."

---

# 52. A/B TESTING FRAMEWORK

Score generations from 1–10 for:

| Dimension | Question |
|---|---|
| Identity | Does it sound like the intended genre/artist identity? |
| Vocal | Is the vocal right? |
| Hook | Is the main idea memorable? |
| Arrangement | Does the song develop? |
| Dynamics | Is there useful contrast? |
| Mix | Is the balance acceptable? |
| Artifacts | Are there obvious defects? |
| Emotion | Does it communicate the intended feeling? |
| Originality | Does it avoid generic output? |
| Editability | Is there enough good material to rescue? |

### Decision rule

A technically cleaner version is not automatically the better artistic version.

---

# 53. PRODUCTION RESCUE WORKFLOW

When a generation is 80–90% right, **do not automatically regenerate from zero**.

```text
BAD FULL SONG?
      │
      ↓
Identify what is actually wrong
      │
      ├── One lyric → single lyric edit
      ├── One section → Replace Section
      ├── Ending → Crop / Extend
      ├── Voice → Voice / Add Vocals workflow
      ├── One instrument → stems / Studio
      ├── Mix issue → Studio effects
      ├── Baked effects → Get Dry
      └── Overall polish → Remaster
```

Then:

```text
Stems
↓
Studio
↓
Automation / EQ / compression / reverb
↓
Export multitrack or master
```

This is usually more efficient than repeatedly regenerating an almost-correct song.

---

# 54. MASTER V6 CREATION WORKFLOW

```text
01. DEFINE THE SONG'S PURPOSE
02. DEFINE GENRE / EMOTION / VOCAL IDENTITY
03. WRITE OR REFINE LYRICS
04. BUILD A CLEAN STYLE PROMPT
05. CHOOSE v6 / v6-wild / v6-mini
06. SET CREATIVE CONTROLS
07. GENERATE MULTIPLE CANDIDATES
08. SCORE THE CANDIDATES
09. SELECT THE BEST FOUNDATION
10. CROP UNWANTED MATERIAL IF NEEDED
11. EXTEND STRONG SECTIONS IF NEEDED
12. REPLACE DEFECTIVE SECTIONS
13. FIX SINGLE LYRICS SURGICALLY
14. REMASTER IF THE VERSION BENEFITS
15. SEPARATE STEMS IF PRODUCTION REPAIR IS NEEDED
16. OPEN IN STUDIO
17. EDIT / ARRANGE
18. ADD MIDI / SYNTH PARTS IF NEEDED
19. APPLY EFFECTS
20. AUTOMATE
21. RECORD REPLACEMENT PARTS IF NEEDED
22. CHECK TIMING
23. CHECK ARTIFACTS
24. EXPORT WAV / MULTITRACK / STEMS
25. ARCHIVE THE SOURCE AND SETTINGS
```

---

# 55. SUNO + CHATGPT MASTER WORKFLOW

Use ChatGPT as the **planning / analysis / writing layer**, not as a pretend Suno control API.

### Stage 1 — creative brief

Give ChatGPT:

```text
Genre
Emotion
Story
Vocal identity
Reference mood
Desired song arc
Hard constraints
```

### Stage 2 — lyric engineering

Ask for:

- hook alternatives
- verse progression
- bridge purpose
- syllable/cadence review
- cliché detection
- emotional escalation

### Stage 3 — Suno prompt

Have ChatGPT convert the brief into:

```text
Style prompt
Lyrics
Section cues
Slider test plan
```

### Stage 4 — generation

Generate multiple candidates.

### Stage 5 — evidence

Tell ChatGPT what actually happened.

Do not tell it that a prompt "worked" if you only generated one example.

### Stage 6 — controlled revision

Change one variable and repeat.

---

# 56. GENRE PROMPT COOKBOOK

## Dark Electropop

```text
Dark modern electropop, intimate low-register male vocal, sparse nocturnal verses, rising tension, huge melodic chorus, warm analog synths, punchy electronic drums, controlled sub bass, glossy arpeggiators, layered harmonies, dry close vocal, wide chorus, restrained reverb, polished but emotionally raw.
```

## Synthwave

```text
Cinematic synthwave, nostalgic analog synthesizers, pulsing bass sequence, gated electronic drums, neon-night atmosphere, expressive lead vocal, wide stereo pads, dramatic builds, melodic instrumental hook, controlled low end, polished retro-modern production.
```

## Indie Pop

```text
Intimate indie pop, conversational lead vocal, organic guitar textures, understated drums, warm bass, subtle synth atmosphere, memorable melodic hook, dynamic verse-to-chorus expansion, human imperfections, close vocal presence, restrained ambience.
```

## Cinematic Pop

```text
Emotional cinematic pop, intimate opening, piano and atmospheric textures, gradual orchestral expansion, deep percussion, large melodic chorus, layered vocals, dramatic harmonic lift, wide stereo image, controlled low end, spacious but clear mix.
```

## Alternative Rock

```text
Dark alternative rock, gritty expressive vocal, distorted electric guitars, live-feeling drums, driving bass, dynamic verses, explosive chorus, dramatic guitar texture, raw emotional delivery, wide guitars, punchy center vocal, controlled saturation.
```

---

# 57. MUSIC-PRODUCTION GLOSSARY FOR SUNO USERS

**Transient** — the initial attack of a sound.

**Dynamics** — changes in loudness/energy over time.

**Stereo width** — perceived left/right spread.

**Low end** — bass and sub-bass region.

**Low-mid buildup** — excessive energy in the lower middle frequencies that can make a mix feel muddy.

**Saturation** — nonlinear coloration that adds harmonics and perceived density.

**Compression** — dynamic-range control.

**Sidechain compression** — one signal controls compression of another, often kick → bass.

**Reverb** — simulated or processed acoustic space.

**Delay** — time-based repetition.

**Gate** — reduces signal below a threshold, often useful for noise/tightness.

**EQ** — frequency-selective boosting/cutting.

**Convolution reverb** — reverb based on an impulse response representing a space or system.

**LUFS** — loudness measurement standard. Do not assume prompting an exact LUFS value guarantees that measurement.

**True peak** — estimate of peak level including inter-sample behavior.

**Phase** — timing/polarity relationship between signals; phase problems can reduce clarity or mono compatibility.

**Mono compatibility** — how well a stereo mix survives being collapsed to mono.

**Crest factor** — relationship between peaks and average signal level; useful when discussing punch/dynamics.

---

# 58. STUDIO KEYBOARD SHORTCUTS

Current Studio documentation lists shortcuts including:

| Action | Shortcut |
|---|---|
| Record | **Shift-R** |
| Play / Stop | **Spacebar** |
| Metronome | **Shift-C** |
| Loop | **Cmd-L** |

Suno's Studio documentation also references soloing an instrument with **Shift-S** when checking timing issues.

Shortcut availability can change. Verify the current Studio shortcut reference if a shortcut stops working.

---

# 59. STUDIO TIMING TROUBLESHOOTING

If a generated clip appears slightly early or late:

1. Turn on the metronome.
2. Solo the relevant track.
3. Compare transients against the grid.
4. Check project tempo.
5. Inspect the clip placement.
6. Correct the arrangement before exporting.

Suno has acknowledged that some Studio generations may exhibit timing offsets and recommends rigorous timing checks.

---

# 60. COMPATIBILITY MATRIX

| Feature | v6 | v6-wild | v6-mini | Custom Model | Studio |
|---|---|---|---|---|---|
| Core generation | ✓ | ✓ | ✓ | ✓ | — |
| Experimental discovery | Good | **Best** | Good | Depends | — |
| Long generation | Up to 8 min | Up to 8 min | Up to 8 min | Varies by current model support | — |
| Custom training | — | — | — | **✓** | — |
| Studio production | Can edit in Studio | Can edit in Studio | Can edit in Studio | Can open supported songs | **✓** |
| MIDI | — | — | — | — | **✓** |
| Automation | — | — | — | — | **✓** |
| Built-in effects | — | — | — | — | **✓** |

**Important:** compatibility is feature-specific and can change. Always verify the current model picker/help documentation for Voice, Custom Model, My Taste and other model-sensitive tools before treating this table as permanent.

---

# 61. FEATURE / EVIDENCE MATRIX

| Area | Evidence status |
|---|---|
| v6 / v6-wild / v6-mini | **OFFICIAL** |
| 8-minute V6 generation ceiling | **OFFICIAL** |
| V6 multimodal references | **OFFICIAL** |
| Variety behavior | **OFFICIAL** |
| Max Mode purpose | **OFFICIAL** |
| Studio 2.0 MIDI | **OFFICIAL** |
| Studio effects | **OFFICIAL** |
| Studio custom plugins | **OFFICIAL** |
| Studio automation | **OFFICIAL** |
| Advanced stems | **OFFICIAL** |
| Custom Models | **OFFICIAL** |
| Sounds | **OFFICIAL / EXPERIMENTAL PRODUCT AREA** |
| Exact prompt syntax guarantees | **UNKNOWN / NOT GUARANTEED** |
| Deterministic section tags | **NOT GUARANTEED** |
| Exact numeric mix results from natural-language prompts | **NOT GUARANTEED** |
| Identical output from identical prompt | **NOT GUARANTEED** |
| Community prompt hacks | **COMMUNITY / EXPERIMENTAL** |

---

# 62. WHAT NOT TO CLAIM

Never state any of the following as guaranteed unless current Suno documentation explicitly supports it:

- secret prompt commands
- hidden token syntax
- deterministic seeds
- exact vocal cloning from arbitrary material
- exact BPM adherence in every generation
- exact key adherence in every generation
- exact LUFS or dB compliance from prompt text
- guaranteed same melody from repeated generation
- guaranteed identical singer from descriptive text alone
- guaranteed instrument isolation without artifacts
- guaranteed preservation of every part during editing

The guide should prefer:

> **“This can help / has been observed / is documented”**

over:

> **“This always works.”**

---

# 63. TROUBLESHOOTING DECISION TREE

```text
RESULT IS BAD
│
├─ Entire song wrong?
│   ├─ Wrong genre → revise Style
│   ├─ Wrong vocal → revise vocal identity / Voice workflow
│   ├─ Wrong arrangement → revise structure / Style
│   └─ Wrong model behavior → test another V6-family model
│
├─ One section wrong?
│   └─ Replace Section
│
├─ One word wrong?
│   └─ Single lyric edit
│
├─ Ending wrong?
│   ├─ Crop
│   └─ Extend
│
├─ One instrument wrong?
│   └─ Stems / Studio
│
├─ Too much reverb/delay?
│   └─ Get Dry / Studio effects
│
├─ Mix balance wrong?
│   └─ Studio EQ / compressor / effects / automation
│
├─ Need different instrument but same notes?
│   └─ MIDI workflow
│
└─ Need final polish?
    └─ Remaster → Studio → external DAW if necessary
```

---

# 64. CURRENT RELEASE-TRACKING CHECKLIST

When maintaining this guide, check these first:

1. V6 FAQ
2. Current Models
3. Model Switching
4. Making Music help category
5. Studio 2.0 category
6. Release Notes
7. Terms / downloads documentation
8. Voices documentation
9. Custom Models documentation
10. Creative Sliders documentation

Then audit the guide for:

```text
new feature
changed UI
new model
changed plan availability
changed credit cost
changed download limits
changed licensing language
changed compatibility
new Studio feature
retired feature
new release note
```

---

# 65. LIVING-KNOWLEDGE-BASE MAINTENANCE PROTOCOL

Every significant Suno update should produce an audit.

### Audit steps

```text
1. Record update date
2. Read official release note
3. Read affected help article
4. Identify changed claims
5. Mark old behavior RETIRED if appropriate
6. Update plan/availability tables
7. Update examples
8. Re-test important workflows
9. Mark community techniques that are now obsolete
10. Update source index
```

### Version discipline

Every section should be mentally answerable as:

> **“Was this true on the guide's current reference date?”**

If not, label it historical or remove it.

---

# 66. OFFICIAL CURRENT REFERENCE LIBRARY

Use official Suno sources as the primary authority:

- V6 FAQ: https://help.suno.com/en/articles/13924481
- Current V6 Models: https://help.suno.com/en/articles/13924737
- Model Switching: https://help.suno.com/en/articles/13924993
- Studio 2.0: https://help.suno.com/en/articles/13670529
- Studio 2.0 category: https://help.suno.com/en/categories/2701953-studio-2-0
- Audio Effects / Plugins: https://help.suno.com/en/articles/13670785
- Custom Models: https://help.suno.com/en/articles/11362497
- Voices FAQ: https://help.suno.com/en/articles/11362433
- Creative Sliders: https://help.suno.com/en/articles/6141377
- Suno release notes: https://suno.com/release-notes
- V6 release notes: https://suno.com/release-notes/introducing-v6
- Studio 2.0 release notes: https://suno.com/release-notes/studio-2
- Studio 2.0 announcement: https://suno.com/blog/studio-2

---

# 67. FINAL V6 PRINCIPLES

```text
1. Define the sound before prompting.
2. Use V6 for control.
3. Use V6-WILD for discovery.
4. Use V6-MINI for rapid iteration.
5. Keep Style identity coherent.
6. Use lyrics for story and performance direction.
7. Use section cues for local behavior.
8. Treat tags as guidance, not code.
9. Test sliders independently.
10. Use Variety 0 when retaining supplied style tags matters.
11. Use Max Mode where consistency and length justify the cost.
12. Preserve good material instead of regenerating everything.
13. Use surgical editing for local defects.
14. Use stems for component-level repair.
15. Use Studio for production control.
16. Use MIDI when notes—not audio—need to remain editable.
17. Use automation for movement over time.
18. Use Get Dry when baked-in effects are the problem.
19. Export stems/multitracks when further production is planned.
20. Keep rights and plan status documented.
21. Separate official facts from community discoveries.
22. Never turn a lucky generation into a fake guarantee.
23. Change one variable at a time when learning.
24. Listen critically; do not judge only from prompt quality.
25. Archive the best source, not just the final MP3.
```

---

# 68. SOURCE-OF-TRUTH RULE

For any conflict:

```text
CURRENT OFFICIAL SUNO DOCUMENTATION
        ↓
CURRENT SUNO RELEASE NOTES
        ↓
REPRODUCIBLE TESTING
        ↓
RELIABLE COMMUNITY REPORTS
        ↓
OLD TUTORIALS / SCREENSHOTS
```

The newest authoritative source wins unless the guide explicitly documents a reproducible current behavior that Suno has not yet documented.

---

# 69. COMPLETENESS STANDARD

This addendum is considered part of the guide's **ALL / EVERYTHING** scope only when each claim is treated according to its evidence level and current date.

The objective is not to create the longest possible document by stuffing it with speculation.

The objective is:

> **The broadest current, useful, evidence-labeled Suno V6 knowledge base possible without inventing information.**

That is what **ALL** and **EVERYTHING** mean here.
