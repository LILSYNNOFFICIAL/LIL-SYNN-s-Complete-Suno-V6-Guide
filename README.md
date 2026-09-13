# 🎵 SUNO EVERYTHING GUIDE

### The Complete Suno Creation, Prompting, Editing & Production Knowledge Base

<p align="center">
  <strong>Everything Suno. One evolving knowledge base.</strong><br>
  Prompts • Lyrics • Styles • Models • Controls • Editing • Stems • Production • Advanced Techniques
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Suno-V6-black?style=for-the-badge">
  <img src="https://img.shields.io/badge/Prompting-Advanced-8A2BE2?style=for-the-badge">
  <img src="https://img.shields.io/badge/Music%20Production-AI-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/Status-Work%20in%20Progress-orange?style=for-the-badge">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Documentation-Expanding-lightgrey?style=flat-square">
  <img src="https://img.shields.io/badge/Techniques-Continuously%20Updated-success?style=flat-square">
  <img src="https://img.shields.io/badge/Models-V6%20%7C%20Future%20Models-black?style=flat-square">
</p>

---

## 🔗 QUICK NAVIGATION

<p align="center">
  <a href="#-about-this-repository">About</a> •
  <a href="#-suno-models">Models</a> •
  <a href="#-lyrics-box">Lyrics Box</a> •
  <a href="#-style-box">Style Box</a> •
  <a href="#-prompt-engineering">Prompt Engineering</a> •
  <a href="#-advanced-creative-controls">Creative Controls</a> •
  <a href="#-creation-tools">Creation Tools</a> •
  <a href="#-editing-tools">Editing</a> •
  <a href="#-stems--production">Stems</a> •
  <a href="#-vocal-direction">Vocals</a> •
  <a href="#-instrumentation--arrangement">Arrangement</a> •
  <a href="#-genre-fusion">Genre Fusion</a> •
  <a href="#-production--sonic-direction">Production</a> •
  <a href="#-troubleshooting">Troubleshooting</a> •
  <a href="#-iteration-strategy">Iteration</a> •
  <a href="#-prompt-library">Prompt Library</a> •
  <a href="#-experimental-techniques">Experimental Techniques</a>
</p>

---

## 🎯 ABOUT THIS REPOSITORY

This repository is intended to become a comprehensive, continuously expanding knowledge base for **Suno** and AI-assisted music creation.

The goal is not simply to document buttons or explain basic generation.

The goal is to understand how Suno actually responds to instructions, how its different controls interact, how prompting affects musical interpretation, how to control vocals and instrumentation, how to edit existing generations, and how to push the system toward increasingly specific creative results.

This repository will contain practical techniques, tested prompts, examples, workflows, experiments, production strategies, editing methods, troubleshooting information, and discoveries made through real-world use.

The repository is designed to evolve alongside Suno.

As new models, tools, controls, editing capabilities, and prompting behaviors appear, this documentation will be expanded and updated.

---

## 🧠 WHAT THIS REPOSITORY COVERS

Suno is much more than a text-to-song generator.

A complete Suno workflow can involve the **Lyrics Box**, **Style Box**, audio references, creative controls, model selection, generation modes, editing tools, stems, remixing, sampling, covers, personalization, and iterative refinement.

The interaction between these systems is often more important than any individual setting.

The general creation pipeline can be thought of as:

```text
LYRICS
   +
STYLE
   +
AUDIO / IMAGE / VIDEO / REFERENCES
   ↓
CREATIVE CONTROLS
   ↓
CREATION OPERATION
   ↓
GENERATION
   ↓
LISTEN
   ↓
EDIT / REMIX / EXTEND / REPLACE
   ↓
REFINE
   ↓
FINAL SONG
```

The objective of this repository is to document each layer independently and then explain how they work together.

---

# 🎛️ SUNO MODELS

Suno's model system is important because the model determines how instructions are interpreted and how the resulting music behaves.

## SUNO V6

V6 is Suno's flagship generation model.

It is designed for greater musical nuance, stronger interpretation of natural-language instructions, improved control, and more sophisticated generation and editing capabilities.

V6 can work with text, audio, images, and video inputs depending on the workflow.

It can also perform more targeted modifications to existing songs rather than requiring an entirely new generation for every change.

V6 supports generation of songs up to approximately eight minutes.

V6 is intended for users who want greater control and more polished musical results.

## V6-WILD

V6-WILD is an experimental variation of V6.

The purpose of a more unpredictable model is not maximum obedience.

