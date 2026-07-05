

Add this to your AGENTS.md:

## Ledger
LEDGER.md is the shared memory for agents, kept as a captain's log. Read it to catch up; write to it when you're done.

### Must
- Record every change/fix in LEDGER.md: concise, 1-2 sentences max.
- Always append: newest entries at the bottom, grouped under the current date.
- Leave one blank line above each new date group before writing entries.
- Never guess dates/times: get them from the system (`date`) before writing.
- Entry format:

      Date: MM-DD-YYYY
      Agent {Claude, Codex, ...}: hh:mm : Concise summary of what was done

```
Date: 07-05-2026
Claude: 14:32 : Fixed source type mismatch in ingest classifier. Updated card chip mapping to follow the canonical table.

Codex: 13:10 : Refactored archive filename parser to handle underscores in dates. Added two unit tests.

Claude: 11:47 : Investigated duplicate entries in import pipeline. Root cause is double-fired watcher event, wrote findings to import-dedup-2026-07-05.md.

Codex: 10:05 : Cleaned up export CSV headers to match canonical column order. No logic changes.

Claude: 09:18 : Added validation for missing source type on card creation. Rejects with a clear error instead of defaulting silently.
```