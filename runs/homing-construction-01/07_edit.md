# Edit Decision List (EDL) — homing-construction-01

- Concept: Grand Orbit — blueprint-pull mechanic
- Aspect ratio: 9:16 (1080 × 1920 px)
- Target length: 50–60 s (master cut: 60 s)
- Platform primary: Facebook; secondary: TikTok
- Output language: Thai (all spoken lines, subtitles, on-screen text)
- Voice mode: Senior builder — calm, direct, explains with quiet confidence

---

## Pre-Edit Requirements

Before opening the timeline, complete all items in `06_assets/asset-test-plan.md`. This EDL cannot be followed until these are done:

1. All 8 AI shot keyframes generated, style-approved by user, and exported as video clips (Shots 2, 3, 4, 5, 6, 7, 9, 12).
2. `Screenshot 2569-10-13 at 22.08.07.png` — worker figure at far right cropped out or blurred (MANDATORY; see Test Item 8). Do not import this file raw into any timeline.
3. "ภาพประกอบ / Illustration" HUD label compositor layer built and tested on Shot 14 background (asset-test-plan.md Test Items 6–7).

---

## Color Grade Instruction

Apply a single base LUT across the entire timeline before per-shot adjustments:

- **LUT direction:** Cinematic desaturated warm-base with a slight cool push on shadows. Overcast-day construction site look — not a music video, not Instagram warm.
- **Ground/earth tones:** Desaturate slightly, push toward dry ochre-beige. No golden warmth.
- **Mountain/sky tones:** Cool blue-grey on ridgeline; sky stays pale grey-white.
- **Character (AI shots):** Neutral-warm skin; dark navy shirt absorbs light cleanly; no color cast.
- **Blueprint glow:** The ONLY fully-saturated color element across the entire clip. Electric blue (#0288D1 core / #4FC3F7 edge). Protect this from LUT desaturation — apply the LUT below the glow layers or mask the glow area.
- **Real photo shots (1, 8, 10, 11, 13, 15):** Apply the same base LUT. Real photos may need a slight contrast lift to match the AI shot tonality — match luminance in Shot 8 to the preceding AI Shot 7 before cutting.
- **CGI render shot (14):** The amber dusk sky tone should be preserved. Apply a lighter hand on this shot — warm tones are intentional and are the emotional peak. Do not desaturate the amber sky.
- **Transition between AI and real photos:** Match overall luminance at cut points. The hard cuts (AI → real photo) are intentional and should feel like a snap of reality, not a jarring brightness jump.

---

## Music Arc Summary

| Timecode | Music state | Description |
|---|---|---|
| 0:00–0:03 | Silence / ambient only | Wind, distant bird call. No score. |
| 0:03 | Score enters | Low strings + single sustained brass note. Quiet, establishing scale and gravitas. |
| 0:03–0:18 | Build stage 1 | Strings and brass thicken slowly. One melodic motif introduced. Score matches the orbital camera arc. |
| 0:18–0:34 | Build stage 2 | Each real-photo hard cut (Shots 8, 10) should land on a rhythmic orchestral accent or percussive hit. The score rewards the pull-to-reveal mechanic. |
| 0:34–0:42 | Orbital climax | Full orchestra. Strings rising, brass swelling. The widest, most sweeping moment of the score — matches the 120–180° drone sweep in Shot 11. |
| 0:42–0:48 | Escalation | Score accelerates with the camera speed-ramp. Percussion adds urgency. Score drives toward apex. |
| 0:48 | Apex / single hit | A brief silence or single piano/bell note immediately before the flash cut to CGI. This silence or hit is the emotional peak. |
| 0:48–0:52 | Hold at peak | Warm ambient swell under the CGI dusk image. Score holds, does not fall yet. |
| 0:52–1:00 | Resolved coda | Same opening motif returns, warm, settled, confident. Holds under brand title to end. |

Music style: Symphonic/cinematic orchestral. Think modern commercial construction or architecture reveal — scale, gravitas, earned confidence. No copyrighted track names.

---

## Shot-by-Shot EDL

---

### Shot 1 — Hook
- **Timecode:** 0:00–0:03 (3 s)
- **Type:** REAL_PHOTO
- **Source file:** `00_raw/836959163_18644608891048359_5489349789714552875_n.jpg`
- **Camera motion:** Ken Burns — slow tilt-down (top-to-bottom). Start frame: mountain ridgeline fills upper 60% of frame. End frame: building mid-distance centered, open grassland visible in foreground. Speed: very slow, smooth, continuous over 3 s.
- **VFX:** None unless AI-extended parallax is applied. If AI parallax motion extension is used to simulate drone descent, "ภาพประกอบ / Illustration" label MUST appear on any AI-generated frames within this shot. If pure Ken Burns (no AI generation), no label required.
- **Audio VO:** (no voiceover — wind ambience and distant birdsong only)
- **Music:** Silence. Ambient sound only.
- **On-screen text:**
  - "แค่ที่ดินเปล่า..." — center frame, 48 pt white Prompt/Noto Sans Thai, no background pill. Fade in at 0:01, fade out by 0:03.
- **Subtitle:** (none — no spoken line)
- **Transition to Shot 2:** Hard cut.

---

### Shot 2 — Owner Enters: Boot Level
- **Timecode:** 0:03–0:06 (3 s)
- **Type:** AI_ILLUSTRATION
- **Source file:** AI-generated — Shot 2 prompt from `06_assets/ai-prompts.md`
- **Camera motion:** Fixed extreme low-angle (boot level). No camera movement. Boots walk toward center frame.
- **VFX:** Dust particle drift upward from footsteps — practical, cinematic, small particles.
- **Audio VO:** "ทุกความสำเร็จ เริ่มต้นจากแบบแปลนเพียงหนึ่งแผ่น" — first half of line begins here. Pacing: slow, deliberate. One syllable group at a time. [PAUSE after "ทุกความสำเร็จ" — 0.5 s]. Then "เริ่มต้นจากแบบแปลนเพียงหนึ่งแผ่น" continues into Shot 3.
- **Music:** Low strings + single sustained brass note enter. Quiet, under the VO.
- **On-screen text:** "ภาพประกอบ / Illustration" — upper-left HUD. White text (#FFFFFF), Prompt/Noto Sans Thai Regular 24–28 pt, on semi-transparent black pill (55% opacity, 8 px vertical padding, 14 px horizontal padding, 6 px corner radius). Anchored at 24 px from left, 48 px from top. Fixed compositor layer — topmost in stack. Appears from frame 1 of this shot.
- **Subtitle:** (no subtitle line for first half of VO — line carries across two shots; subtitle chunk appears in Shot 3)
- **Transition to Shot 3:** Continuous flow (no cut visible — same AI generation pass).

---

### Shot 3 — Owner Enters: Rising to Mid-Shot
- **Timecode:** 0:06–0:09 (3 s)
- **Type:** AI_ILLUSTRATION
- **Source file:** AI-generated — Shot 3 prompt from `06_assets/ai-prompts.md`
- **Camera motion:** Slow rising from knee level to chest level; simultaneous slow left-to-right orbital arc beginning; slight forward drift. Mountains remain stable in background.
- **VFX:** Dust particle continuity from Shot 2.
- **Audio VO:** "เริ่มต้นจากแบบแปลนเพียงหนึ่งแผ่น" — second half of line, completing the sentence.
- **Music:** Strings slowly thicken. Melodic motif begins to emerge.
- **On-screen text:** "ภาพประกอบ / Illustration" — HUD persists, static, fixed to frame. Does not scroll or move during orbital arc.
- **Subtitle:** "ทุกความสำเร็จ เริ่มต้นจากแบบแปลนเพียงหนึ่งแผ่น" — lower third, white text, dark semi-transparent background bar, Prompt/Noto Sans Thai. 2-line max. Position within platform safe zone (see Safe Zone note below). Subtitle appears over Shots 2–3 combined; holds for ~4 s.
- **Transition to Shot 4:** Continuous into Shot 4.

---

### Shot 4 — Owner Surveying: Hero 3/4 View
- **Timecode:** 0:09–0:12 (3 s)
- **Type:** AI_ILLUSTRATION
- **Source file:** AI-generated — Shot 4 prompt from `06_assets/ai-prompts.md`
- **Camera motion:** Orbital arc decelerates from Shot 3 and settles at front 3/4 position. Slight continued push-in. Camera height: just below eye level.
- **VFX:** None. Character expression must read "calm, confident, expert."
- **Audio VO:** "ผมและทีมงาน ลงมือสร้างมันขึ้นมา ทีละขั้นตอน" — first half begins here. [EMPHASIS on "ลงมือสร้าง" — slight weight in delivery]. Continues into Shot 5.
- **Music:** First full orchestral swell begins. Brass joins strings.
- **On-screen text:** "ภาพประกอบ / Illustration" — HUD persists, static to frame.
- **Subtitle:** "ผมและทีมงาน ลงมือสร้างมันขึ้นมา ทีละขั้นตอน" — subtitle chunk, lower third. Appears over Shots 4–5 combined.
- **Transition to Shot 5:** Cut on owner's turn gesture into Shot 5.

---

### Shot 5 — Blueprint Raised with Energy Lines
- **Timecode:** 0:12–0:15 (3 s)
- **Type:** AI_ILLUSTRATION
- **Source file:** AI-generated — Shot 5 prompt from `06_assets/ai-prompts.md`
- **Camera motion:** Orbital arc continues slowly. Slight push-in toward owner as he raises the blueprint. Wide-to-medium framing.
- **VFX:** Electric-blue energy lines begin to trace the scroll surface. Energy lines: hex #0288D1 core, #4FC3F7 edge bloom. Soft volumetric edge falloff. Not hard neon lines. VFX begins faint and intensifies across the 3 s.
- **Audio VO:** "ผมและทีมงาน ลงมือสร้างมันขึ้นมา ทีละขั้นตอน" — second half, completing the line.
- **Music:** Strings and brass thicken. Orchestra builds.
- **On-screen text:** "ภาพประกอบ / Illustration" — HUD persists.
- **Subtitle:** (continues from Shot 4 subtitle block)
- **Transition to Shot 6:** Match-cut on blueprint movement.

---

### Shot 6 — Blueprint Unfurl Close-Up (Hands)
- **Timecode:** 0:15–0:18 (3 s)
- **Type:** AI_ILLUSTRATION
- **Source file:** AI-generated — Shot 6 prompt from `06_assets/ai-prompts.md`
- **Camera motion:** Static close-up on hands. Very slow push-in toward glowing blueprint surface. Shallow depth of field on blueprint edges and hands.
- **VFX:** Blueprint edges light up with electric-blue glow (#0288D1 core, #4FC3F7 edge bloom, soft 3–5 mm volumetric falloff). Faint abstract architectural line geometry glows at 30–40% opacity beneath blueprint surface. Small slow-floating blue particle specks drift upward from surface (ember drift quality, not confetti or large sparks). Apple Watch Ultra on left wrist must remain visible and legible.
- **Audio VO:** (VO from Shot 5 carries over — no new line starts here. Brief natural pause before next line.)
- **Music:** Orchestra holds; slight suspense beat before the first pull.
- **On-screen text:** "ภาพประกอบ / Illustration" — HUD persists.
- **Subtitle:** (none — no new spoken line)
- **Transition to Shot 7:** Hard cut on the moment hands reach into the blueprint surface.

---

### Shot 7 — First Pull: Bamboo Poles
- **Timecode:** 0:18–0:21 (3 s)
- **Type:** AI_ILLUSTRATION
- **Source file:** AI-generated — Shot 7 prompt from `06_assets/ai-prompts.md`
- **Camera motion:** Static/slight push-in on hands. Poles emerge and sweep screen-right.
- **VFX:** Hands plunge into glowing blueprint portal (shallow portal depth, blue ambient wash upward onto hands and forearms). Bamboo poles emerge solid and physically real (not translucent/ghostly). Electric-blue particle trails follow poles pointing back toward the portal. Slight motion blur on the sweeping gesture.
- **Audio VO:** "เริ่มจากโครงนั่งร้าน ฐานที่มั่นคงของงานก่อสร้าง" — full line. [EMPHASIS on "ฐานที่มั่นคง"]. Pacing: measured, confident.
- **Music:** Rhythmic orchestral accent lands on the hard cut to Shot 8. Time the accent to land at 0:21.
- **On-screen text:** "ภาพประกอบ / Illustration" — HUD persists until the hard cut. Label disappears on frame 1 of Shot 8.
- **Subtitle:** "เริ่มจากโครงนั่งร้าน ฐานที่มั่นคงของงานก่อสร้าง" — lower third, appears over Shots 7–8 combined (VO line carries across the cut).
- **Transition to Shot 8:** HARD CUT on the moment poles leave the frame. Transition must feel like a snap.

---

### Shot 8 — Scaffolding Real Reveal
- **Timecode:** 0:21–0:26 (5 s)
- **Type:** REAL_PHOTO
- **Source file:** `00_raw/836959163_18644608891048359_5489349789714552875_n.jpg`
- **Camera motion:** Ken Burns — slow push-in (z-axis) from wide aerial toward building face. Simulated drone push. Speed: slow and dramatic over 5 s. Start frame: wide aerial showing full building and grassland foreground. End frame: medium close on building face with scaffolding structure.
- **VFX:** None. No label on this shot. Confirm scaffolding material before publishing (see storyboard flag: if scaffold is metal pipe, not bamboo, remove "โครงนั่งร้าน" overlay from this shot and move to Shot 10 only).
- **Audio VO:** "เริ่มจากโครงนั่งร้าน ฐานที่มั่นคงของงานก่อสร้าง" — line completes over this shot.
- **Music:** Rhythmic hit has landed; score breathes and then continues building.
- **On-screen text:**
  - NO "ภาพประกอบ / Illustration" label.
  - "โครงนั่งร้าน" — lower-left, white sans-serif (Prompt/Noto Sans Thai), clean, no pill background. Appears at 0:21, hold 1.5 s, then fade out.
- **Subtitle:** (continues from Shot 7 subtitle block)
- **Transition to Shot 9:** Hard cut back to AI.

---

### Shot 9 — Second Pull: Steel Sheets and Concrete Blocks
- **Timecode:** 0:26–0:29 (3 s)
- **Type:** AI_ILLUSTRATION
- **Source file:** AI-generated — Shot 9 prompt from `06_assets/ai-prompts.md`
- **Camera motion:** Medium shot. Slight push-in. Owner's gestures are swift and decisive.
- **VFX:** Two visually distinct pulls: (1) flat galvanized steel roofing sheets (flat, metallic shimmer, reflective); (2) concrete blocks (grey, heavy-textured, matte). Background building rises a storey via fast morph effect. Electric-blue blueprint glow in the held hand.
- **Audio VO:** "วัสดุคุณภาพ ถูกคัดสรรและประกอบขึ้นอย่างพิถีพิถัน ทีละชั้น" — full line. [PAUSE after "วัสดุคุณภาพ" — 0.5 s]. [EMPHASIS on "พิถีพิถัน"].
- **Music:** Rhythmic orchestral accent timed to land at 0:29 on the hard cut to Shot 10.
- **On-screen text:** "ภาพประกอบ / Illustration" — HUD upper-left. Upper-left corner of the generated image must remain visually clear for the overlay.
- **Subtitle:** "วัสดุคุณภาพ ถูกคัดสรรและประกอบขึ้น อย่างพิถีพิถัน ทีละชั้น" — lower third, over Shots 9–10 combined.
- **Transition to Shot 10:** Hard cut on second throw.

---

### Shot 10 — Materials Real Reveal
- **Timecode:** 0:29–0:34 (5 s)
- **Type:** REAL_PHOTO
- **Source file:** `00_raw/Screenshot 2569-10-13 at 22.08.07.png`
- **PRE-EXPORT MANDATORY ACTION — WORKER BLUR:** The construction worker figure at the far right of this frame MUST be cropped out or blurred (Gaussian blur, full face and identifying features removed) BEFORE this file is imported into any timeline or used in any test render. This is a MUST FIX. Blue water tank and arched window openings must remain visible after the crop/blur. Do not export any version of this clip until this is confirmed done.
- **Camera motion:** Ken Burns — slow tilt-up (low-angle push upward along building face). Start frame: ground level (debris, bamboo poles). End frame: top of building filling upper frame. Speed: slow and dramatic over 5 s.
- **VFX:** None.
- **Audio VO:** "วัสดุคุณภาพ ถูกคัดสรรและประกอบขึ้นอย่างพิถีพิถัน ทีละชั้น" — line completes over this shot.
- **Music:** Rhythmic hit has landed; orchestra continues building toward orbital climax.
- **On-screen text:**
  - NO "ภาพประกอบ / Illustration" label.
  - "วัสดุคุณภาพ" — lower-left, white sans-serif, same style as Shot 8 overlay. Appears at 0:29, hold 1.5 s, fade out.
- **Subtitle:** (continues from Shot 9 subtitle block)
- **Transition to Shot 11:** Cut or speed-ramp into orbital sweep.

---

### Shot 11 — Orbital Climax
- **Timecode:** 0:34–0:42 (8 s)
- **Type:** REAL_PHOTO
- **Source file:** `00_raw/836959163_18644608891048359_5489349789714552875_n.jpg`
- **Camera motion:** Ken Burns orbital sweep — simulate 120–180° orbital arc around the building. Camera height held at below mid-building level throughout. Mountains in background fill upper frame consistently throughout the arc. No altitude change. This must read as a single unbroken 8-second movement — do not cut within this shot.
- **VFX:** None. If orbital motion is created via AI frame interpolation on the static photo, any AI-generated interpolated frames require the "ภาพประกอบ / Illustration" label for those frames only.
- **Audio VO:** "โครงสร้างสูงขึ้น ด้วยมาตรฐานงานช่างที่ใส่ใจทุกรายละเอียด" — full line. [EMPHASIS on "มาตรฐานงานช่าง"]. Pacing: slow, giving the line space to breathe against the wide music swell.
- **Music:** Full orchestra — strings rising, brass swelling against the mountain backdrop. This is the widest, most sweeping music moment. Score is at its orchestral peak for these 8 seconds.
- **On-screen text:** NO "ภาพประกอบ / Illustration" label (real photo). NO text overlay during this shot — let the building and music speak.
- **Subtitle:** "โครงสร้างสูงขึ้น ด้วยมาตรฐานงานช่าง ที่ใส่ใจทุกรายละเอียด" — lower third, 2-line break as shown.
- **Transition to Shot 12:** Cut on owner's re-entry into frame.

---

### Shot 12 — Final Pull: Deep Both-Hands Pull + Fast Orbital Pull-Back
- **Timecode:** 0:42–0:46 (4 s)
- **Type:** AI_ILLUSTRATION
- **Source file:** AI-generated — Shot 12 prompt from `06_assets/ai-prompts.md`
- **Camera motion:** Fast orbital pull-back at 2× the previous orbital rate. Wide to reveal full construction site context. Dramatic background motion blur on mountain and site edges as orbital speed peaks. Speed escalation must feel like a climactic gear-shift — this is the pacing signal that the sequence is ending.
- **VFX:** Both hands plunge simultaneously into glowing blueprint portal. Abstract luminous orb or energy fragment emerges (not bamboo, steel, or concrete — abstract essence, electric blue, softly pulsing). Cool rim lighting on character shoulders from mountain skyline behind. Motion blur on fast orbital.
- **Audio VO:** "และนี่คือผลงานจริง ที่เราส่งมอบให้ลูกค้า" — full line. [EMPHASIS on "ผลงานจริง"]. [PAUSE before "ที่เราส่งมอบให้ลูกค้า" — 0.5 s].
- **Music:** Score accelerates with the camera speed-ramp. Percussion adds urgency. Driving toward apex at 0:48.
- **On-screen text:** "ภาพประกอบ / Illustration" — HUD persists through entire Shot 12 and through to Shot 13 cut.
- **Subtitle:** "และนี่คือผลงานจริง ที่เราส่งมอบให้ลูกค้า" — lower third, over Shots 12–13 combined.
- **Transition to Shot 13:** Speed-ramp hard cut.

---

### Shot 13 — Speed-Ramp Real Reveal
- **Timecode:** 0:46–0:48 (2 s)
- **Type:** REAL_PHOTO
- **Source file:** `00_raw/836959163_18644608891048359_5489349789714552875_n.jpg`
- **Camera motion:** Speed-ramp cut landing at wide drone angle. Brief static hold 2 s. No camera movement. Let the building register before flash cut.
- **VFX:** None.
- **Audio VO:** "และนี่คือผลงานจริง ที่เราส่งมอบให้ลูกค้า" — tail of line carries into this shot.
- **Music:** Score drives hard — final beats before the apex pause.
- **On-screen text:** NO "ภาพประกอบ / Illustration" label.
- **Subtitle:** (continues from Shot 12 subtitle block)
- **Transition to Shot 14:** Flash cut to CGI. This is the sharpest cut in the clip.

---

### Shot 14 — CGI Reveal (Apex)
- **Timecode:** 0:48–0:52 (4 s)
- **Type:** CGI_RENDER
- **Source file:** `00_raw/Screenshot 2569-10-13 at 22.07.49.png`
- **Camera motion:** Static wide frame. No camera movement. CGI fills the 9:16 frame. Hold 2 s. Then initiate cross-dissolve toward Shot 15. The cross-dissolve duration: 1–1.5 s, completing by 0:52.
- **VFX:** None (the CGI render is the visual event).
- **Audio VO:** (no voiceover — music reaches apex)
- **Music:** Brief silence or single piano/bell hit at 0:48 (the flash cut moment). Then a warm ambient swell under the CGI dusk image. Score holds at peak; does not resolve yet.
- **On-screen text:**
  - "ภาพประกอบ / Illustration" — HUD MANDATORY on every frame of this shot for the full 4 s, INCLUDING all frames during the cross-dissolve transition. The label must NOT fade, soften, or disappear during the dissolve. Verify white text legibility against the amber dusk sky background at upper-left. If WCAG AA contrast is not met at 55% opacity, increase pill opacity to 70% for this shot only (shot-specific override; document in style-lock.md). Label must remain at 100% legibility through all dissolve frames.
- **Subtitle:** (none — no spoken line)
- **Transition to Shot 15:** Cross-dissolve completes into Shot 15.

---

### Shot 15 — Close + CTA
- **Timecode:** 0:52–1:00 (8 s)
- **Type:** REAL_PHOTO
- **Source file:** `00_raw/836959163_18644608891048359_5489349789714552875_n.jpg`
- **Camera motion:** Static or very slow pull-back (Ken Burns). Wide beauty shot. Serene. Camera locks down after initial settle. No orbital movement.
- **VFX:** None.
- **Audio VO:** "โฮมมิ่ง คอนสตรัคชั่น แอนด์ ดีไซน์ รับสร้างบ้านคุณภาพ" — final line. Pacing: clear, unhurried, direct. [EMPHASIS on brand name]. [PAUSE 0.5 s between brand name and service descriptor].
- **Music:** Resolved warm coda. Same opening motif returns — warm, settled, confident. Holds under brand title to end of clip. Score does not cut abruptly; allow a 1–2 s fade after the final frame if needed for platform.
- **On-screen text (layered lower-third, sequential fade-ins):**
  1. "โฮมมิ่ง คอนสตรัคชั่น แอนด์ ดีไซน์" — brand title. Clean dark semi-transparent lower-third bar (not full black). Prompt/Noto Sans Thai. Fade-in at 0:53.
  2. "รับสร้างบ้านคุณภาพ เชียงใหม่ และพะเยา" — service line, below brand title. Smaller font size. Fade-in at 0:54.
  3. "ทักมาคุยได้เลย" — CTA text. Larger than service line for visual hierarchy. Appears at 0:56, hold to end of clip. Not spoken aloud — text only.
- **Subtitle:** "โฮมมิ่ง คอนสตรัคชั่น แอนด์ ดีไซน์ รับสร้างบ้านคุณภาพ" — lower third. Do not overlap with the brand lower-third bar; position subtitle above the lower-third bar.
- **Transition:** Clip ends at 1:00 on hold. No outro animation.

---

## Platform Safe Zones

9:16 vertical format. UI elements appear at top and bottom on both Facebook and TikTok.

- **Top safe zone:** Keep critical content below 160 px from top (status bar + platform UI). The "ภาพประกอบ / Illustration" HUD is anchored at 48 px from top — this is within the top safe zone; accept this position as it is required for regulatory visibility. Confirm it does not collide with platform-native UI elements on export.
- **Bottom safe zone:** Keep subtitles and on-screen text above 300 px from the bottom edge (above TikTok/Facebook action buttons and caption overlay area). The lower-third brand bar in Shot 15 must clear this zone — place the bar with its bottom edge no lower than 280 px from the bottom.
- **Side safe zones:** 40 px from each side edge minimum for all text.
- **Subtitle placement:** Lower third, inside bottom safe zone. Two-line maximum per screen. Thai word-break check: do not break Thai words mid-syllable cluster at a line end. Recommended break points for multi-line subtitles are marked in the subtitle list above.

---

## AI Label QC Checklist

The editor must verify each item below before final export. Every frame listed must carry the "ภาพประกอบ / Illustration" HUD label.

| Shot | Timecode | Type | Label required | QC check |
|---|---|---|---|---|
| 2 | 0:03–0:06 | AI_ILLUSTRATION | Yes — from frame 1 | [ ] Label visible frame 1; static; does not move with camera |
| 3 | 0:06–0:09 | AI_ILLUSTRATION | Yes | [ ] Label visible throughout orbital arc; static to frame |
| 4 | 0:09–0:12 | AI_ILLUSTRATION | Yes | [ ] Label visible; static at orbital deceleration |
| 5 | 0:12–0:15 | AI_ILLUSTRATION | Yes | [ ] Label visible during push-in; static |
| 6 | 0:15–0:18 | AI_ILLUSTRATION | Yes | [ ] Label visible; face not in frame; label still required |
| 7 | 0:18–0:21 | AI_ILLUSTRATION | Yes — until hard cut | [ ] Label present on last AI frame before cut to Shot 8 |
| 9 | 0:26–0:29 | AI_ILLUSTRATION | Yes | [ ] Upper-left frame corner clear for overlay |
| 12 | 0:42–0:46 | AI_ILLUSTRATION | Yes — persists through speed-ramp | [ ] Label visible during 2× orbital speed-ramp |
| 14 | 0:48–0:52 | CGI_RENDER | Yes — ENTIRE DURATION including dissolve | [ ] Label present on every dissolve frame; contrast at AA on amber sky; increase pill to 70% if needed |

Shot 1: Label required ONLY if AI parallax motion extension is applied. If pure Ken Burns, no label required. Editor must document which approach was used.
Shot 11: Label required ONLY on AI-interpolated frames, if AI frame interpolation was used for orbital motion. If pure Ken Burns, no label required. Editor must document.

---

## Pre-Export Checklist

Complete all items before exporting the final deliverable.

- [ ] Aspect ratio: 9:16 confirmed. No pillarboxing, no letterboxing.
- [ ] Length: Total clip 50–60 s. Master cut is 60 s. Do not exceed 60 s.
- [ ] Loudness: Target -14 LUFS integrated (Facebook/Meta standard). TikTok: -14 LUFS. Peak: -1 dBTP true peak. VO mixed at -12 to -10 dBFS. Music mixed 6–8 dB below VO during spoken lines; music at natural level during silent beats.
- [ ] Subtitles: All Thai lines present. No subtitle overlaps with lower-third brand bar. Maximum 2 lines per screen. Thai word breaks checked against subtitle text above.
- [ ] "ภาพประกอบ / Illustration" HUD: All 9 AI/CGI shots confirmed labeled (see AI Label QC Checklist above). Shot 14 contrast verified against amber sky. Label does not disappear during dissolve.
- [ ] Worker blur: `Screenshot 2569-10-13 at 22.08.07.png` (Shot 10) — worker figure at far right confirmed cropped or blurred. Verified in exported frame, not only in source file.
- [ ] No UNVERIFIED claims on screen: Owner name not shown. Project address not shown. Construction timeline not stated. No price or model name on screen.
- [ ] CTA text "ทักมาคุยได้เลย" visible in Shot 15 from 0:56 to end. Not spoken in VO.
- [ ] Review flag #4 resolved: Confirm scaffolding material in Shot 8 aerial photo is bamboo before using "โครงนั่งร้าน" overlay. If metal pipe scaffold, update overlay text or remove.
- [ ] Export format: MP4, H.264 (or H.265 for TikTok), minimum 1080 × 1920 px, 30 fps minimum.
