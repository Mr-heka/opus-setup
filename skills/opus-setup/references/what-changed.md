# What changed in Opus 5.5

A short summary of Anthropic's own guidance (September 2026), in plain words. Sources are linked at the bottom.

## How to ask

- **Give it the goal and what "done" looks like, not the steps.** Opus 5.5 works out the path itself and handles long, multi-part jobs well.
- **Stop saying "think hard" or "make no mistakes".** It always thinks, and scales how much by itself. These lines just make replies start later.
- **Ask for the finished thing** (the spreadsheet, the report, the page), not an outline.
- **Send the real material.** It reads charts, screenshots and dense documents accurately. Context is the biggest lever.
- **Explain why a rule exists.** A rule with its reason works better than a bare ban.

## Effort

- **Medium is the default and the sweet spot.** In Anthropic's testing, Opus 5.5 on medium matched or beat the previous Opus on high.
- To make it think less, lower effort rather than adding instructions.

## How instructions should be written

- **Short.** Anthropic's target is under about 200 lines per CLAUDE.md; longer files make Claude ignore rules. For each line, ask: would removing it cause a mistake? If not, cut it.
- **Calm.** "CRITICAL / MUST / NEVER" on many lines makes newer models overreact, and nothing stands out.
- **No contradictions.** When two rules disagree, Claude may follow either one.
- **Retire old workarounds.** Forced double-checks and "if in doubt, use this tool" lines written for older models now cause over-checking.

## Sources

- Anthropic, "Prompting Claude Opus 5.5": https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/prompting-claude-opus-5-5
- Anthropic, "Prompting best practices": https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/claude-prompting-best-practices
- Anthropic, "Effort": https://platform.claude.com/docs/en/build-with-claude/effort
- Claude Code, "Memory and CLAUDE.md": https://code.claude.com/docs/en/memory
- Claude Code, "Best practices": https://code.claude.com/docs/en/best-practices
