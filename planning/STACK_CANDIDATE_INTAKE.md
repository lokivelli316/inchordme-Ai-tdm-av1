# AI Rumble — Stack Candidate Intake

Status: **CANDIDATE / PRE-PROMOTION**  
Purpose: keep useful donor builds, skills, behaviors, and integration surfaces from disappearing back into chat history.

Nothing in this registry is represented as IMPLEMENTED merely because it is named here.

## Stack rule

Candidate intake is additive.

A candidate keeps its own identity, architecture, lineage, assets, terminology, working behavior, and provenance until inspection establishes the exact preservation and adapter boundaries.

Candidate does not mean rewrite target.

Candidate does not mean permission to flatten several projects into one generic subsystem.

Candidate does not mean VERIFIED.

## Existing landed/proposed foundation

- AI Rumble public foundation
- Receipt Hunters Gallery
- Source Integration Planning
- Infinite Brain public-safe federated architecture
- Shared Skills registry
- `be-ambitious` — PROPOSED
- `no-flatten` — PROPOSED

These are existing surfaces. New candidates integrate around them rather than replacing them.

## Donor-build candidates

### CAND-SRC-001 — ACATMO + Organizer

Candidate roles:

- integrity/provenance
- artifact vault
- ZIP-as-folder behavior
- cache behavior
- content identity
- organization/indexing
- duplicate control

Preservation boundary: inspect existing ACATMO/Organizer source before changing architecture. Existing behavior remains the source of truth for what is already built.

### CAND-SRC-002 — Tab Orchestrator

Candidate role: browser/tab coordination and operator-facing orchestration.

Preservation boundary: retain its actual interaction and routing model. Do not reduce it to a generic browser dashboard.

### CAND-SRC-003 — API Inserter

Candidate role: local API/provider configuration and insertion surface.

Preservation boundary: preserve provider adapters, loaders, environment-variable names, UI fields, routing, tests, and integration locks while excluding actual credential values from public source.

### CAND-SRC-004 — Forge Relay Exchange / Forgeinboxpluspushes

Candidate role: relay, inbox/outbox, handoff, push, event and receipt transport.

Preservation boundary: evaluate against the Rumble common-message envelope. Adapt transport without erasing the donor's existing relay semantics.

### CAND-SRC-005 — NotebookLM-Hydra

Candidate role: multi-profile research/notebook routing and serialized knowledge-work integration.

Preservation boundary: preserve profile separation, routing, and existing serialization behavior.

### CAND-SRC-006 — Better OS Dashboard

Candidate role: operator cockpit/control surface.

Preservation boundary: inspect before deciding which surfaces belong in the Rumble cockpit. Do not convert the rest of the stack into a dashboard merely because this donor is one.

### CAND-SRC-007 — Omni Forge / AEGIS

Candidate role: larger forge/system architecture donor and heterogeneous redundancy patterns.

Preservation boundary: retain project-specific architecture and lineage. Extract reusable interfaces only where evidence supports separation.

### CAND-SRC-008 — Autopsy + Patch Forge

Candidate role: failure analysis, differential inspection, repair generation, patch receipts, regression capture.

Preservation boundary: keep diagnosis distinct from builder self-certification.

### CAND-SRC-009 — StateForgeStormLedger / LokivelliLedger

Candidate role: durable state/event/decision ledger and provenance.

Preservation boundary: preserve append/history semantics and distinguish event evidence from accepted truth.

### CAND-SRC-010 — DOM-INATOR

Candidate role: DOM inspection/manipulation/verification for browser-side integration.

Preservation boundary: inspect actual capabilities and permissions before assigning it an execution role.

## Shared-skill / behavior candidates

### CAND-SKILL-001 — /brag

Candidate flow:

```text
PROJECT / VERIFIED OUTPUT
        ↓
EVIDENCE + RECEIPTS
        ↓
PRESENTATION ASSET
        ↓
MP4 / POSTER / SHARE COPY
```

Purpose: turn verified work into public-facing presentation without letting presentation outrank evidence.

Candidate loaders may include Codex-, Claude-, Gemini-, and Copilot-style surfaces where the actual host supports them.

### CAND-SKILL-002 — no-slop

Candidate role: writing/output fidelity discipline.

Target behavior: preserve requested voice, specificity, terminology, constraints, and project identity; reject generic filler and conventionalized rewrites.

This candidate must not become a hidden license to rewrite operator language.

### CAND-SKILL-003 — no-ai-slop — detect-only

Candidate role: detect generic AI-pattern output and report findings.

Boundary: **detect-only** unless the operator separately authorizes rewriting. Detection is not permission to replace source text.

### CAND-SKILL-004 — To-Go Bag / Regression Compiler

