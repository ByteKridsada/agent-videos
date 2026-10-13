# Pipeline

```
00_raw
  ▼
[0 video-extractor] → 00_raw/*_transcript.txt, 00_raw/*_meta.json, 00_raw/frames/
  (only runs if video files are present)
  ◆ GATE 0: user reviews extracted frames and confirms extraction looks correct
  ▼
[1 intake-analyst]  → 01_brief.md
  ▼
[2 idea-strategist] → 02_ideas.md
  ◆ GATE 1: user picks idea (record in status.md)
  ▼
[3 scriptwriter]    → 03_script.md
  ▼
[4 fact-reviewer]   → 04_review.md
  │  FAIL → back to 3 (max 2 rounds, then ask user)
  ◆ GATE 2: user approves reviewed script
  ▼
[5 storyboarder]    → 05_storyboard.md
  ▼
[6 scene-producer]  → 06_assets/
  ▼
[7 editor-packager] → 07_edit.md, 08_publish.md
  ◆ GATE 3: user watches real clip, approves before publishing
  ▼
 post (by human)
  ▼
[8 performance-analyst] → 10_analysis.md + append context/active/learnings.md
                          (reads real numbers the user fills in 09_results.md)
```

## I/O
| # | Agent | Reads | Writes |
|---|---|---|---|
| 0 | video-extractor | `00_raw/*.{mp4,mov,…}`, `context/active/settings.md` | `00_raw/*_transcript.txt`, `00_raw/*_meta.json`, `00_raw/frames/`, `00_raw/video_extraction_log.md` |
| 1 | intake-analyst | `00_raw/*`, `context/active/*` | `01_brief.md` |
| 2 | idea-strategist | `01_brief.md`, `context/active/*` | `02_ideas.md` |
| 3 | scriptwriter | `01_brief.md`, chosen idea in `status.md`, `voice.md`, `dos-donts.md`, `04_review.md` (revisions) | `03_script.md` |
| 4 | fact-reviewer | `03_script.md`, `01_brief.md`, `00_raw/*`, `dos-donts.md` | `04_review.md` |
| 5 | storyboarder | `03_script.md`, `04_review.md`, `asset-library.md`, `01_brief.md` | `05_storyboard.md` |
| 6 | scene-producer | `05_storyboard.md`, `06_assets/style-lock.md` if present | `06_assets/*` |
| 7 | editor-packager | `03_script.md`, `05_storyboard.md`, `06_assets/*` | `07_edit.md`, `08_publish.md` |
| 8 | performance-analyst | `09_results.md`, all run files | `10_analysis.md`, append `learnings.md` |

## Gates
- Orchestrator stops and asks at all 4 gates (0–3); never skips.
- Gate report: what was produced, what is blocked, decisions needed.
- Decisions are recorded in the run's `status.md`.

## status.md
Each run has `status.md`: current step, chosen idea, gate results, open items. Lets work pause and resume.

## Style lock
AI shots must look consistent. Before producing scenes, scene-producer:
1. Writes `style-lock.md` (colors, light, lens, recurring characters/places).
2. Test-generates 1-2 key assets.
3. User approves; then all shots reference the locked set.