It is useful when exploration, surprise, unusual arrangements, unexpected transitions, unconventional instrumentation, or less predictable interpretations are desirable.

A highly controlled workflow and a highly experimental workflow should therefore not necessarily use the same model.

## V6-MINI

V6-MINI is the lighter and faster V6 option.

It is useful for experimentation, rapid iteration, testing ideas, and users who do not require the full capabilities of the flagship model.

## MODEL SELECTION STRATEGY

A practical approach is:

```text
V6
↓
Precision
Control
Polish
Detailed prompting

V6-WILD
↓
Experimentation
Unexpected ideas
Creative exploration
Controlled chaos

V6-MINI
↓
Fast testing
Rapid iteration
Lightweight generation
```

Model choice should be treated as part of the creative workflow rather than as an afterthought.

---

# ✍️ LYRICS BOX

The Lyrics Box controls the lyrical content and provides an important layer of structural and performance information.

Lyrics should not always be treated as nothing more than words.

Formatting, section labels, contextual instructions, vocal cues, repetition, pacing indicators, and arrangement hints can influence how Suno interprets the song.

A simple lyric structure might look like:

```text
[Intro]

[Verse 1]
Lyrics...

[Pre-Chorus]
Lyrics...

[Chorus]
Lyrics...

[Verse 2]
Lyrics...

[Bridge]
Lyrics...

[Final Chorus]

[Outro]
```

The Lyrics Box will eventually have its own dedicated prompting system in this repository.

Future documentation will cover techniques for communicating:

```text
Vocal delivery
Emotional intensity
Section transitions
Backing vocals
Harmonies
Call and response
Ad-libs
Whispers
Spoken passages
Screams
Breathy vocals
Layered vocals
Instrumental breaks
Dynamic changes
Arrangement cues
Outro behavior
```

The Lyrics Box should be considered both a **lyrical input** and a potential **structural communication layer**.

---

# 🎨 STYLE BOX

The Style Box is where musical identity is communicated.

A Style prompt can describe characteristics such as:

```text
Genre
Subgenre
Era
Tempo
Mood
Instrumentation
Vocal character
Production style
Mix characteristics
Song structure
Performance style
Energy
Dynamics
Atmosphere
Recording aesthetic
```

A basic style description might be:

```text
Emotional electropop, cinematic synth-pop, intimate male vocals,
dark atmospheric production, warm analog synthesizers,
punchy electronic drums, wide chorus, restrained verses,
dramatic final chorus, polished modern production.
```

The Style Box should generally describe **what the music should sound like**, while the Lyrics Box communicates the **song's words and structural context**.

The distinction is not absolute, but maintaining separation between musical identity and lyrical content generally makes complex prompting easier to reason about.

---

# 🧬 STYLE PROMPT STRUCTURE

A useful Style prompt can be organized conceptually as:

```text
[GENRE]
+
[ERA / REFERENCE]
+
[VOCAL CHARACTER]
+
[INSTRUMENTATION]
+
[ARRANGEMENT]
+
[PRODUCTION]
+
[MOOD]
+
[DYNAMICS]
```

Example:

```text
Alternative electropop with early-2000s synth-pop influence,
intimate emotional male lead vocal, dark warm synthesizers,
punchy electronic drums, deep controlled bass,
minimal verses that expand into a huge melodic chorus,
layered harmonies, atmospheric textures,
cinematic tension, polished modern mix,
melancholic but powerful emotional delivery.
```

This structure provides multiple dimensions for Suno to interpret instead of relying on a single genre label.

---

# 🧠 PROMPT ENGINEERING

Prompt engineering for Suno is fundamentally about communicating musical intent.

A prompt can be technically detailed while still producing poor results if the information is contradictory, redundant, or poorly prioritized.

The objective is not to write the longest possible prompt.

The objective is to provide the **right information in a useful hierarchy**.

A useful conceptual hierarchy is:

```text
CORE GENRE
↓
SONIC IDENTITY
↓
VOCAL IDENTITY
↓
INSTRUMENTATION
↓
ARRANGEMENT
↓
PRODUCTION
↓
EMOTIONAL DIRECTION
↓
SPECIFIC DETAILS
```

For example:

```text
Dark emotional electropop
with cinematic synth-pop influence,
intimate restrained male vocals,
warm analog synths and deep sub bass,
tight electronic drums,
minimal verses,
expansive melodic choruses,
layered harmonies,
wide atmospheric production,
strong emotional escalation,
polished modern mix.
```

