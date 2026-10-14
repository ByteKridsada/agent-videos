# Asset Test Plan — homing-construction-01

> Complete every item in this checklist before generating the full 8-shot AI batch.
> User style approval is required after items 1–2 before proceeding to items 3–8.

---

## Phase 1 — Style Approval Test (Generate First, Hold for User Review)

### Test Item 1 — Shot 4: Hero Character Reveal (Full Body)

**Why first:** Shot 4 is the clearest full-body character reveal in the clip. It must confirm that the generation model has correctly rendered all locked character traits before any other shot is produced.

**What to generate:** One keyframe image using the Shot 4 prompt from `ai-prompts.md`.

**Pass criteria (all must be YES before proceeding):**
- [ ] Build is visibly stocky/chubby — not average weight, not slim
- [ ] Round glasses present with black or black-gold metal frames
- [ ] Short black hair styled back (pompadour/side-swept)
- [ ] Dark navy long-sleeve button-up shirt — no jacket, no variation in color
- [ ] Dark jeans and black sneakers visible at lower frame
- [ ] Blueprint roll tucked under left arm (cylindrical, brown/cream)
- [ ] Expression reads "calm, quiet confidence" — not a wide grin, not stiff
- [ ] Mountains visible in upper 30% of background
- [ ] Sky is overcast grey-white, not deep blue or golden
- [ ] Overall color grade is muted and cinematic — no HDR pop, no warm filter
- [ ] Image does not look like a CGI render or cartoon — photorealistic editorial quality

**Fail action:** Adjust prompt (add weight to build, glasses, shirt color descriptors) and regenerate before any other shot is produced.

---

### Test Item 2 — Shot 6: Hands Close-Up (Apple Watch + Rings Legibility)

**Why second:** Shot 6 is an extreme close-up on the hands. It tests the accuracy of specific accessory details (Apple Watch Ultra on the left wrist, rings on both hands) and the quality of the blueprint glow FX.

**What to generate:** One keyframe image using the Shot 6 prompt from `ai-prompts.md`.

