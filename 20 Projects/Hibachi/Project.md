---
type: project
project: Hibachi
status: active
created: 2026-08-01
updated: 2026-08-09
sources:
  - kofiarhin/hibachi
  - kofiarhin/hibachi-vault
  - kofiarhin/ideahub/projects/hibachi.md
tags:
  - project/hibachi
  - status/active
---

# Hibachi

Search tags: #project/hibachi #status/active #local-first #voice #operational-agent #software-delivery-loop #accessibility #elevenlabs

## Outcome

Build a local-first, voice-first personal operating agent for one owner on native Windows. Hibachi should preserve Kofi's projects, standards, priorities, workflows, and skills, then safely execute repeatable work through governed tools with minimal dependence on visual interaction.

The immediate product goal is Software Delivery Loop v1: safely run the complete software-development delivery loop from idea and project context through specification, approved implementation, verification, commit, branch push, draft pull request, spoken completion report, and retained evidence.

## Current state

- Application repository: https://github.com/kofiarhin/hibachi
- Vault repository: https://github.com/kofiarhin/hibachi-vault
- Lifecycle: active.
- Current stage: Software Delivery Loop v1.
- The application repository contains the React/Vite client, localhost Node.js companion service, shared schemas, MongoDB models, governed tools, policy enforcement, Obsidian integration, startup scripts, and test suites.
- Hibachi application `main` includes the strategic product PRD through merged pull request #9 at commit `8ff40dff6a74459253b589b1777ca9138a5e5cc7`.
- The current implementation records unified first-person Hibachi behaviour, deterministic and provider routing, governed workspace writes, and compact live workflow feedback.
- The interface supports typed commands, push-to-talk, an immersive visualizer, workflow feedback, approval controls, and spoken-output integration.
- Hibachi uses deterministic routing for known actions, NVIDIA for conversational reasoning when configured, and Codex for repository analysis and implementation proposals.
- Reasoning providers propose; Hibachi validates and executes through typed, allowlisted tools.
- The companion service remains bound to `127.0.0.1` and protects state-changing work with the Grill, execution contracts, approval, workspace boundaries, Git safety, and protected-file rules.
- ElevenLabs TTS was implemented on application `main` at commit `0b29390690a731383293cfeecf0f677953d8f826`.
- The Vault retains the 2026-08-03 ElevenLabs implementation and verification record in [[20 Projects/Hibachi/Logs/2026-08-03 ElevenLabs TTS]]. That log remains historical evidence and does not override newer Ideas Hub product priorities.
- Complete native-Windows verification against the current application revision has not been recorded in Ideas Hub.
- The full Software Delivery Loop v1 has not yet been proven end-to-end on a real repository request with retained evidence.
- The application is not publicly deployed.

## Current focus

- Create and review an implementation-ready Software Delivery Loop v1 technical specification.
- Prove Software Delivery Loop v1 end-to-end on one real repository request with exact retained evidence.
- Make the full workflow operable through voice or keyboard without requiring terminal reading.
- Run the complete native-Windows verification suite against the exact current application revision.
- Reconcile existing Hibachi implementation-package state and historical verification evidence with the current Software Delivery Loop v1 direction.
- Configure `OBSIDIAN_VAULT_PATH` to the local clone of this repository and verify `Vault Index.md`, targeted retrieval, note capture, and the on-demand daily brief.
- Keep unresolved ElevenLabs-specific verification items tracked as implementation verification debt rather than the primary product milestone.

## Canonical links

- Tasks: [[20 Projects/Hibachi/Tasks]]
- Latest retained TTS log: [[20 Projects/Hibachi/Logs/2026-08-03 ElevenLabs TTS]]
- Portfolio: [[20 Projects/Projects Index]]
- Vault routing: [[Vault Index]]
- Working profile: [[40 Resources/Operating Context/Working Profile]]
- Engineering defaults: [[60 Decisions/Engineering Defaults]]

## Product scope

### Active scope

- Local React browser application served by the companion service.
- Local Node.js companion service bound to `127.0.0.1`.
- Voice and typed interaction with concise spoken feedback.
- One active registered workspace at a time.
- Conversation and project context.
- Local `whisper.cpp` transcription.
- ElevenLabs spoken output with server-side credentials and ephemeral streamed audio.
- MongoDB conversation and workflow history.
- Obsidian long-term knowledge retrieval and governed note capture.
- Deterministic routing and governed reasoning-provider use.
- Brainstorming, requirements, specification, and implementation planning.
- Grill, execution contracts, explicit approval, and protected-change confirmation.
- Typed filesystem and command tools.
- Git checkpoints and non-main task branches.
- Tests, lint, type checks, builds, and browser verification.
- Approved commits, branch pushes, and draft pull requests.
- Action history, artifacts, and retained evidence.
- Cancellation, timeout, pause, and safe recovery.
- Read-only public web research through isolated Crawlee and Playwright.

