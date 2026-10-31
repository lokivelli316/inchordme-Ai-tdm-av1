# Integration Receipt — `be-ambitious`

Status: **PROPOSED** (landed, not promoted)

Per the Shared Skills promotion path in the root README, landing a skill is not promotion. This skill is available to read and invoke, but it has not passed sandbox, test, independent audit, permission inspection, or the operator gate.

## Record

```text
skill_name:            be-ambitious
skill_type:            instruction skill (procedure text, no executable code)
source:                operator-supplied plugin skill (Rob / Lokivelli), loaded in a Claude session
source_path_at_intake: /mnt/skills/plugins/be-ambitious/SKILL.md
intake_date:           2026-10-31
landed_by:             E seat (Claude), on operator request
operator_request:      "add /be-ambitious to the repo"
files_imported:        SKILL.md (verbatim, unmodified)
files_excluded:        none
sha256:                41bbf79ea489640c68ed293528cdaed1e354dbca1e4bee86b4d3976de71a1cb3
size_bytes:            12861
modifications:         none
side_effects:          none (instructional text only)
permissions_needed:    none beyond whatever task it is applied to
secrets_scan:          manual read: no credentials, keys, or personal data present
tests_run:             sha256 match between source and landed copy
test_results:          match
auditor:               none yet
rollback_point:        parent commit of the commit that added this file
```

## Layout

```text
sections/shared-skills/be-ambitious/SKILL.md   canonical copy (provider-neutral)
.claude/skills/be-ambitious                    symlink to the canonical folder;
                                               Claude loader path
.agents/skills/be-ambitious                    symlink to the same canonical folder;
                                               Codex / Agent Skills loader path
```

One physical copy, multiple views. Claude and Codex both resolve to the same canonical skill text. Other seats should read the canonical path or add a loader link to it rather than duplicate or fork it.

## Portability review

The canonical skill is vendor-neutral instruction text. It does not depend on Claude-specific hidden behavior, APIs, tools, model internals, or executable code. OpenAI Codex supports repository-local Agent Skills built around a `SKILL.md` manifest, so the canonical skill can be used by Codex without rewriting its behavioral contract. The `.agents/skills/be-ambitious` link exists only for discovery/loading; it does not create a Codex-specific copy.

Future AI collaborators should prefer the canonical path. If their harness requires a vendor-specific discovery directory, add the smallest loader/adapter pointing to the canonical skill rather than modifying the canonical skill solely for that vendor.

## What the skill does

Pushes a builder past "it works" to "it is materially harder to outperform": baseline the existing code first, stay in the same lane, run an ambition pass, fail forward with truthful states, test the real route, preserve provenance, and finish with a BEFORE / BUILT / OUTDID BASELINE / FAILURE HARDENING / TESTED / REMAINS receipt.

## Fit with AI Rumble rules

- Its "make status mean something" and "do not fake evidence" sections line up with the Model-Safe Truth Contract.
- Its "preserve what is good" and additive-improvement guidance lines up with the Source-Build Integration Rule.
- Its final receipt is a Builder's self-report. Under AI Rumble governance that receipt is an input to independent audit, not a substitute for it. Builder cannot certify Builder.

## Remaining before promotion

1. Independent audit of the skill text by a seat other than the one that landed it.
2. At least one real build run under the skill, with its final receipt checked against evidence.
3. Operator promotion decision recorded in the ledger.