**Pass criteria (all must be YES before proceeding):**
- [ ] Apple Watch Ultra clearly visible on the left wrist — rectangular watch face, orange band or black/orange crown detail recognizable
- [ ] Rings visible on both hands
- [ ] Blueprint edges show electric-blue glow (hex range #0288D1–#4FC3F7) — NOT green, NOT purple, NOT neon white
- [ ] Glow has a soft volumetric falloff at the edge — NOT a hard neon line
- [ ] Faint architectural geometry visible beneath blueprint surface at low opacity
- [ ] Particle effects (if rendered in still) are small and drift-like — NOT large sparks, NOT confetti
- [ ] Shallow depth of field: blueprint edges sharp, background soft
- [ ] Hands look realistically proportioned — NOT distorted, NOT extra fingers
- [ ] No face visible in frame

**Fail action:** If Apple Watch is missing or wrong, adjust prompt to add stronger Apple Watch Ultra descriptor. If glow color is wrong, add hex values and "NOT neon, NOT green" to the negative block. Regenerate before proceeding.

---

### User Style Approval Gate

After Test Items 1 and 2, present both images to the user with this question:

"Test shots for Shot 4 (full-body character reveal) and Shot 6 (blueprint close-up with glow) are ready for review. Do the character build, glasses, outfit, Apple Watch, and blueprint glow match the locked style? Reply YES to proceed with all 8 shots, or describe any changes needed."

**Do NOT generate Shots 2, 3, 5, 7, 9, or 12 until the user approves.**

---

## Phase 2 — Pre-Production Consistency Checks (After Style Approval)

### Test Item 3 — Costume Continuity Across Shots

**When:** After generating all 8 AI shots.

**Check:** Place all 8 generated keyframes side by side (or in a grid). Confirm:
- [ ] Dark navy shirt color is consistent — same shade across all shots
- [ ] Glasses frames are visibly round and the same color in every shot
- [ ] Build (stocky/chubby) remains consistent — no shot shows a noticeably slimmer character
- [ ] Apple Watch visible in Shots 6 and 7 (close-up shots where it must read clearly)
- [ ] Skin tone is consistent across Shots 2, 3, 4, 5, 9, 12

**Fail action:** Flag inconsistent shots and regenerate individually.

---

### Test Item 4 — Blueprint Glow Color Consistency

**When:** After generating all 8 AI shots.

**Check:** Verify the electric-blue glow appears in Shots 5, 6, 7, 9, and 12. Confirm it is the same blue family (#0288D1–#4FC3F7) across all shots. No shot should show green, purple, or white glow.

**Fail action:** Regenerate any shot with off-color glow, adding explicit hex values to the prompt.

---

### Test Item 5 — Sky and Mountain Consistency

**When:** After generating all 8 AI shots.

**Check:** Confirm that Shots 2, 3, 4, 5, 9, and 12 all show:
- [ ] Overcast to partly cloudy pale grey-white sky (not deep blue, not golden sunset)
- [ ] Mountain ridgeline in the upper 25–35% of the frame in wide and mid shots
- [ ] Mountains have consistent green-to-grey appearance (no snow, no dramatic black peaks)

**Fail action:** Add "overcast grey-white sky, gentle rolling mountains, northern Thailand" to any shot that shows wrong sky or missing mountains.

---

## Phase 3 — "ภาพประกอบ / Illustration" Label Legibility Test

### Test Item 6 — Label on CGI Render Background (Shot 14)

**When:** Before final edit assembly.

**What to test:** Place the "ภาพประกอบ / Illustration" label (white text, 55% opacity black pill, Prompt or Noto Sans Thai, 24–28 pt) at upper-left corner of `Screenshot 2569-10-13 at 22.07.49.png`.

**Pass criteria:**
- [ ] White text is clearly readable against the amber dusk sky at the top-left of the CGI render
- [ ] WCAG AA contrast ratio is met (minimum 4.5:1 for normal text)
- [ ] Pill background does not obscure any critical image content

**Fail action:** If contrast is insufficient at 55% opacity, increase pill opacity to 70% for Shot 14 only. Document the adjusted opacity in `style-lock.md` as a shot-specific override.

---

### Test Item 7 — Label on Dark AI Shot Background

**When:** Before final edit assembly.

**What to test:** Place the label at upper-left corner of the Shot 4 generated image (the darkest likely AI sky area).

**Pass criteria:**
- [ ] White text on 55% opacity pill is readable against the overcast grey-white AI sky
- [ ] Label does not visually merge with any bright element in the frame corner

**Fail action:** Increase pill opacity as needed.

---

## Phase 4 — Real Photo Pre-Publish Check

### Test Item 8 — Worker Blur Check: Screenshot 22.08.07.png (Shot 10)

**When:** Before this photo is used in any edit or export.

**Required action:** Open `runs/homing-construction-01/00_raw/Screenshot 2569-10-13 at 22.08.07.png`. The construction worker figure at the far right of the frame must be cropped out or blurred (Gaussian blur or equivalent, full face and identifying features removed) before this image is used in any edit, test render, or published clip.

**Pass criteria:**
- [ ] Worker figure is not identifiable in the exported frame
- [ ] Crop or blur does not visually disrupt the building facade composition
- [ ] Blue water tank and arched window openings remain visible after crop/blur

**This is a MUST FIX per review issue #3. Do not publish Shot 10 without completing this step.**

---

## Summary Checklist

| Item | Description | Phase | Gate |
|---|---|---|---|
| 1 | Shot 4 hero character keyframe generated and reviewed | Phase 1 | User approval required |
| 2 | Shot 6 hands close-up keyframe generated and reviewed | Phase 1 | User approval required |
| — | USER STYLE APPROVAL GATE | — | Stop until YES |
| 3 | Costume continuity across all 8 shots | Phase 2 | QA pass |
| 4 | Blueprint glow color consistency across all shots | Phase 2 | QA pass |
| 5 | Sky and mountain consistency across all shots | Phase 2 | QA pass |
| 6 | "ภาพประกอบ / Illustration" label legibility on CGI render (Shot 14) | Phase 3 | QA pass |
| 7 | "ภาพประกอบ / Illustration" label legibility on AI shot | Phase 3 | QA pass |
| 8 | Worker blur/crop on Screenshot 22.08.07.png (Shot 10) | Phase 4 | MUST COMPLETE before any edit |