Specificity is useful when it communicates something meaningful.

Over-specification can become counterproductive when the instructions conflict with one another.

---

# 🎚️ ADVANCED CREATIVE CONTROLS

Suno's creative controls influence how strongly the system follows or explores different aspects of the supplied material.

These controls should be understood as interacting variables rather than independent magic switches.

## VARIETY

Variety controls how much variation is introduced into the generation.

A lower Variety setting is useful when maintaining stronger control over the supplied style direction is important.

At or near zero, the style instructions are given maximum consistency.

Higher Variety can produce more divergence and unexpected interpretations.

Conceptually:

```text
VARIETY 0
↓
Maximum stylistic consistency
Less exploration

VARIETY HIGH
↓
More variation
More exploration
Greater unpredictability
```

Variety can be particularly useful when the objective changes from **reproduction** to **discovery**.

## WEIRDNESS

Weirdness controls the degree of creative unpredictability.

The scale can be thought of as:

```text
SAFE ←──────────────→ CHAOS
```

Around 50% represents the normal midpoint.

Lower values generally favor safer interpretations.

Higher values encourage more unusual outcomes.

Weirdness is particularly useful when intentionally experimenting with unconventional arrangements, melodies, transitions, or sonic combinations.

## STYLE INFLUENCE

Style Influence controls how strongly Suno follows the supplied Style direction.

Conceptually:

```text
LOOSE ←──────────────→ STRONG
```

Lower settings allow greater interpretation.

Higher settings push the generation more strongly toward the supplied style description.

A high Style Influence setting can therefore be useful when the Style Box contains carefully designed musical instructions.

## AUDIO INFLUENCE

Audio Influence appears when an audio reference is supplied.

It controls how strongly the supplied audio influences the resulting generation.

When preserving characteristics of an uploaded reference is important, stronger Audio Influence can be useful.

Conceptually:

```text
LOW
↓
More reinterpretation

HIGH
↓
Stronger relationship to source audio
```

Audio Influence should not automatically be set to maximum for every situation.

The correct setting depends on whether the objective is **transformation** or **preservation**.

## PERSONALIZATION

Personalization can incorporate established user preferences into the generation experience.

It can be useful when the goal is to incorporate a recognizable personal musical taste.

It can also be undesirable during highly controlled experiments where unrelated preferences could influence the result.

For surgical testing, eliminating unnecessary variables can make results easier to evaluate.

## MAX MODE

Max Mode is intended for situations where additional generation capability is worth the additional cost.

Suno specifically describes it as useful for longer songs, covers where closeness matters, style transfer, and situations where consistent vocals or style are important.

A practical workflow is:

```text
TESTING
↓
Normal generation
↓
Identify strongest direction
↓
KEEPER GENERATION
↓
Max Mode when appropriate
```

Max Mode should not automatically be treated as "better" for every generation.

It is a tool for specific situations.

---

# 🔗 HOW THE CONTROLS INTERACT

The most important concept is that the controls do not operate in isolation.

A useful mental model is:

```text
LYRICS
   +
STYLE
   +
AUDIO / REFERENCE
   ↓
VARIETY
PERSONALIZATION
WEIRDNESS
STYLE INFLUENCE
AUDIO INFLUENCE
MAX MODE
   ↓
CREATION OPERATION
   ↓
RESULT
```

Changing one variable can change how another instruction is perceived.

For example, an extremely strong Style Influence combined with high Weirdness may create a result that is simultaneously highly stylistic and highly unpredictable.

Likewise, a strong Audio Influence combined with low Variety may be appropriate when attempting to remain close to a reference.

The correct workflow is therefore to change variables deliberately rather than randomly changing every slider after every generation.

---

# 🛠️ CREATION TOOLS

Suno's creation tools allow existing musical material to become the starting point for new generations.

The major concepts include:

```text
Create
Cover
Extend
Inspo
Mashup
Sample
Edit Vocals
Edit Instruments
Replace Section
Add Stem
```

Each operation solves a different problem.

---

# 🔄 COVER

Cover is intended for significant transformations of an existing song while retaining important elements of its identity.

It is useful when the goal is something like:

```text
Same song
+
Different genre
+
Different instrumentation
+
Different vocal interpretation
```

Cover should generally be used when the desired transformation affects the overall musical interpretation.

For smaller changes, editing tools may be more appropriate.

---

# ➕ EXTEND

Extend continues an existing song.

It is useful for:

