# AI Rumble — Source Integration Proposal Plan

Status: PROPOSED / PRE-INTEGRATION  
Target: `lokivelli316/inchordme-Ai-tdm-av1`

## Objective

Integrate planned source builds as identifiable additive side sections without flattening their architecture, deleting functionality, rewriting lineage, confusing proposal with implementation, or accidentally publishing private source.

## Intake sequence

```text
DISCOVER SOURCE
      ↓
RECORD VISIBILITY + AUTHORITY
      ↓
PIN SOURCE COMMIT / ARTIFACT HASH
      ↓
INVENTORY
      ↓
PUBLICATION / SECRET REVIEW
      ↓
DEFINE PRESERVATION BOUNDARY
      ↓
DEFINE ADAPTER BOUNDARY
      ↓
DEFINE DEPENDENCIES
      ↓
DEFINE ACCEPTANCE TESTS
      ↓
CLONE / COPY / VENDOR / ADAPT
      ↓
WIRE
      ↓
TEST
      ↓
INDEPENDENT AUDIT
      ↓
PROMOTE STATUS
```

## Source registry — initial discovery

### SRC-001 — TheBeast / Generator Forge

- Source: `lokivelli316/TheBeast`
- Current source visibility: **PRIVATE**
- Intended Rumble role: Generator Forge side section; generation; Builder/Auditor lineage; Termux/runtime integration.
- Source planning authority found: `planning/GENERATOR_FORGE_INITIAL_LANDING.md`
- Source candidate named there: `Nemotron_Generator_Forge_v0.4.3.6_COLD_AUDIT_CLAUDE.zip`
- Existing source landing doctrine requires source receipt, inventory, non-destructive import, qualification, acceptance, rollback, provenance, and preservation of working paths/module seams.
- Existing durable material also states Nemotron Generator Forge remains private.
- **Current Rumble action:** proposal/integration metadata only.
- **Public source copy:** BLOCKED pending explicit operator publication decision plus secret/runtime-state review.
- Preservation boundary: do not redesign into a generic dashboard; do not flatten modules; preserve frozen assets and working path/module seams where source authority requires them.
- Adapter target: `sections/generator-forge/`
- Planned bridges: Termux, local relay, artifact bus, skill bus, audit/receipt bus.

### SRC-002 — Infinite Brain

- Source: `lokivelli316/infinite-brain`
- Current source visibility: **PRIVATE**
- Source description: chat-native, git-versioned persistence/federation layer.
- Architecture found: `FEDERATED_BRAIN_ARCHITECTURE.md`
- Existing architecture preserves independent model-native lanes plus shared reconciliation, dissent, provenance, promotion decisions, and human authority.
- Existing honest limit: deliberate versioned synchronization rather than automatic/background semantic memory.
- **Current Rumble action:** proposal/integration metadata only.
- **Public source copy:** BLOCKED pending explicit operator publication decision plus private-state/publication review.
- Preservation boundary: do not flatten model-native disagreement into artificial consensus; preserve native lanes, provenance, promotion gates, and honest runtime limits.
- Adapter target: `sections/infinite-brain/`
- Planned bridges: context builder, model seat lanes, shared knowledge proposals, Git relay, receipts, ACATMO artifact references.

### SRC-003 — ACATMO

- Source: NOT YET LOCATED through current GitHub search.
- Intended Rumble role: integrity, provenance, vault/artifact handling, ZIP-as-folder behavior, cache behavior, content identity.
- Current status: **SOURCE REQUIRED / PROPOSED INTEGRATION**
- Adapter target: `sections/acatmo/`
- Rule: inspect the real source before proposing implementation changes.

### SRC-004 — Local Vault / Organizer / Deduplicator

- Source: NOT YET PINNED.
- Intended Rumble role: local storage, indexing, relationships, content-addressable identity, duplicate control, logical project views.
- Current status: **PROPOSED**
- Adapter targets:
  - `sections/local-vault/`
  - `sections/organizer/`
  - `sections/deduplicator/`

### SRC-005 — Interconnect / Relay Fabric

- Source: architecture currently established in AI Rumble planning; implementation source NOT YET PINNED.
- Intended role: common message semantics across heterogeneous transports.
- Current status: **PROPOSED**
- Adapter target: `sections/interconnect/`
- Transport targets: Unix socket, SQLite, filesystem, Android IPC, localhost, browser extension, Git/GitHub, SSH/LAN, operator-mediated bridge.

## Public/private rule

AI Rumble itself is public.

A private donor/source repository does **not** become public merely because AI Rumble plans to integrate it.

Before private source enters this public repository:

1. operator explicitly authorizes publication of that source/build;
2. source is pinned by commit/hash;
3. secrets and credentials are reviewed;
4. private runtime state and personal data are reviewed;
5. publication/licensing constraints are checked;
6. preservation boundary is recorded;
7. imported files receive provenance.

Until then, public-safe adapters, schemas, interfaces, documentation, and independently reimplemented compatible components may be developed without copying private source.

## Integration receipt

Every landed source section should eventually carry an `INTEGRATION_RECEIPT.md` containing:

```text
source_repository
source_visibility_at_intake
source_commit_or_artifact_hash
intake_date
source_authority
files_imported
files_excluded
exclusion_reasons
preservation_boundary
adapter_boundary
dependencies
secrets_scan
tests_run
test_results
auditor
status
rollback_point
```

## Acceptance rule

No source section becomes `VERIFIED` merely because it was copied successfully.

Copying proves copying.

Wiring proves only what its integration tests demonstrate.

Promotion requires the stated acceptance evidence and independent audit gate.
