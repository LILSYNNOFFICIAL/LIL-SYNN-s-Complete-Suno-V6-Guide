# 🎧 SUNO V6 — AUDIO QUALITY RESCUE / REFERENCE RECREATION FIX

> **Operational note — September 2026**
> Use this controlled setup when V6 produces unexpectedly poor audio quality from a source/reference and the goal is to preserve the original performance while improving the resulting audio quality.

---

## 1. THE CONTROLLED RESCUE SETUP

**Use V6 Mini. Do not use the other V6 models for this rescue workflow — they can change the result and defeat the controlled test. Use Sample mode, select the entire song for Sample Length, and use the settings below exactly.**

```text
MODEL
→ V6 Mini — REQUIRED
→ Do NOT use V6, V6 Wild, or another model for this rescue workflow

OPERATION / MODE
→ Sample

SAMPLE LENGTH
→ Entire song — select the whole song

WEIRDNESS
→ 0%

STYLE INFLUENCE
→ 85%

AUDIO INFLUENCE
→ 85%

MAX MODE
→ ON

PERSONALIZE
→ OFF

OTHER OPTIONS
→ Nothing else enabled
```

**Do not substitute another model. Do not change these values during the first controlled rescue pass.** Select the required male/female vocal setting when applicable.

---

## 2. LYRICS BOX — LYRICS ONLY

Put **ONLY the original song lyrics** in the **Lyrics box**.

**Do not put `[SND]`, the audio instruction, mastering language, settings, or any other instructions in the Lyrics box.** The Lyrics box contains the song lyrics only.

```text
YOUR ORIGINAL SONG LYRICS ONLY
```

---

## 3. STYLE BOX — FULL AUDIO-QUALITY PROMPT

**This entire prompt goes in the Style box. Do not put it in the Lyrics box. Do not shorten it.**

```text
recreate the original audio exactly as sung and performed, identical vocal timbre phrasing dynamics intensity and emotion, identical instrument playing style technique feel and arrangement, identical overall musical energy and mood, ultra-professional studio mastering, lossless hi-fi, reference-grade mix, 24-bit digital clean, dynamic range 12dB+, wide cinematic stereo imaging, crystal-clear highs, high quality bass, perfectly balanced mids, zero mud, zero muddiness, zero low-end buildup, zero artifacts, zero compression artifacts, zero digital hiss, zero clipping, no frequency pollution, no resonance, no phase issues, fully transparent final master, radio broadcast quality, concert hall clarity, warm analog depth + razor-sharp digital precision, present lead vocals, wide and airy soundstage, high-fidelity studio production, crisp transients, layered instruments with clear separation, stable tonal balance and loudness
```

**Do not shorten this prompt during the rescue test.** The controlled test depends on the complete preservation/performance instruction and the complete audio-quality instruction being present.

---

## 4. EXACT CHECKLIST — USE THESE SETTINGS

| Setting | Required value |
|---|---|
| **Model** | **V6 Mini — REQUIRED** |
| **Mode / Operation** | **Sample** |
| **Sample Length** | **Entire song — select the whole song** |
| **Weirdness** | **0%** |
| **Style Influence** | **85%** |
| **Audio Influence** | **85%** |
| **Max Mode** | **ON** |
| **Personalize** | **OFF** |
| **Other options** | **Nothing else enabled** |
| **Lyrics box** | **Original song lyrics ONLY** |
| **Style box** | **Complete Audio Quality prompt — the entire prompt above** |
| **Vocal gender** | **Male/Female as required** |

### Before you generate

1. **Choose V6 Mini.** Do not choose another V6 model for this workflow.
2. Choose **Sample** as the mode/operation.
3. Set **Sample Length to the entire song** — select the whole song.
4. Set **Weirdness to 0%**.
5. Set **Style Influence to 85%**.
6. Set **Audio Influence to 85%**.
7. Turn **Max Mode ON**.
8. Make sure **Personalize is OFF**.
9. Leave **all other options disabled**.
10. Put **ONLY the original song lyrics** in the **Lyrics box**.
11. Put the **entire long audio-quality prompt** in the **Style box**.
12. Select the required **male/female vocal** setting.
13. Generate the controlled test.

**The placement matters:** Lyrics box = **lyrics only**. Style box = **the complete audio-quality prompt only**. There is **no `[SND]` tag** in this workflow. The mode is **Sample**, and Sample Length is **the entire song**. The model is **V6 Mini**. Max Mode is **ON**. Personalize is **OFF**. Weirdness is **0%**. Style Influence and Audio Influence are **85%**.

---

## 5. WHEN V6 AUDIO SOUNDS BAD

Classify the defect before changing the recipe.

### A. Distortion / clipping / crunchy artifacts

Run the controlled rescue setup first. Do not stack additional mastering language or unrelated style instructions on top of it during the diagnostic pass.

### B. Vocal timbre changed

Verify that the entire song was selected for **Sample Length**, that **V6 Mini** is selected, and that the preservation language remains intact. Compare against the original at matched playback level.

### C. Instruments or arrangement drifted

The Style-box prompt explicitly calls for the original instrument playing style, technique, feel and arrangement. Do not add new arrangement directions during the rescue test.

### D. Mud / low-end buildup / harshness

The Style-box prompt explicitly addresses mud, muddiness, low-end buildup, frequency pollution, resonance, clipping and related artifacts. Test the complete prompt before changing individual phrases.

### E. Excessive processing / crushed dynamics

Keep Weirdness at **0%**, keep **Max Mode ON**, and do not enable additional options during the controlled test. The purpose is to isolate the variables rather than create another creative generation.

---

## 6. A/B TESTING RULE

Change one variable at a time **only after the exact controlled setup has been tested**.

```text
BAD V6 RESULT
     ↓
V6 MINI + SAMPLE + ENTIRE SONG SAMPLE LENGTH + MAX MODE ON
     ↓
WEIRDNESS 0% + STYLE 85% + AUDIO 85% + PERSONALIZE OFF
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

This is a **reproducible operational workaround**. The Lyrics box in this workflow contains only the original lyrics; there is **no `[SND]` tag or special directive required**. Judge the workflow by the resulting audio.

Likewise, descriptive phrases such as “lossless hi-fi,” “24-bit digital clean,” “dynamic range 12dB+,” and “zero clipping” are instructions describing the desired result; they do not guarantee a particular technical export specification from the generation model.

The goal of this workflow is simple:

```text
PRESERVE THE PERFORMANCE
+
PRESERVE THE ARRANGEMENT
+
USE THE ENTIRE SONG AS THE SAMPLE
+
REDUCE UNWANTED AUDIO DAMAGE
+
DO NOT INTRODUCE NEW CREATIVE VARIABLES
```