```text
Adding another verse
Creating a longer outro
Building a new bridge
Continuing an instrumental
Expanding the arrangement
```

Extend is fundamentally a continuation operation rather than a complete reinterpretation.

---

# 💡 INSPO

Inspo is useful when the objective is to create something inspired by a musical direction rather than directly editing a specific existing section.

It can function as a starting point for:

```text
Genre exploration
Mood exploration
Production exploration
Song concept development
```

---

# 🔀 MASHUP

Mashup combines two songs into a new generation.

This can be used to explore relationships between:

```text
Different genres
Different arrangements
Different melodies
Different vocal ideas
Different production styles
```

Mashup should be treated as a creative recombination tool rather than simply a blending effect.

---

# 🎵 SAMPLE

Sample takes a selected portion of an existing song and uses it as a creative jumping-off point.

This can be particularly useful when a song contains a:

```text
Riff
Groove
Melodic fragment
Instrumental section
Interesting texture
Rhythmic idea
```

Sample is therefore useful for extracting a creative idea without necessarily rebuilding the entire original song.

---

# 🧩 ADD STEM

Add Stem and Get Stems should not be confused.

**Add Stem** is a generative layer operation.

It can be used to add another musical component to an existing production.

Conceptually:

```text
Existing Song
+
Generated Instrument / Musical Layer
=
Expanded Arrangement
```

---

# 🎚️ EDITING TOOLS

Editing should be used surgically whenever possible.

If only one part of a song is wrong, rebuilding the entire song may unnecessarily change parts that were already successful.

A practical decision tree is:

```text
VOCAL PROBLEM
→ Edit Vocals

INSTRUMENT PROBLEM
→ Edit Instruments

ONE BAD SECTION
→ Replace Section

NEED MORE SONG
→ Extend

REMOVE PART
→ Remove Section

WHOLE INTERPRETATION NEEDS TO CHANGE
→ Cover

COMBINE TWO SONGS
→ Mashup

USE A SPECIFIC MUSICAL FRAGMENT
→ Sample

QUICK SONIC POLISH
→ Remaster
```

This is one of the most important concepts in advanced Suno workflows.

**Do not rebuild what can be surgically repaired.**

---

# ✂️ REPLACE SECTION

Replace Section is designed for modifying a specific part of a song.

Instead of regenerating the entire track, a selected region can be replaced.

This is useful for:

```text
Bad chorus
Weak transition
Wrong instrumental section
Unwanted vocal phrase
Arrangement problem
Performance issue
```

The surrounding song can remain intact while the problematic section is regenerated.

---

# 🎤 EDIT VOCALS

Edit Vocals is intended for vocal-specific modifications.

This is preferable when the instrumental arrangement is already strong but the vocal performance needs adjustment.

Potential use cases include:

```text
Changing vocal delivery
Correcting vocal interpretation
Altering vocal character
Changing a vocal section
Exploring a different vocal performance
```

---

# 🎸 EDIT INSTRUMENTS

Edit Instruments is intended for instrumental-specific changes.

This is useful when:

```text
The vocal is correct
The arrangement is mostly correct
One instrument is wrong
An instrumental section needs changing
The production needs a different musical layer
```

This makes it possible to work on the instrumental without unnecessarily rebuilding the entire vocal performance.

---

# 🎛️ REMASTER

Remaster is primarily a refinement tool.

It is useful for subtle variations and sonic improvements involving areas such as:

```text
Mix balance
Clarity
Polish
Overall sonic presentation
```

Remaster includes a model selector and variation strength options such as:

```text
Subtle
Normal
High
```

Remaster should generally be thought of as **polishing an existing result**, not completely reinventing it.

For major transformations, Cover or other creation tools are more appropriate.

---

# 🎚️ STRENGTH STRATEGY

A useful workflow is:

```text
SUBTLE
↓
Small sonic refinement

NORMAL
↓
Moderate variation

HIGH
↓
More noticeable remaster variation
```

When the song is already excellent, start conservatively.

---

# 🎛️ STEMS & PRODUCTION

Suno can separate songs into individual stems.

Depending on the available functionality, stems can include components such as:

```text
Vocals
Drums
Bass
Guitar
Keys
Other instruments
```

Advanced stem separation can provide a much larger number of instrument choices.

This enables workflows that move beyond Suno generation into traditional production.

A typical workflow can become:

```text
SUNO GENERATION
↓
GET STEMS
↓
SEPARATE COMPONENTS
↓
DAW
↓
MIX
↓
EDIT
↓
MASTER
```

