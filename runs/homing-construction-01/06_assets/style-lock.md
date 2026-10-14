# Style Lock — homing-construction-01

> This document is the single visual consistency bible for all shots in this clip.
> Reuse every description below verbatim when writing or reviewing any AI generation prompt for this run.
> No deviations without a new versioned style-lock that replaces this file entirely.

---

## 1. Color Palette and LUT Direction

- **Overall grade target:** Muted, cinematic desaturation. Not Instagram-warm, not HDR-vivid.
- **Ground / earth tones:** Dry ochre-brown compacted soil, dusty beige grassland — desaturated, not golden.
- **Mountain / sky tones:** Cool blue-grey mountain ridgeline; sky is overcast-to-partly-cloudy pale grey-white — NOT deep tourist blue.
- **Character tones:** Neutral-warm skin on the owner; dark navy shirt absorbs light cleanly; no color cast on clothing.
- **Blueprint glow:** The ONLY fully-saturated color in any AI-generated frame. Electric blue — hex `#4FC3F7` (light) to `#0288D1` (core glow). Never cyan-green, never purple, never orange.
- **LUT direction:** Cinematic desaturated warm-base with a slight cool push on shadows. Think overcast-day construction site, not a music video.
- **Colors to avoid in AI shots:** Over-saturated sky blues, neon greens, golden-hour orange warmth, Instagram presets, purple lens flare.

---

## 2. Lighting Style for AI-Generated Shots

- **Primary light source:** Diffused overcast daylight — no hard directional sun shadows on the character or site.
- **Character lighting:** Soft, slightly elevated frontal fill. No rim-light theatrics. Shadows exist but are gentle.
- **Dramatic character:** Achieved through composition, lens, and depth of field — NOT through contrast or theatrical light.
- **Exception — Shot 12 (climactic pull):** Dramatic lighting uplift allowed: slightly stronger backlight from the mountain skyline, cooler rim on character shoulders, to match the escalating score moment.
- **No:** Artificial studio key-lights, warm-gel bounce, fog/haze machine look, golden-hour lens flare.

---

## 3. Blueprint Glow — Exact Specification

- **Color:** Electric blue, core hex `#0288D1`, edge bloom to `#4FC3F7`. No variation across any shot.
- **Intensity:** Moderate. The glow should be clearly visible but not wash out surrounding detail. Blueprint lines readable beneath the glow in close-up shots.
- **Edge behavior:** Soft volumetric edge bloom — the outer 3–5 mm of the blueprint edge radiates outward with a soft falloff. Edges do not clip to hard bright lines.
- **Interior surface:** Faint architectural line geometry (abstract, no legible real drawings) glows at 30–40% opacity beneath the surface of the unrolled blueprint.
- **Portal depth (Shots 7, 12):** When hands plunge into the blueprint surface, the interior appears to have depth — like looking into a shallow luminous pool. A slight ambient blue wash emanates upward onto the hands and forearms.
- **Quality:** Cinematic, grounded, practical-light quality. NOT neon signage. NOT video-game HUD. NOT cartoon glow effect.

---

## 4. Blueprint Pull VFX — Mid-Air Material Description

- **Particle trail:** Materials emerging from the blueprint portal leave a light electric-blue particle drift — small, slow-floating specks (like ember drift, not confetti). Particles fade out within 10–20 cm of the object.
- **Object appearance mid-pull:** Objects are fully solid and physically real-looking the instant they leave the blueprint surface — bamboo poles look like real bamboo, steel sheets look like real galvanized metal. The glow does NOT make them look translucent or ghostly.
- **Solidification behavior:** No dissolve-in, no phase-in animation required in the still image. In the still: object is solid, mid-pull, with trailing blue particles still attached.
- **Energy trail direction:** Always follows the direction of arm sweep — trails point BACK toward the blueprint, not forward.

---

## 5. Camera Lens Character

- **Focal length range:** 24 mm to 50 mm equivalent (full-frame). No telephoto compression. No extreme wide fisheye distortion.
- **Depth of field:** Shallow in close-up shots (6, 7) — background mountains soft. Medium depth in mid-shots (3, 4, 5, 9). Wide depth in the orbital pull-back (Shot 12).
- **Motion blur:** Orbital sweeps carry gentle background motion blur consistent with the 24–35 mm focal range and a slow sweep speed. Not streaky. Not stylized.
- **Orbital arc behavior:** Camera orbits feel physically motivated — like a camera operator walking slowly around the subject, not a CG turntable.
- **Aspect ratio:** All AI-generated shots: **9:16** (vertical, 1080 × 1920 px reference).

---

## 6. "ภาพประกอบ / Illustration" HUD Label — Exact Specification