### Deferred

- Unrestricted laptop access.
- Gmail and calendar workflows.
- Broad administration automation.
- Marketing campaign execution.
- Content publishing and media-production automation.
- Multiple concurrent executing projects.
- Autonomous background work and scheduled monitoring.
- Telegram and mobile interfaces.
- Production deployments.
- Pull-request merging.
- Personality imitation.

## Durable decisions

- Hibachi is a governed personal operating agent, not a generic chatbot or unrestricted desktop agent.
- Software Delivery Loop v1 is the active milestone.
- The current autonomy target is a controlled operator: Hibachi may run allowlisted tools inside registered workspaces after governed approval.
- Windows is the first supported operating system; Chrome is the default browser and Edge remains a supported fallback.
- Use one root `package.json` with npm workspaces for `client`, `server`, and `packages/shared`.
- Use MongoDB for operational history and Obsidian for user-owned durable knowledge.
- Use `kofiarhin/hibachi-vault` as the canonical GitHub repository for this curated vault.
- Read `Vault Index.md` first, then use targeted folder, filename, tag, link, and text search.
- Do not load the entire vault by default and do not use embeddings or a vector database in the MVP.
- ElevenLabs is the spoken-output provider recorded by the current implementation; credentials remain server-side and generated audio is not persisted.
- If speech output is unavailable, unrelated safe text workflows should remain usable.
- Reasoning providers propose; Hibachi validates and executes through typed allowlisted tools.
- Clear, low-risk, reversible, read-only work may proceed directly.
- Materially ambiguous, state-changing, risky, destructive, costly, credential-sensitive, Git-write, deployment, or externally consequential work triggers the Grill.
- Code-changing workflows use a clean repository, Git checkpoint, and non-main task branch.
- Verification evidence is required before completion is claimed.
- Commit, push, draft pull request, merge, and deployment authorities remain distinct.
- Direct protected-branch writes, merges, production deployments, arbitrary shell execution, and administrator operations remain blocked or separately gated inside Hibachi's governed execution model.
- Non-visual operation is a core acceptance boundary, not deferred interface polish.

## Accessibility requirements

Hibachi must support:

- voice or keyboard operation for every important workflow;
- no critical action that depends only on a visual control;
- concise and interruptible spoken status updates;
- optional detailed spoken explanations;
- repeat-back confirmation for risky actions;
- large scalable text and strong contrast;
- semantic screen-reader-compatible structure;
- predictable focus management;
- interruption, pause, cancellation, and resume commands;
- spoken error recovery and next-step guidance;
- outcome-focused summaries instead of requiring terminal-log inspection;
- accessible approval and protected-change confirmation flows.

## Software Delivery Loop v1

```text
Idea
→ Brainstorm
→ Research
→ Requirements
→ Specification
→ Implementation plan
→ Grill when materially required
→ Execution contract
→ Approval
→ Task branch
→ Code changes
→ Tests, lint, type checks, and build
→ Browser verification when relevant
→ Commit
→ Branch push
→ Draft pull request
→ Spoken completion report
→ Retained evidence
```

The milestone is complete only when the full workflow can be operated without reading terminal output and exact actions, changed files, verification results, artifacts, branch, commit, and pull-request evidence are retained.

## Known limitations

- Complete native-Windows runtime verification against the current application revision has not been recorded.
- The full Software Delivery Loop v1 has not yet been proven end-to-end with retained evidence.
- Complete non-visual operation has not yet been verified with keyboard-only, screen-reader-compatible, spoken-progress, cancellation, error-recovery, and no-terminal-reading evidence.
- A redistributable wake-word model is not recorded as bundled; push-to-talk remains the reliable fallback.
- ElevenLabs speech requires internet access and available account quota.
- Gmail, Calendar, Telegram, proactive scheduling, production deployment, and PR merge are outside the current MVP scope.
- The application is not publicly deployed.

## Evidence

- Canonical Ideas Hub record: `kofiarhin/ideahub/projects/hibachi.md`, updated 2026-08-05.
- Strategic product PRD merged into `kofiarhin/hibachi` through pull request #9 at commit `8ff40dff6a74459253b589b1777ca9138a5e5cc7`.
- ElevenLabs implementation commit on application `main`: `0b29390690a731383293cfeecf0f677953d8f826`.
- Vault TTS evidence: [[20 Projects/Hibachi/Logs/2026-08-03 ElevenLabs TTS]].
- Canonical vault repository: `kofiarhin/hibachi-vault`.