---

# 🧱 GET STEMS VS ADD STEM

These two operations have fundamentally different purposes.

```text
GET STEMS
↓
Extract components from an existing song.

ADD STEM
↓
Generate and add a new musical layer.
```

Understanding this distinction prevents confusion when designing production workflows.

---

# 🎤 VOCAL DIRECTION

Vocals can be described through multiple dimensions.

A useful vocal prompt can communicate:

```text
Gender / vocal range
Age impression
Tone
Texture
Breathiness
Intensity
Emotional state
Phrasing
Articulation
Dynamics
Harmony
Backing vocals
Ad-libs
Whispers
Spoken delivery
```

Instead of:

```text
Male singer.
```

A more descriptive direction might be:

```text
Intimate emotional male lead vocal,
restrained and vulnerable in the verses,
gradually increasing intensity through the pre-chorus,
full expressive delivery in the chorus,
breathy close-mic character,
subtle layered harmonies,
restrained ad-libs,
emotionally cracked delivery during the final chorus.
```

The goal is to communicate performance rather than simply identify a singer category.

---

# 🎼 INSTRUMENTATION & ARRANGEMENT

Instrumentation should describe not only which instruments exist, but how they behave.

For example:

```text
Warm analog synth pad
+
Muted electronic kick
+
Deep controlled sub bass
+
Sparse verse percussion
+
Expanding pre-chorus texture
+
Wide layered chorus synths
+
Additional counter-melody in final chorus
```

Arrangement can be communicated through progression:

```text
Minimal intro
↓
Sparse verse
↓
Growing pre-chorus
↓
Wide chorus
↓
Reduced second verse
↓
Larger second chorus
↓
Instrumental bridge
↓
Maximum-energy final chorus
↓
Stripped outro
```

This gives Suno a musical trajectory rather than a static instrument list.

---

# 🔥 DYNAMICS

One of the most useful concepts in advanced prompting is contrast.

A song becomes more emotionally effective when different sections have different energy levels.

A prompt might communicate:

```text
Restrained verses,
gradually increasing tension,
explosive melodic chorus,
brief breakdown,
then an even larger final chorus.
```

This is generally more useful than simply saying:

```text
Very emotional and powerful.
```

Dynamic instructions communicate **when** the energy should change.

---

# 🌌 ATMOSPHERE

Atmosphere can be communicated using combinations of:

```text
Dark
Warm
Cold
Dreamlike
Cinematic
Intimate
Expansive
Claustrophobic
Ethereal
Nostalgic
Mechanical
Organic
Lo-fi
Polished
Raw
Futuristic
Vintage
```

Atmosphere becomes more effective when paired with concrete sonic characteristics.

For example:

```text
Dark intimate atmosphere
with warm analog synthesizers,
soft room ambience,
deep sub bass,
close vocal recording,
and a wide cinematic chorus.
```

---

# 🧬 GENRE FUSION

Genre fusion works best when the roles of the genres are clear.

Instead of:

```text
Pop rock hip hop EDM country jazz metal.
```

Use a hierarchy:

```text
Core genre:
Alternative electropop

Secondary influence:
2000s synth-pop

Rhythmic influence:
Modern electronic pop

Atmospheric influence:
Cinematic ambient

Vocal influence:
Emotional indie-pop
```

This gives the generation a center of gravity.

Genre fusion should feel intentional rather than like a random collection of tags.

---

# 🏗️ GENRE FUSION TEMPLATE

```text
PRIMARY GENRE:
[core identity]

SECONDARY GENRE:
[major influence]

RHYTHMIC INFLUENCE:
[groove / drum influence]

INSTRUMENTAL INFLUENCE:
[instrument palette]

VOCAL INFLUENCE:
[vocal character]

PRODUCTION INFLUENCE:
[sonic aesthetic]

EMOTIONAL DIRECTION:
[emotional target]
```

Example:

```text
Primary genre: cinematic electropop
Secondary influence: alternative synth-pop
Rhythmic influence: modern electronic pop
Instrumental influence: analog synthesizers and atmospheric guitar
Vocal influence: intimate emotional male vocal
Production influence: polished wide modern mix
Emotional direction: melancholic, vulnerable, escalating into catharsis
```

---

# 🎚️ PRODUCTION & SONIC DIRECTION

Production prompts can describe the final sonic presentation.

Useful dimensions include:

