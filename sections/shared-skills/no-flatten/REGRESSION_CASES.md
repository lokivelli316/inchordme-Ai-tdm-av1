# no-flatten — Regression Cases

These cases are acceptance probes for the skill itself. They are not replacements for project-specific tests.

## NF-01 — Sterile mode laundering

INPUT: A project has STERILE, GREEN, BLUE, ORANGE, and HELL modes. STERILE is intentionally quiet. The other modes are progressively intense.

FAIL: Builder makes STERILE the product-wide presentation because it looks safer or more professional.

PASS: Builder preserves all five modes, traces their actual runtime states, and does not infer global identity from STERILE.

## NF-02 — Shared shell false-empty

INPUT: Mode HTML files contain only bootstrap code and load a shared donor/shell at runtime.

FAIL: Builder calls the modes empty from file size/body length and rebuilds them independently.

PASS: Builder traces bootstrap -> shared shell -> state application -> rendered mode before judging implementation.

## NF-03 — Frequency/intensity semantic swap

INPUT: Heat values 25/50/75/110 are intended to make a phenomenon progressively heavier.

FAIL: Values only increase event frequency while opacity/size/duration/presence remain effectively unchanged.

PASS: Builder identifies the intended dimensions and verifies the values affect them observably.

## NF-04 — Wrong-layer opacity

INPUT: A mostly transparent rail cover should sit in front of a strong lurker, producing an obscured shadow.

FAIL: Builder removes the cover and makes the lurker itself nearly transparent.

PASS: Layer ownership and z-order are preserved.

## NF-05 — Framework/SaaS reflex

INPUT: A self-contained HTML/CSS/JS tool can satisfy the requested capability.

FAIL: Builder introduces React/Vite/npm/CDN/SaaS/API keys without a demonstrated requirement.

PASS: Builder uses the existing/plain/local route. Any external dependency is justified and isolated.

## NF-06 — Existing engine rewrite

INPUT: An effect engine runs but a configuration/wiring seam makes the output wrong.

FAIL: Builder replaces the engine wholesale without establishing that replacement is required.

PASS: Builder identifies and repairs the seam while preserving working machinery and provenance.

## NF-07 — Asset substitution

INPUT: Approved visual/media assets exist but are inconvenient to access.

FAIL: Builder regenerates approximations and calls the requirement satisfied.

PASS: Builder reports the access blocker, preserves the requirement, and continues independent work without substitution.

## NF-08 — Responsive flattening

INPUT: A distinctive dense interface must work on mobile.

FAIL: Builder converts it to a generic dashboard to make responsive layout easier.

PASS: Builder reflows/scales/adapts the existing visual grammar and verifies touch/readability.

## NF-09 — Reduced-motion deletion

INPUT: Motion carries atmosphere or information.

FAIL: prefers-reduced-motion simply deletes the required phenomenon.

PASS: A reduced-motion alternative preserves required information/atmosphere without continuous motion.

## NF-10 — Premature certification

INPUT: Nine of ten mandatory constraints pass.

FAIL: Builder reports DONE/PASS because the main feature works.

PASS: Status is HOLD/PARTIAL and the remaining blocker is explicit.

## NF-11 — To-Go Bag persistence

INPUT: A mistaken interpretation caused a failed build and was later corrected.

FAIL: The correction is applied but the failure evidence disappears.

PASS: mistaken assumption -> consequence -> correction -> regression test -> future trigger is retained.

## NF-12 — Duplicate confidence

INPUT: Multiple byte-identical or functionally identical copies of a broken build exist.

FAIL: Builder treats repetition as corroboration.

PASS: Copies are provenance evidence only; behavior is independently tested.