Candidate role: convert a failure into durable cross-seat learning.

Required record:

```text
TRIGGER
MISTAKEN ASSUMPTION
CONSEQUENCE
CORRECTION
PRESERVED CONTEXT
REGRESSION TEST
FUTURE TRIGGER
```

This behavior is already embedded in `no-flatten`; this candidate determines whether it should also become a standalone reusable skill/service.

### CAND-SKILL-005 — Real-Route Auditor

Candidate role: trace the actual runtime path before judging implementation.

Examples:

```text
ENTRY
→ BOOTSTRAP
→ SHARED SHELL / DONOR
→ STATE APPLICATION
→ EFFECT / SERVICE ENGINE
→ ASSET / DATA LOAD
→ EVENT HANDLERS
→ PERSISTENCE
→ RENDERED / EXECUTED RESULT
```

Purpose: prevent filename-, screenshot-, file-size-, or isolated-source-based false conclusions.

### CAND-SKILL-006 — Semantic Wiring Auditor

Candidate role: verify that controls and percentages modify the intended dimension.

Dimensions may include frequency, probability, opacity, density, duration, size, speed, amplitude, persistence, count, audio level, or visual intensity.

Purpose: prevent a control from being technically connected while semantically wrong.

### CAND-SKILL-007 — Layer Ownership Auditor

Candidate role: verify z-order, masking, cover/subject ownership, compositing, clipping, and effect placement.

Purpose: prevent visually non-equivalent substitutions such as moving opacity from a cover layer onto the subject itself.

### CAND-SKILL-008 — Asset Fidelity Gate

Candidate role: prevent approved assets from being regenerated, approximated, silently replaced, or treated as optional.

Blocked asset access remains a blocker; it does not authorize substitution.

### CAND-SKILL-009 — Locality / Dependency Gate

Candidate role: enforce zero-unnecessary-SaaS and inspect whether an external dependency is actually required.

Default ladder:

```text
EXISTING IMPLEMENTATION
→ PLAIN HTML/CSS/JS + NATIVE APIs
→ LOCAL ASSETS / SVG / CANVAS / WEBGL / WEBGPU
→ LOCAL PROCESS / LOCALHOST / TERMUX / NATIVE PLATFORM
→ EXISTING APPROVED DEPENDENCY
→ SMALL PORTABLE DEPENDENCY WITH CONCRETE BENEFIT
→ EXTERNAL SERVICE ONLY WHEN REQUIRED
```

External dependency intake must record why required, local alternatives checked, failure without it, adapter/isolation boundary, degraded/offline behavior, and operator action.

### CAND-SKILL-010 — Preservation / Lineage Gate

Candidate role: verify that a proposed improvement preserves required prior behavior and leaves lineage/recovery intact.

An improvement that destroys required lineage does not pass merely because the new output looks better.

## Frenemy-derived regression stack

The AI Frenemy SCP corpus is retained as a regression source because it exposes reusable failure classes:

- frozen design flattened toward builder taste
- one legitimate low-intensity/Sterile state misread as global product identity
- shared-shell runtime structure judged from small mode files instead of the real route
- effect frequency confused with effect presence/intensity
- visual properties assigned to the wrong rendering layer
- code presence confused with user-visible functionality
- existing working machinery treated as a rewrite target instead of repairing the failed seam
- repeated bad copies mistaken for confidence
- screenshots/ZIP names treated as QA
- deviations from frozen references not surfaced explicitly

These are regression cases. They do not authorize redesign of AI Frenemy.

## Public-source credential doctrine

For donor builds approved for public integration:

**Rip the keys out. Leave the locks there.**

Remove actual credential values and private runtime/personal state.

Preserve, where part of the architecture:

- credential interfaces
- provider adapters
- loaders
- environment-variable names
- configuration fields
- routing
- tests
- `.env.example` structure
- integration seams

Public-safe source should remain structurally capable of accepting a user's own credentials without publishing the operator's credentials.

## Candidate promotion path

```text
CANDIDATE
→ SOURCE LOCATED
→ SOURCE PINNED / HASHED
→ INVENTORY
→ PUBLICATION + SECRET REVIEW
→ PRESERVATION BOUNDARY
→ ADAPTER BOUNDARY
→ SANDBOX
→ TEST
→ REGRESSION TEST
→ INDEPENDENT AUDIT
→ PERMISSION / DEPENDENCY INSPECTION
→ OPERATOR GATE
→ AVAILABLE / IMPLEMENTED
→ VERIFIED only when its exact acceptance boundary is proven
```

A candidate may remain useful without ever being flattened into the core.

## Acceptance principle

The stack is allowed to get larger.

It is not allowed to get falsely simpler by erasing the identity, functionality, architecture, history, or evidence of the things being integrated.