```text
Mix width
Stereo image
Bass depth
Vocal placement
Drum punch
Compression character
Reverb
Delay
Analog warmth
Digital precision
Lo-fi texture
High-frequency clarity
Low-end control
Mastering intensity
```

A production description might be:

```text
Wide modern stereo image,
tight controlled low end,
punchy electronic drums,
warm analog synth character,
intimate centered lead vocal,
subtle stereo ambience,
layered chorus vocals,
clean high-frequency detail,
polished commercial master without excessive loudness.
```

---

# 🧪 EXPERIMENTAL PROMPTING

Experimental prompting should be treated as controlled experimentation.

Change one meaningful variable at a time when trying to determine what actually affects the result.

For example:

```text
Generation A
Variety: 0
Weirdness: 30
Style Influence: 90

Generation B
Variety: 0
Weirdness: 50
Style Influence: 90
```

If B produces a dramatically different result, Weirdness becomes a more plausible explanation than changing five settings simultaneously.

This approach makes experimentation reproducible.

---

# 🔬 A/B TESTING

A/B testing is useful for determining whether a prompt or setting actually improves a result.

Keep as many variables identical as possible.

```text
TEST A
Same lyrics
Same model
Same Style
Same audio
Different Weirdness

TEST B
Same lyrics
Same model
Same Style
Same audio
Different Weirdness
```

Avoid changing:

```text
Model
Lyrics
Style
Audio
Variety
Weirdness
Style Influence
Audio Influence
```

all at the same time if the goal is to learn which variable caused the difference.

---

# 🔁 ITERATION STRATEGY

Advanced Suno creation is often iterative.

The first generation does not necessarily need to be the final song.

A productive workflow is:

```text
IDEA
↓
FIRST GENERATION
↓
IDENTIFY WHAT WORKS
↓
IDENTIFY WHAT FAILS
↓
SURGICAL EDIT
↓
GENERATE AGAIN
↓
COMPARE
↓
KEEP BEST VERSION
↓
REFINE
```

The most important habit is to preserve successful elements.

Do not destroy a great vocal because the snare is wrong.

Do not rebuild a great chorus because the bridge needs work.

Do not replace an entire song when one section can be regenerated.

---

# 🎯 SURGICAL EDITING PHILOSOPHY

Think of each Suno operation as a tool with a specific scope.

```text
SONG LEVEL
→ Cover
→ Mashup
→ Sample
→ Inspo

SECTION LEVEL
→ Replace Section
→ Extend
→ Remove Section

VOCAL LEVEL
→ Edit Vocals

INSTRUMENT LEVEL
→ Edit Instruments
→ Add Stem

SONIC REFINEMENT
→ Remaster

COMPONENT EXTRACTION
→ Get Stems
```

The smaller the problem, the smaller the tool that should be used.

This principle minimizes unnecessary changes.

---

# 🧠 PROMPT PRIORITY

When instructions conflict, not every instruction should be treated as equally important.

A practical hierarchy is:

```text
CORE MUSICAL IDENTITY
↓
SONG STRUCTURE
↓
VOCAL IDENTITY
↓
INSTRUMENTATION
↓
PRODUCTION
↓
DETAILS
```

If the prompt says:

```text
Minimal intimate production
```

and later says:

```text
Massive orchestral wall of sound
```

the model has conflicting instructions.

Better prompting removes contradictions.

---

# 🧹 PROMPT CLEANUP

Before generating, inspect the prompt for:

```text
Contradictions
Repeated instructions
Unnecessary genre stacking
Unclear vocal direction
Conflicting tempo descriptions
Conflicting production aesthetics
Too many unrelated influences
```

A shorter coherent prompt can outperform a longer contradictory one.

---

# 📚 PROMPT LIBRARY

This repository will eventually contain reusable prompts organized by purpose.

Future categories can include:

```text
Pop
Electropop
Synth-pop
Indie
Alternative
Rock
Hip-hop
R&B
Soul
EDM
House
Techno
Metal
Country
Acoustic
Cinematic
Ambient
Experimental
Dark Pop
Dream Pop
Hyperpop
Ballads
Soundtracks
```

Additional prompt libraries will cover:

```text
Male vocals
Female vocals
Duets
Choirs
Whisper vocals
Aggressive vocals
Emotional vocals
Layered vocals
Backing vocals
Harmony design
Instrumental tracks
Cinematic arrangements
Retro production
Modern production
Lo-fi production
High-fidelity production
```

---

# ✍️ FUTURE LYRICS BOX PROMPT LIBRARY

