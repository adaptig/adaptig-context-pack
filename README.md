# Adaptig Context Pack

This folder is the canonical reference for Adaptig company facts. Any team member's agent — Claude Code, Copilot, Gemini, or anything else — should read these files before generating content on behalf of Adaptig.

## Files

- **`adaptig.md`** — Spine. Start here. Entity, tagline, mission, and how the rest of the pack is organized.
- **`team.md`** — Core management team with roles.
- **`vision.md`** — What Adaptig is building and why.
- **`product.md`** — Spark / Shift / Shape / Show product lines, the 100-10-10-100 adoption framework, training pipeline, and trainer economics.
- **`brand-tone-of-voice.md`** — How Adaptig communicates.
- **`brand-visual-style.md`** — Logo, typography, color palette, illustration style, and relative file paths to all visual assets in `brand-assets/`.
- **`achievement.md`** — Verified track record numbers. Use these, not approximations.
- **`brand-assets/`** — Logos, fonts, shapes, illustration references, call backgrounds, LinkedIn backgrounds, email signatures. `brand-visual-style.md` serves as the index.

## Company presentation

The canonical company presentation is stored in the shared Google Drive, not in this repo (file size is too large for git).

Drive folder: [01 Company Presentation](https://drive.google.com/drive/folders/1sTPpF7j40ySIHraLA9ziNA69q85uOIyx).

- **English master** — [`20260416_Adaptig company presentation_long with video.pptx`](https://docs.google.com/presentation/d/1FhSXk3jGapoEWoqHgfEHt33Ct3QATYqP/edit) (35 slides, 99 MB, includes embedded intro video and speaker notes).
- **German version** — [`Adaptig_Company_Presentation_DE_20260416.pptx`](https://docs.google.com/presentation/d/105tYC9bLNuB7iPiks8itVoft6U6w3XY2/edit) (same structure, translated by Gemini 3 Pro Preview with the Adaptig terminology lock — formal Sie, Spark/Shift/Shape/Show kept English, SMART+SZENE acronyms, anti-hype voice).

Both decks should be kept in sync with this pack. If you update the deck, update the pack file that covers the same claim (e.g., a new program → `product.md`; a new team member → `team.md`; a new headline number → `achievement.md`). The pack is the source of truth for facts; the deck is the presentation of those facts.

## Quick setup: Claude Code

### 1. Clone the repo

```
git clone git@github.com:adaptig/adaptig-context-pack.git ~/adaptig-context-pack
```

### 2. Reference from your project

Add this line to your global instructions file (`~/.claude/CLAUDE.md`) or to a project-specific `CLAUDE.md`:

```
For Adaptig company context, read the files in ~/adaptig-context-pack/ before generating any Adaptig-facing content. Start with adaptig.md (the spine file) and read whichever other files are relevant to the task.
```

### 3. Verify it works

Open Claude Code and ask: "What is Adaptig's tagline?" It should answer "AI adoption that sticks" without you having to tell it.

### 4. Keep it updated

Pull the latest version periodically:

```
cd ~/adaptig-context-pack && git pull
```

## Setup for other agents

- **Claude Co-worker**: Add the folder as a reference file set in your project settings.
- **GitHub Copilot**: Reference the folder in your `.github/copilot-instructions.md` or Copilot instructions.
- **Other agents**: Follow their context-loading convention — most support pointing at a local folder of reference files.

## Golden rule

Every fact in these files is either sourced or flagged. If you disagree with a fact, **fix the file** rather than arguing in chat. The pack is canonical by design — discussions become distributed across channels, but the file is one place and one state.

## What's NOT in this pack

- Personal workflows and operator-specific skills — those live in each team member's personal context folder.
- Client-specific information, NDAs, client pricing, or engagement contracts — those live in internal systems, not here.
- Financial, investor, or fundraising information — not a team-facing concern.

## Maintenance

- **Who can update**: Any core team member via pull request.
- **Who approves**: Sam or Jan-Eric must approve changes to factual claims (numbers, client names, product definitions).
- **When to update**: After major client wins, team changes, product launches, or brand decisions.
- **How to flag uncertainty**: If a fact seems wrong, open an issue or comment in the PR — do not silently change numbers or claims.

## Version

- **Drafted:** 2026-04-08
- **Published to company GitHub:** 2026-04-15
- **Last reviewed:** 2026-04-15
