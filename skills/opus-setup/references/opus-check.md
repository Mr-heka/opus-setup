# The Opus 5.5 check

Six yes/no checks on the main instructions file, one point each. Score the file before the rewrite and again after. A missing file scores 0.

| # | Check | Passes when |
|---|---|---|
| 1 | **Short** | Under about 150 lines. |
| 2 | **Calm** | No more than two ALL-CAPS pressure words (MUST, NEVER, CRITICAL, IMPORTANT, ALWAYS) in the whole file. |
| 3 | **No old-model habits** | No "think hard / carefully / step by step", "make no mistakes", forced double-check or "summarise every few steps" lines. |
| 4 | **Current** | No pinned old model names (for example claude-3, sonnet-4, opus-4) and no "if in doubt, use X" tool pushes. |
| 5 | **Consistent** | No two rules that contradict each other (for example "never long replies" and "explain everything in full detail"). |
| 6 | **Built for how Opus 5.5 works** | Tells Claude to work out the goal and finish line itself, finish the job, and look for context before asking; and every red line has its reason. |

When showing the score, give one plain line per missed check, naming the actual line from their file where possible. Example:

> **Your setup scores 2/6 for Opus 5.5.**
> - 42 lines of rules is fine, but 11 of them are in capitals, so none of them stand out.
> - "Think step by step before every answer" slows every reply and no longer helps.
> - It pins claude-3-5-sonnet, an older model.
> - "Never write long replies" and "explain your reasoning in full detail" pull against each other.
