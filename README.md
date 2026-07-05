LEDGER.md is a chronological record of what agents have done in the repository. It differs from git commit logs, which capture the state of the code and are shaped by version control. Ledger entries capture the work behind the changes: what happened, when it happened, and which agent did it.

Each entry should be small and focused. Some entries may correspond to code changes, while others may document work that leaves no trace in git, such as investigations, decisions, or notes. Because one commit can involve several separate actions, the ledger makes it easier to connect individual pieces of work to the surrounding git history.

The result is a more detailed trail of how the repository evolved and a quick way for the next agent to get oriented.

```
Date: 07-05-2026
Claude: 14:32 : Fixed source type mismatch in ingest classifier. Updated card chip mapping to follow the canonical table.

Codex: 13:10 : Refactored archive filename parser to handle underscores in dates. Added two unit tests.

Claude: 11:47 : Investigated duplicate entries in import pipeline. Root cause is double-fired watcher event, wrote findings to import-dedup-2026-07-05.md.

Codex: 10:05 : Cleaned up export CSV headers to match canonical column order. No logic changes.

Claude: 09:18 : Added validation for missing source type on card creation. Rejects with a clear error instead of defaulting silently.
```