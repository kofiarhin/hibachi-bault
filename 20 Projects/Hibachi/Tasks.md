---
type: task-list
project: Hibachi
status: active
updated: 2026-08-09
source: kofiarhin/ideahub/projects/hibachi.md
tags:
  - project/hibachi
  - task
---

# Hibachi Tasks

Search tags: #project/hibachi #task #status/active #software-delivery-loop #accessibility

Only current actionable work uses unchecked checkboxes in this note.

## High priority

- [ ] Create and review an implementation-ready Software Delivery Loop v1 technical specification #priority/high
- [ ] Prove Software Delivery Loop v1 end-to-end on one real repository request with exact retained evidence #priority/high
- [ ] Verify the complete delivery loop can be operated by voice or keyboard without reading terminal output #priority/high
- [ ] Run the complete native-Windows verification suite against the exact current application revision #priority/high
- [ ] Reconcile the Hibachi implementation-package state and historical verification evidence with the current Software Delivery Loop v1 direction #priority/high
- [ ] Configure `OBSIDIAN_VAULT_PATH` to this vault and verify `Vault Index.md`, targeted retrieval, note capture, and the on-demand daily brief #priority/high

## Medium priority

- [ ] Record keyboard-only, screen-reader-compatible, spoken-progress, cancellation, error-recovery, and no-terminal-reading accessibility evidence #priority/medium
- [ ] Verify targeted Vault retrieval returns the Working Profile, Projects Index, Hibachi project note, and Engineering Defaults #priority/medium
- [ ] Verify safe Obsidian note creation and append against a disposable test note #priority/medium
- [ ] Verify governed overwrite, move, and delete operations create recoverable backups and enforce approval #priority/medium
- [ ] Recheck unresolved ElevenLabs-specific verification items against the exact current application revision before carrying them forward #priority/medium
- [ ] Decide whether to bundle a compatible redistributable wake-word model or retain push-to-talk as the reliable fallback #priority/medium

## Completed / retained evidence

- [x] Create the local-first Hibachi application repository and implementation foundation
- [x] Implement the React client, companion service, shared schemas, policies, MongoDB models, and test structure
- [x] Implement deterministic `Vault Index.md` retrieval and targeted Markdown note search
- [x] Implement safe note creation, append, and governed high-risk vault operations with backups
- [x] Implement pairing, session, CSRF, origin, WebSocket, redaction, and policy-integrity controls
- [x] Improve coding-agent readiness detection and subprocess failure diagnostics
- [x] Replace the initial dashboard with the immersive visualizer and command interface
- [x] Populate the vault with curated operating context and project routing
- [x] Merge the strategic Hibachi product PRD through application pull request #9
- [x] Establish Software Delivery Loop v1 as the active product milestone
- [x] Implement ElevenLabs TTS with server-side credential isolation and streamed audio
- [x] Record local client tests, server tests, root typecheck, lint, and production build evidence for the 2026-08-03 ElevenLabs work

## Related notes

- [[20 Projects/Hibachi/Project]]
- [[20 Projects/Hibachi/Logs/2026-08-03 ElevenLabs TTS]]
- [[20 Projects/Projects Index]]
- [[Vault Index]]
