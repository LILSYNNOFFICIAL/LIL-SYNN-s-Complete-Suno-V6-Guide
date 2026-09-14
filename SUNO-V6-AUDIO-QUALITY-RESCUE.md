# 🎧 SUNO V6 — AUDIO QUALITY RESCUE / REFERENCE RECREATION FIX

> **Operational note — September 2026**
>
> Use this controlled setup when V6 produces unexpectedly poor audio quality from a source/reference and the goal is to preserve the original performance while improving the resulting audio quality.

---

## 1. THE CONTROLLED RESCUE SETUP

Use **V6 Mini** and isolate the test. Do not add unrelated options while diagnosing the audio problem.

```text
MODEL
→ V6 Mini

SOURCE
→ Select the song as a Cover
→ Select the entire song from Sample

WEIRDNESS
→ 0%

STYLE INFLUENCE
→ 86%

AUDIO INFLUENCE
→ 86%

OTHER OPTIONS
→ Nothing else enabled
```

Keep Personalize off for this diagnostic pass and select the required male/female vocal setting when applicable.

---

## 2. LYRICS BOX — `[SND]` DIRECTION

Put the following structure direction in the **Lyrics box**:

```text
[SND]
recreate the original audio exactly as sung and performed, identical vocal timbre phrasing dynamics intensity and emotion, identical instrument playing style technique feel and arrangement, identical overall musical energy and mood
```

The `[SND]` line is the explicit structure direction for this workflow. Do not silently replace it with an unrelated tag or invent additional control syntax.

---

## 3. STYLE BOX — FULL AUDIO-QUALITY PROMPT

Put the complete prompt below in the **Style box**:

```text
recreate the original audio exactly as sung and performed, identical vocal timbre phrasing dynamics intensity and emotion, identical instrument playing style technique feel and arrangement, identical overall musical energy and mood, ultra-professional studio mastering, lossless hi-fi, reference-grade mix, 24-bit digital clean, dynamic range 12dB+, wide cinematic stereo imaging, crystal-clear highs, high quality bass, perfectly balanced mids, zero mud, zero muddiness, zero low-end buildup, zero artifacts, zero compression artifacts, zero digital hiss, zero clipping, no frequency pollution, no resonance, no phase issues, fully transparent final master, radio broadcast quality, concert hall clarity, warm analog depth + razor-sharp digital precision, present lead vocals, wide and airy soundstage, high-fidelity studio production, crisp transients, layered instruments with clear separation, stable tonal balance and loudness
```

**Do not shorten this prompt during the rescue test.** The controlled test depends on the complete preservation/performance instruction and the complete audio-quality instruction being present.

---

## 4. EXACT CHECKLIST

| Setting | Required value |
|---|---|
| Model | **V6 Mini** |
| Mode | **Cover** |
| Sample | **Entire song** |
| Weirdness | **0%** |
| Style Influence | **86%** |
| Audio Influence | **86%** |
| Personalize | **OFF** |
| Other options | **Nothing else enabled** |
| Lyrics box | **`[SND]` direction + preservation instruction** |
| Style box | **Complete Audio Quality prompt** |
| Vocal gender | **Male/Female as required** |

---

## 5. WHEN V6 AUDIO SOUNDS BAD

Classify the defect before changing the recipe.

### A. Distortion / clipping / crunchy artifacts

Run the controlled rescue setup first. Do not stack additional mastering language or unrelated style instructions on top of it during the diagnostic pass.

### B. Vocal timbre changed

Verify that the entire source was selected and that the preservation language remains intact. Compare against the original at matched playback level.

### C. Instruments or arrangement drifted

The preservation instruction explicitly calls for the original instrument playing style, technique, feel and arrangement. Do not add new arrangement directions during the rescue test.

### D. Mud / low-end buildup / harshness

The Style-box prompt explicitly addresses mud, muddiness, low-end buildup, frequency pollution, resonance, clipping and related artifacts. Test the complete prompt before changing individual phrases.

### E. Excessive processing / crushed dynamics

Keep Weirdness at 0% and do not enable additional options during the controlled test. The purpose is to isolate the variables rather than create another creative generation.

---

## 6. A/B TESTING RULE

Change one variable at a time.

```text
BAD V6 RESULT
     ↓
CONTROLLED RESCUE SETUP
     ↓
COMPARE AGAINST SOURCE
     ↓
IDENTIFY WHAT IMPROVED / FAILED
     ↓
CHANGE ONE VARIABLE
     ↓
TEST AGAIN
```

Do not judge a rescue generation only by loudness. Compare vocal identity, dynamics, transients, stereo image, low end, high end, artifacts and overall musical energy.

---

## 7. IMPORTANT BOUNDARY

This is a **reproducible operational workaround**, not a claim that `[SND]` is an officially documented Suno programming command. Treat it as a controlled prompt/structure technique and judge it by the resulting audio.

Likewise, descriptive phrases such as “lossless hi-fi,” “24-bit digital clean,” “dynamic range 12dB+,” and “zero clipping” are instructions describing the desired result; they do not guarantee a particular technical export specification from the generation model.

The goal of this workflow is simple:

```text
PRESERVE THE PERFORMANCE
+
PRESERVE THE ARRANGEMENT
+
REDUCE UNWANTED AUDIO DAMAGE
+
DO NOT INTRODUCE NEW CREATIVE VARIABLES
```
