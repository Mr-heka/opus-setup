# Working with Opus 5.5: a plain-English guide

Use this to answer questions about Opus 5.5, such as "how should I ask it for a report?", "which effort level?" or "why does it ignore my rules?". It summarises Anthropic's own guidance from September 2026. Answer from this page, say when something isn't covered, and point to the sources at the bottom for full detail.

## How to ask it for work

**In short:** give it the goal and what "done" looks like in one message, hand it the real material, and leave out the steps and the "think hard" lines.

- **Outcome and finish line up front.** Say what you want back and what it must include, in the first message. It carries long, multi-part work well, so you don't need to feed it one step at a time.
- **Don't map the path.** "Look in this sheet, then this PDF, then…" usually does worse than describing the result and letting it work out the approach. Keep numbered steps only where the order really matters.
- **Drop "think hard", "think carefully" and "make no mistakes".** It always thinks, and decides how much for itself. Those lines just make the first reply slower.
- **Ask for the finished thing.** The spreadsheet, the proposal, the report, not an outline of one.
- **Give it the real material.** Files, connected tools, screenshots, the customer's actual email. Anthropic calls context the single biggest lever.
- **Explain why.** A rule with its reason ("show me client emails first, they can't be unsent") generalises better than a bare ban.
- **Say what to do, not what not to do.** The exception is design, where a list of looks to avoid works well.

Example: instead of "help me with a proposal", try "Create a proposal I can review and send to this client. Use their email and our pricing sheet in this folder. Include price, what's included, timeline and next step. Check the totals and flag anything missing."

## Effort: how hard it thinks

**In short:** medium by default. Raise it only where you've seen a real gain.

- Opus 5.5 defaults to medium. In Anthropic's testing, medium matched or beat the previous Opus on high for coding and knowledge work.
- Effort is the dial. Lowering it cuts thinking more reliably than any instruction does.
- At the same setting it thinks more than older models did, so carrying over "high" or "max" costs more than it used to.
- The top settings won't always give a much better result. Keep them for long, hard jobs where you've seen the difference.
- Effort changes everything about a reply: how many tools it uses, how long the summary is, how much it explains.

## Writing instructions it actually follows

**In short:** fewer, calmer, specific rules, each with its reason.

- **The pruning test:** would removing this line cause a mistake? If not, cut it. A long file makes Claude miss the rules that matter. Anthropic's target is under about 200 lines.
- **If it keeps breaking a rule it has, the file is probably too long.**
- **Shouting stopped working.** "CRITICAL / MUST / NEVER" on many lines makes newer models overreact. Save emphasis for the one line that keeps getting skipped.
- **Contradictions get resolved at random.** If two rules disagree, Claude may follow either. Read the file for stale or clashing rules.
- **Make rules checkable.** "Show me every client email before sending" beats "be careful with emails".
- **Retire old workarounds.** Lines written to push older models ("be thorough", "double-check everything", "summarise every few steps", "if in doubt, use this tool") can now cause over-checking. Re-test rather than carry them over.
- In recent Claude Code versions, `/doctor prompt-audit` scans instruction files for old-model wording and contradictions and suggests edits.

## Design, visuals and reports

**In short:** show it examples, name the looks you don't want, hand it screenshots directly, and ask for the finished file.

- Without direction it falls back to a few default styles, and "avoid a generic look" just swaps one default for another. Name the specific looks you don't want, and add to the list after each round.
- For a brand, written rules work, or point it at a folder of examples you like.
- It reads dense charts and screenshots accurately, so send them as they are. No need to retype numbers.
- Reports should lead with the point: what it did, what it found, what it needs from you.
- It's good at catching mistakes in long documents, like a chart that doesn't match its numbers. Ask it to check.

## Not covered here

Pricing, API details and team-wide setups (rules per folder, large skill libraries, memory structure, agents) are outside this guide. Say so rather than guessing, and point to the sources.

## Sources

- Anthropic, "Prompting Claude Opus 5.5": https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/prompting-claude-opus-5-5
- Anthropic, "Prompting best practices": https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/claude-prompting-best-practices
- Anthropic, "Effort": https://platform.claude.com/docs/en/build-with-claude/effort
- Claude Code, "Memory and CLAUDE.md": https://code.claude.com/docs/en/memory
- Claude Code, "Best practices": https://code.claude.com/docs/en/best-practices
- Anthropic webinar, "Opus 5.5 for Work" (25 September 2026): https://www.anthropic.com/webinars/opus-5-5-for-work
