# Federated Infinite Brain Architecture

Version: 1.2.0 (public-safe edition)
Established: 2026-07-16
Updated: 2026-10-01 — added Generator nested second-brain and differential swarm federation
Owner and final authority: Lokivelli (operator)

> **Public-safe edition.** Derived from the private `infinite-brain` repository's architecture record. Operator-specific account details, private working-lane contents, named in-progress research items, and private migration notes have been removed. The architecture, authority rules, read/write order, failure containment, and honest limit are preserved. The source repository remains private. See [PUBLIC_SAFE_RECEIPT.md](PUBLIC_SAFE_RECEIPT.md).

Status in AI Rumble: **PROPOSED** integration. This document describes the source system's design; it does not claim that any Infinite Brain component is implemented inside AI Rumble.

## Purpose

The system is not a single-model memory store. It is a federated memory system with independent model-native brains and one shared reconciliation layer.

The design preserves disagreement instead of forcing artificial consensus.

## Layer Map

```text
Operator / Human Authority
          |
          v
brains/universal/          Shared, reconciled, provenance-backed state (cross-model)
     ^              ^              ^
     |              |              |
family shared   brains/<model>/  brains/<model>/
tier (per model  native brain     native brain
 family)
     ^
     |
per-instance native lanes
(private working memory, one per account or seat instance of the same model family)
```

### Same-family native lanes

An operator may run more than one instance of the same model family (for example, separate accounts or seats assigned different roles such as independent auditor or collaborator). Each instance gets its own native lane, reconciled through a family-level shared tier before anything is proposed up to the cross-model Universal Brain.

- **Per-instance lanes**: each instance owns only its own lane.
- **Family shared tier**: reconciled state across instances of the same model family only. Sits below `brains/universal/` in the stack. Records consensus and divergence between those instances specifically.
- Rule: agreement between instances of the same model family is correlated evidence, not independent replication (shared base model and training). Weight it below cross-model convergence recorded in `brains/universal/`.

### Model-native lanes

- Path pattern: `brains/<model>/`
- Each participating model defines and maintains its own model-native structure without overwriting any other model's lane.
- A lane may be optimized for that model's strengths (for example: architecture, implementation, governance, adversarial integration, confidence grading, and explicit separation of verified facts from inference).

### Universal Infinite Brain

- Path: `brains/universal/`
- Stores only shared state that has been reconciled.
- Records provenance, dissent, pending proposals, and promotion decisions.
- Never erases a model-specific disagreement merely because a majority prefers another answer.

## Authority Rules

1. The operator is the final authority for promotion into the Universal Brain and into any family shared tier.
2. Each model, and each instance within a model family, may write only to its own native lane unless explicitly asked to perform a merge.
3. A model or instance may propose a shared or universal change, but a proposal is not a promotion.
4. Status stamps require the underlying check or evidence. Agreement alone, across models or across instances, is not evidence.
5. Prior conclusions are superseded with an audit note; they are never silently rewritten out of history.
6. When models or instances disagree, the shared layer records the disagreement, evidence, and confidence levels.
7. `brains/universal/` is authoritative for shared cross-model context. A family shared tier is authoritative for shared context within that family. Native lanes remain authoritative for each model's or instance's own reasoning posture, unresolved concerns, and specialized workflow.

## Read Order

At the start of relevant work, each model should read:

1. `brains/universal/state.md`
2. Its family shared tier `state.md`, where one exists
3. Its own native `state.md`
4. Recent universal, shared, and native changelog entries when history matters
5. Project files directly relevant to the task

## Write Order

At the end of substantive work:

1. Update the model's (or instance's) native state and native changelog.
2. Write a proposed shared diff (family tier or universal) when shared context may need to change.
3. Do not mutate Universal Brain or family-tier status stamps without applying the relevant merge protocol.
4. Record the source model/instance, evidence, confidence, and reason.

## Shared Infrastructure

- A cross-platform continuity protocol carries a portable context snapshot between platforms.
- A convergence ledger compares model outputs and exposes agreement, divergence, unique contributions, and verification flags.
- Convergence analysis informs universal proposals; it does not automatically establish truth.

## Failure Containment

- A bad update in one native brain does not automatically contaminate the other brains.
- Universal and shared promotions are traceable and reversible through Git history and changelogs.
- Model or instance absence is tolerated: the system can operate with fewer active native lanes, but missing review is recorded.
- Stale state must be labeled stale rather than treated as current.

## Honest Limit

This is deliberate, versioned synchronization, not continuous background memory and not semantic-vector recall. The system works because each model explicitly pulls, evaluates, and writes structured state.

## Nested Generator Second-Brain Federation

Generator Forge has an accepted architectural direction for a nested federation beneath its isolated three-seat board.

The primary Generator roles remain Architect, Builder, and Independent Auditor. Each seat may gain a persistent role-native Infinite Second Brain. Persistent differential specialist subagents may gain bounded Micro Infinite Brains below their parent seat. The three seat-second-brains may propose reconciled cross-seat learning into a Generator Shared Second Brain.

This nested structure does not create additional board seats, Council votes, or authority. Provider/model identity remains separate from seat identity, so seat memory and learned failure history can survive provider replacement.

Implementation status remains **PROPOSED** until Generator runtime storage, access controls, swarm registry, reconciliation flow, receipts, and seat-isolation tests exist.

The repository-level Universal Brain remains the cross-model reconciliation layer. Generator's Shared Second Brain is project-local cross-seat learned state and must not be confused with `brains/universal/`.
