# Adaptig Context Pack

This folder is the canonical reference for Adaptig company facts. Any team member's agent — Claude Code, Copilot, Gemini, or anything else — should read these files before generating content on behalf of Adaptig.

## Files

- **`adaptig.md`** — Spine. Start here. Entity, tagline, mission, and how the rest of the pack is organized.
- **`team.md`** — Core management team with roles.
- **`vision.md`** — What Adaptig is building and why.
- **`product.md`** — Spark / Shift / Shape / Show product lines, the 100-10-10-1 adoption framework, training pipeline, and trainer economics.
- **`brand-tone-of-voice.md`** — How Adaptig communicates.
- **`brand-visual-style.md`** — Logo, typography, color palette, illustration style, canonical asset locations.
- **`achievement.md`** — Verified track record numbers. Use these, not approximations.

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