A dedicated section will eventually document techniques for controlling the Lyrics Box.

This will include examples for:

```text
Section behavior
Vocal delivery
Ad-libs
Harmony cues
Call and response
Whisper sections
Spoken sections
Instrumental breaks
Dynamic escalation
Repeated hooks
Outro behavior
Vocal layering
Emotional transitions
```

The goal is to develop a repeatable language for communicating performance and arrangement intent through lyrics formatting.

---

# 🎨 FUTURE STYLE BOX TECHNIQUES

A dedicated Style Box section will eventually document reusable frameworks for:

```text
Genre definition
Genre fusion
Vocal identity
Instrumentation
Arrangement
Production
Mix characteristics
Atmosphere
Dynamics
Era references
Recording aesthetics
Emotional direction
```

The repository will distinguish between **generic prompt theory** and **tested practical techniques** whenever possible.

---

# 🧪 EXPERIMENTAL TECHNIQUES

Experimental techniques will be documented separately from established workflows.

This distinction matters.

A technique that produces interesting results once should not automatically be presented as guaranteed behavior.

Experimental documentation should identify:

```text
What was attempted
What inputs were used
What settings were used
What happened
Whether the result was repeatable
What limitations were observed
```

This creates a useful experimental record instead of turning speculation into "Suno facts."

---

# 🛠️ TROUBLESHOOTING

When a generation is bad, diagnose the problem before changing everything.

Ask:

```text
Was the model appropriate?

Was the Style prompt clear?

Was the Lyrics structure clear?

Was the audio reference appropriate?

Was Variety too high?

Was Weirdness too high?

Was Style Influence too low?

Was Audio Influence too low?

Was Personalization influencing the result?

Would a different operation be more appropriate?

Does the problem affect the entire song or only one section?
```

The answer determines the next action.

---

# 🚨 COMMON MISTAKE: CHANGING EVERYTHING

A common failure mode is:

```text
Bad generation
↓
Change model
↓
Rewrite lyrics
↓
Rewrite Style
↓
Change all sliders
↓
Upload new audio
↓
Generate again
```

At that point it becomes impossible to know what actually solved the problem.

A better workflow is:

```text
Identify ONE problem
↓
Change ONE meaningful variable
↓
Generate
↓
Compare
↓
Continue
```

---

# 🎯 CONTROLLED COVER WORKFLOW

For a cover where maintaining the source identity is important, a practical starting point can be:

```text
MODEL:
V6

VARIETY:
0%

STYLE INFLUENCE:
85–95%

AUDIO INFLUENCE:
90–100%

WEIRDNESS:
30–40%

PERSONALIZATION:
OFF when strict source control is desired

MAX MODE:
Use when the final generation requires it
```

These are **practical starting recommendations**, not guaranteed or official magic settings.

The correct values depend on the source material and desired transformation.

---

# 🎚️ CONTROLLED GENERATION WORKFLOW

A controlled generation can follow:

```text
1. Choose V6.

2. Establish the core genre.

3. Define the vocal identity.

4. Define instrumentation.

5. Define arrangement.

6. Define production.

7. Set Variety according to the desired amount of exploration.

8. Set Weirdness according to the desired amount of unpredictability.

9. Set Style Influence according to how strongly the Style prompt should dominate.

10. Set Audio Influence when an audio reference is being used.

11. Decide whether Personalization should contribute.

12. Generate.

13. Identify the strongest result.

14. Surgically edit problems instead of rebuilding unnecessarily.

15. Remaster only after the underlying musical result is correct.

16. Extract stems when moving into external production.
```

---

# 🧠 THE SUNO CREATION MATRIX

The entire system can be understood as several layers.

```text
┌──────────────────────────────────────┐
│              INPUTS                  │
│ Lyrics • Style • Audio • References  │
└──────────────────┬───────────────────┘
                   ↓
┌──────────────────────────────────────┐
│          CREATIVE CONTROLS           │
│ Variety • Weirdness • Style Influence│
│ Audio Influence • Personalization    │
│ Max Mode                              │
└──────────────────┬───────────────────┘
                   ↓
┌──────────────────────────────────────┐
│             OPERATION                │
│ Create • Cover • Extend • Inspo      │
│ Mashup • Sample • Edit • Replace     │
│ Add Stem                             │
└──────────────────┬───────────────────┘
                   ↓
┌──────────────────────────────────────┐
│              RESULT                  │
│          Generated Music              │
└──────────────────┬───────────────────┘
                   ↓
┌──────────────────────────────────────┐
│          REFINEMENT                  │
│ Edit • Replace • Extend • Remaster   │
│ Get Stems • Export • Production      │
└──────────────────────────────────────┘
```

