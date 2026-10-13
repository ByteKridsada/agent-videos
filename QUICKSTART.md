# How to Run a Clip

## What this system does
You give it raw material. It writes the script, plans every shot, and tells you exactly how to edit the video. You do the final edit and post it yourself.

---

## Step 1 — Set up your run folder
Copy the template folder and rename it:
```
runs/_template/  →  runs/2026-10-13_my-clip/
```
Drop your raw material into `runs/2026-10-13_my-clip/00_raw/`
(notes, numbers, links, images, transcripts — anything relevant)

---

## Step 2 — Start the pipeline
Open this project in Claude Code and type:
```
make a clip from runs/2026-10-13_my-clip
```

---

## Step 3 — Three stops where you decide

The system runs automatically but pauses at three gates:

| Gate | What you do |
|------|-------------|
| **Gate 1** | Pick one idea from the list it gives you |
| **Gate 2** | Read and approve the script |
| **Gate 3** | Watch your finished edit, then approve before posting |

---

## Step 4 — Edit and post
Use the files the system produces as your guide:
- `07_edit.md` — shot order and edit instructions
- `08_publish.md` — caption, hashtags, thumbnail text

Do the edit in your video tool of choice, then post it yourself.

---

## Step 5 — Log the results
After posting, fill in `runs/<your-folder>/09_results.md` with real numbers (views, reach, etc.).
Then tell Claude: `analyze results for runs/<your-folder>` — it will save lessons for future clips.

---

## File map
```
runs/<your-clip>/
├── 00_raw/          your input files
├── 01_brief.md      facts pulled from your raw data
├── 02_ideas.md      clip concepts to choose from
├── 03_script.md     full script with spoken lines
├── 04_review.md     fact-check results
├── 05_storyboard.md shot-by-shot breakdown
├── 06_assets/       style guide and shot prompts
├── 07_edit.md       edit instructions (your guide in the editor)
├── 08_publish.md    caption, hashtags, thumbnail text
├── 09_results.md    you fill this after posting
└── status.md        tracks which step you're on
```
