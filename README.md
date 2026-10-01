# Opus 5.5 Setup

Claude Opus 5.5 does its best work when you give it the goal, tell it what finished looks like, and let it run. Most instruction files were written for older models: long, full of ALL-CAPS rules and old workarounds. On Opus 5.5 that makes Claude stop halfway, over-check, or write walls of text.

This kit gives you a short instructions file built for how Opus 5.5 works, and a skill that fits it to you:

- It reads the instructions file you already have and backs it up first.
- It asks you up to three quick questions about how you work.
- It rewrites the file into a short version with the Opus 5.5 working habits built in, keeping every rule you rely on.
- It offers to set Claude Code to the latest Opus at medium effort, Anthropic's recommended default.

That's it. It touches one file (plus two settings if you say yes), and you can put the old one back at any time.

**You need:** Claude Code or Codex. No API keys.

## Install

Copy the prompt in [SETUP-PROMPT.md](SETUP-PROMPT.md) into a new Claude Code or Codex session. Then start a new session and say:

> Set me up for Opus 5.5

## Just want the template?

It's in [`claude-md-template.md`](skills/opus-setup/references/claude-md-template.md). Fill in the brackets yourself and save it as `~/.claude/CLAUDE.md`.

## What it's based on

Anthropic's own guidance for Opus 5.5. A plain-English summary with links is in [`what-changed.md`](skills/opus-setup/references/what-changed.md).

Made by Selr AI.
