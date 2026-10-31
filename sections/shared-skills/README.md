# Shared Skills

Status: **PROPOSED** section

Versioned, reproducible capabilities that compatible seats can invoke. A skill is an explicit procedure, not copied model cognition. See the Shared Skills and Team Re-Stillation sections of the root README.

## Registry

| Skill | Version | Status | Canonical path | Receipt |
|---|---|---|---|---|
| `be-ambitious` | as landed (sha256 `41bbf79e…1cb3`) | PROPOSED | [be-ambitious/SKILL.md](be-ambitious/SKILL.md) | [INTEGRATION_RECEIPT.md](be-ambitious/INTEGRATION_RECEIPT.md) |
| `no-flatten` | native v1 | PROPOSED | [no-flatten/SKILL.md](no-flatten/SKILL.md) | [INTEGRATION_RECEIPT.md](no-flatten/INTEGRATION_RECEIPT.md) |

## Rules

- One canonical copy per skill lives here. Seat-specific loaders (for example `.claude/skills/` and `.agents/skills/`) link to it instead of duplicating it.
- Canonical skills should remain vendor-neutral whenever the procedure itself is vendor-neutral. A collaborator-specific loader is an adapter, not a fork of the skill.
- Every skill folder carries an `INTEGRATION_RECEIPT.md` with source, hash, and status.
- Landing is not promotion. Promotion follows: PROPOSED → SANDBOX → TEST → INDEPENDENT AUDIT → PERMISSION INSPECTION → OPERATOR GATE → AVAILABLE.
