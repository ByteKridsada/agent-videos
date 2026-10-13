# Video Agents: reusable AI team that turns raw data into clips

Fixed pipeline, swappable context.
- **Pipeline** (agents + `pipeline.md`): same for every clip.
- **Context** (`context/active/`): swap per business, campaign or owner voice.
- **Raw data**: per clip, in `runs/<date>_<name>/00_raw/`.

## Principles
1. Agents hand off through files. Each reads the previous step's file and writes its own.
2. No company facts inside agents. All read `context/active/`.
3. Three human gates: after idea choice, after script review, before publishing. AI never posts.
4. Every fact needs a source in `00_raw/` or context. Missing or unconfirmed = `[UNVERIFIED]`.

## Layout
```
video-agents/
├── CLAUDE.md          orchestrator rules
├── pipeline.md        flow, I/O table, gates
├── .claude/agents/    8 agent specs
├── context/active/    brand, audience, voice, dos-donts, asset-library, learnings
├── templates/         brief, script, storyboard
└── runs/_template/    copy per clip (00_raw, 06_assets, status.md, 09_results.md)
```

## Use
1. Copy `runs/_template/` to `runs/<date>_<name>/`.
2. Put raw data in `00_raw/` (notes, numbers, photos/videos, customer questions, links).
3. Open this folder in Claude Code and say: `make a clip from runs/<folder>`.
4. The orchestrator runs the steps and stops at each gate.
5. After posting, fill `09_results.md` with real numbers; the analyst updates `learnings.md`.

## Language
Agent instructions and working files are English (cheaper). Clip output (spoken lines, on-screen text, subtitles, captions) uses the **output language** set in `context/active/brand.md` (default Thai). Replies to you follow the language you write in.

## Swap context
Replace files in `context/active/` (keep the old set in `context/<name>/`). Owner voice: add real samples to `voice.md`. Never mix two context sets.

## Scope
The system produces production-ready plans and prompts. Video generation runs in an external AI video tool you choose. Real project footage is always used for real work; AI is for explainers, graphics and labeled illustrations.