- **Text:** `ภาพประกอบ / Illustration`
- **Font:** Prompt Regular or Noto Sans Thai Regular — whichever is available at rendering time; both are acceptable.
- **Size:** 24–28 pt equivalent at 1080 × 1920 px. Approximately 50–60 px rendered height.
- **Color:** White (`#FFFFFF`), no shadow, no outline.
- **Background pill:** Rounded rectangle behind the text. Fill: black (`#000000`) at 55% opacity. Padding: 8 px vertical, 14 px horizontal. Corner radius: 6 px.
- **Position:** Upper-left corner. Anchored at 24 px from left edge, 48 px from top edge (safe zone, inside notch/status bar area).
- **Layer behavior:** Fixed compositor HUD — topmost layer in the composition stack. Must NOT be attached to any moving on-screen element. Must NOT animate, scale, fade, or scroll with camera movement.
- **Legibility on CGI render (Shot 14 — amber dusk sky):** The amber sky background at the top-left of `Screenshot 2569-10-13 at 22.07.49.png` requires verification. If WCAG AA contrast is not met by the 55% opacity pill alone, increase pill opacity to 70% for that shot only. Do NOT reduce the pill opacity below 55% on darker AI shots.
- **Legibility on AI shots (darker sky):** At 55% pill opacity over the overcast grey-blue sky of AI shots, white text meets AA contrast. Confirm before final export.
- **Persistence:** Label appears on every frame that contains AI-generated or CGI content. Disappears only on shots confirmed as pure real-photo (Shots 1 [if no AI motion extended], 8, 10, 11, 13, 15). Persists through all dissolve and transition frames involving AI or CGI.

---

## 7. Consistent Elements Across All AI Shots (Shots 2–12)

### Sky
- Overcast to partly cloudy pale grey-white. NOT deep blue. NOT golden sunset. NOT dramatic storm.
- Consistent across Shots 2 through 12. The sky tone must not shift between shots within this run.

### Ground Surface
- Dry compacted earth/clay, dusty ochre-beige. Short dead grassland patches scattered. Consistent across all site-level and mid-shot AI frames.
- No puddles, no mud, no freshly turned soil.

### Site Boundaries
- Open construction plot. No fencing visible in AI shots unless required by narrative.
- Site has a clear open foreground and the mountain range fills the upper 25–35% of the background in wide shots.
- No urban clutter, no vehicles, no power lines visible in AI frames.
- No other people visible in any AI shot — owner is always alone on the site.

### Mountain Range
- Gentle rolling mountain ridgeline. Northern Thailand character — green-to-grey vegetated slopes, no snow, no dramatic jagged peaks.
- Mountains appear in the upper 25–35% of the 9:16 frame in Shots 2, 3, 4, 5, 9, and 12.
- Mountains must NOT shift position, size, or color between shots within the same sequence.

---

## 8. Recurring Character — เจ้าของ (Business Owner) — VERBATIM LOCK

> This description must be prepended verbatim to every AI generation prompt that includes the character.

**Thai male business owner, early-to-late 30s, chubby round face, full cheeks, short black hair styled back in a pompadour/side-swept manner, round glasses with black or black-gold metal frames (medium-large size), stocky build (chubby, not thin), medium height, dark navy long-sleeve button-up shirt, dark jeans, black sneakers, Apple Watch Ultra on left wrist, small rings on both hands, upright confident posture, not stiff.**

Lock rules:
- Round glasses: present in every shot except on-site sunglasses variant (on-site variant NOT used in this run — glasses in all shots).
- Dark navy shirt: no variation, no jacket, no vest added.
- Apple Watch Ultra on LEFT wrist: must be visible in Shots 6 and 7 (close-up hand shots).
- Stocky/chubby build: confirmed in every shot — do not drift toward slim or average build.
- No other people in frame in any AI shot.

---

## 9. Recurring Prop — Blueprint Roll — VERBATIM LOCK

> This description must be used verbatim in every prompt that includes the blueprint.

**Cylindrical scroll, 60–70 cm long, brown/cream exterior paper with slightly weathered edges, held under the left arm when not active; when raised, the exterior begins to trace faint electric-blue energy lines; when unrolled, the interior surface activates with glowing electric-blue architectural line geometry and a soft portal depth; electric-blue color #0288D1 core, #4FC3F7 edge bloom; cinematic particle drift from the surface; NOT neon, NOT cartoon, NOT video-game HUD aesthetic.**

---

## 10. Negative List (All AI Shots)

The following must NOT appear in any AI-generated frame for this run:

- Slim, thin, or average-build character (character must be stocky/chubby)
- Missing glasses or wrong glasses shape (must be round frames)
- Suit jacket, tie, vest, polo shirt, or short sleeves on the character
- Other people in the frame
- Deep blue or golden sunset sky
- Cartoonish glow effects, neon colors, rainbow energy, purple or green blueprint glow
- CGI-looking renders or 3D-rendered aesthetic
- Fantasy or video-game aesthetic
- Legible real architectural drawings on the blueprint surface
- Brand logos, text in the image, signage
- Urban clutter: cars, power lines, tall buildings, crowds
- Weapons, animals, fire, water
- Any real person's likeness