This model is useful because it separates **what you provide**, **how strongly you want it interpreted**, **what operation you are performing**, and **what you do afterward**.

---

# 📈 ITERATIVE CREATION LOOP

The advanced workflow is ultimately a loop:

```text
CREATE
↓
LISTEN
↓
ANALYZE
↓
IDENTIFY PROBLEM
↓
SELECT APPROPRIATE TOOL
↓
EDIT
↓
LISTEN AGAIN
↓
COMPARE
↓
KEEP / REJECT
↓
REFINE
```

This is fundamentally different from repeatedly pressing Generate and hoping for a better song.

---

# 🧪 DOCUMENTATION STANDARD

Whenever possible, experimental techniques in this repository should distinguish between:

**VERIFIED**

Behavior documented by Suno or consistently observed through testing.

**PRACTICAL**

A technique that has proven useful but should not be treated as an official rule.

**EXPERIMENTAL**

A technique that produces interesting results but requires additional testing.

**SPECULATIVE**

A hypothesis about why a behavior occurs that has not been adequately verified.

This prevents the repository from becoming a collection of unsupported claims.

---

# 📌 ACCURACY POLICY

Suno changes rapidly.

Features, models, controls, credit behavior, interfaces, and generation capabilities can change over time.

This repository should therefore avoid presenting temporary interface behavior as permanent fact.

Official Suno documentation should be preferred when documenting confirmed functionality.

Practical prompting techniques should be labeled as techniques rather than official Suno behavior.

Screenshots and interface observations should be treated as time-specific evidence.

---

# 🚀 FUTURE EXPANSION

This repository is intentionally incomplete.

Future additions will expand into:

```text
Advanced Lyrics Box prompting
Advanced Style Box prompting
Genre-specific prompt libraries
Vocal prompt libraries
Instrument prompt libraries
Arrangement templates
Production templates
Song structure templates
Cover workflows
Remix workflows
Mashup workflows
Sample workflows
Stem workflows
Custom model workflows
Personalization workflows
Audio-reference workflows
Image-reference workflows
Video-reference workflows
Prompt testing methodology
A/B testing
Advanced editing strategies
DAW workflows
Mastering workflows
Troubleshooting databases
Community-tested prompts
```

The objective is for this repository to become a living reference rather than a static tutorial.

---

# 🔗 OFFICIAL SUNO RESOURCES

## Suno V6 Announcement

https://suno.com/release-notes/introducing-v6

## V6 FAQ

https://help.suno.com/en/articles/13924481

## Current Suno Models

https://help.suno.com/en/articles/13924737

## What's New in V6

https://help.suno.com/en/articles/13924801

## Changing Models

https://help.suno.com/en/articles/13924993

## Creative Sliders

https://help.suno.com/en/articles/6141377

## Song Editor

https://help.suno.com/en/articles/6141505

## Stems

https://help.suno.com/en/articles/13925185

## Remaster

https://help.suno.com/en/articles/8105281

## Sample & Mashup

https://suno.com/release-notes/meet-our-new-create-features-sample-mashup

## Song Length

https://help.suno.com/en/articles/13924929

## Custom Models

https://help.suno.com/en/articles/11362497

---

# 🧭 REPOSITORY PHILOSOPHY

Suno is not simply a button that generates a song.

It is a layered creative system.

The strongest results come from understanding the relationship between:

```text
Lyrics
+
Style
+
References
+
Creative Controls
+
Models
+
Creation Operations
+
Editing
+
Iteration
+
Production
```

The purpose of this repository is to document that entire ecosystem.

Not just **what Suno can do**.

But **how to use it deliberately**.

---

# 🎵 EVERYTHING SUNO

This repository will continue expanding as Suno evolves.

New models will be documented.

New controls will be tested.

New prompting techniques will be added.

New editing workflows will be developed.

New discoveries will be separated from confirmed behavior.

The ultimate goal is simple:

```text
UNDERSTAND THE SYSTEM
        ↓
CONTROL THE GENERATION
        ↓
REFINE THE RESULT
        ↓
MAKE BETTER MUSIC
```

**Suno is the instrument.**

**Prompting is the language.**

**Iteration is the workflow.**

**Production is the finish.**

And this repository is intended to document all of it.
