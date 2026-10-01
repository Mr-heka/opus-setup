# Set up Opus 5.5 Setup

You are installing this kit on the user's machine. Paths that don't start with `~` are relative to this repo.

## 1. Install the skill

Copy `skills/opus-setup/` to `~/.claude/skills/opus-setup/`, replacing an older copy of this same skill if one is there. Create `~/.claude/skills/` if it's missing.

If Codex is installed (`~/.codex` exists), copy the same folder to `~/.codex/skills/opus-setup/` as well.

Change nothing else. Installing this kit does not touch the user's instructions or settings; the skill only does that later, when they ask for it and say yes.

## 2. Check

1. `~/.claude/skills/opus-setup/SKILL.md` exists and matches this repo's copy (and the Codex copy, if you made one).
2. Count the lines in the user's current instructions file (`~/.claude/CLAUDE.md`, or `~/.codex/AGENTS.md` in Codex) without changing it. If there isn't one, note that.

## 3. Report

Tell the user, briefly:

- the skill is installed (and where);
- how long their current instructions file is (or that they don't have one yet);
- next step: start a new session and say "Set me up for Opus 5.5". It backs up the file before changing anything.

## Removing

Delete `~/.claude/skills/opus-setup/` (and `~/.codex/skills/opus-setup/` if present). Backups the skill made stay in `~/.claude/backups/`.
