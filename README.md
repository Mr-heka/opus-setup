# Opus 5.5 Setup

Claude Opus 5.5 does its best work when you give it the goal, tell it what finished looks like, and let it run. Most instruction files were written for older models: long, full of ALL-CAPS rules and old workarounds. On Opus 5.5 that makes Claude stop halfway, over-check, or write walls of text.

This kit installs one skill that sets you up for Opus 5.5 in a single session:

- **Scores your setup** out of 6 for Opus 5.5, and tells you in plain words what's holding it back.
- **Rewrites your instructions file** into a short version with the Opus 5.5 working habits built in, keeping every rule you rely on. It backs up the old one first.
- **Writes three ready-to-copy prompts for your own work**, in the shape Opus 5.5 does its best work with: the whole job, the right information, a clear finish line.
- **Sets Claude Code to the latest Opus at medium effort**, Anthropic's recommended default (only if you say yes).
- **Answers your Opus 5.5 questions** afterwards, from a plain-English guide built on Anthropic's own advice.

It touches your instructions file and one new prompt file (plus two settings if you say yes), and you can put everything back at any time.

**You need:** Claude Code or Codex. No API keys.

## Install

Copy the prompt in [SETUP-PROMPT.md](SETUP-PROMPT.md) into a new Claude Code or Codex session. Then start a new session and say:

> Set me up for Opus 5.5

## Just want the template?

It's in [`claude-md-template.md`](skills/opus-setup/references/claude-md-template.md). Fill in the brackets yourself and save it as `~/.claude/CLAUDE.md`.

## What it's based on

Anthropic's own guidance for Opus 5.5. A plain-English guide with links is in [`opus-guide.md`](skills/opus-setup/references/opus-guide.md).

Made by Selr AI.
