# Daily case-study reconciliation protocol
Status: connector-assisted scheduled reconciliation; unattended end-to-end execution NOT verified.
Automation: 6ad5debc43888191a1886a433fee82c4, existing daily schedule in Asia/Calcutta.

## Boundaries and revisions
GitHub is canonical. Notion page 377ce6de608980daae89e74da8236287 is the KM hub.
The exact text BEFORE the separator and heading "Original OmniVerse Notion Research — Preserved Below" maps to sync/notion-narrative.md. Everything from that heading onward is protected original research, including child pages and attachments. Never replace the whole page. New research remains in Notion until explicitly reconciled into a canonical section; never blindly copy the whole page into a public repository.
sync/state.json stores the last verified narrative, Notion revision, and canonical file blob SHAs. Git history preserves revisions.

## Run algorithm
1. Read this protocol, state, every changed canonical file and full Notion page. Stop with failure notification if any fetch is incomplete/truncated or unavailable.
2. Compare exact mapped narrative against state.baseline_narrative on both sides. Formatting-only differences must be reviewed rather than silently normalized.
3. Neither changed: no-op. GitHub only changed: targeted Notion replacement of the old mapped narrative. Notion only changed: inspect for contradictions with canonical master/personas; if consistent, update mapped GitHub file using current blob SHA. Both changed identically: verify and advance state. Both changed differently: no content write; log a conflict with both revisions and excerpts.
4. Changes in canonical files outside the narrative require explicit source-to-narrative reconciliation. Use stable OVE IDs and the six acts. If the narrative also changed in a related passage, hold that passage as conflict. Never infer approval of new financial values or select one disputed source value.
5. Re-fetch destination immediately before each mutation; abort on revision drift. Use GitHub SHA checks. Notion tool writes do not provide an atomic compare-and-swap: a concurrent edit race remains a limitation. Use smallest exact targeted edits; do not claim transactional consistency.
6. Re-fetch both after each write. Require exact mapped text equality and unchanged protected research. Advance baseline ONLY after read-back verification. On partial failure retain the prior baseline and log pending recovery; next run must reconcile actual destinations before retry.
7. Write a new sync/logs/<UTC timestamp>-<run-id>.md with outcome, source/destination revisions, before/after details, conflicts, errors and direct links. No-op runs also log. Use unique paths, do not erase earlier logs. Log failures in GitHub when accessible; otherwise report in the automation response.
8. Notify the user in the automation result for every failure, conflict or partial write. Include the affected links and recovery action. Email/WhatsApp delivery and platform-level missed-run alerts are not configured. Never claim a successful integration merely because a task exists.
9. Update state through its current SHA only after success; preserve per-file baselines for held conflicts. Never advance unresolved source SHAs.

## Future Notion-link-only intake
Fetch the supplied page; identify sector/company from evidence; locate existing matching case before creating one. Create/update its sector folder, 22-section master, executive brief, fictional personas, simulations, seven stream blueprints and evidence/resource registers. Preserve original research. Label invented facts and unavailable assets. Link the Notion narrative to GitHub and register a per-case baseline before including it in scheduled reconciliation. Ambiguous sector or contradictory facts stay in the gap register. Scope of this automation currently covers OmniVerse only.

## Acceptance tests
Manual connector transfer: CDIO correction GitHub→Notion; audit note Notion→GitHub; both read back; protected research unchanged.
Still required: first unattended scheduled execution, injected concurrent conflict, partial-write recovery, notification delivery and missed-run monitoring. This protocol is an agent workflow, not a deployed API synchronization service.
