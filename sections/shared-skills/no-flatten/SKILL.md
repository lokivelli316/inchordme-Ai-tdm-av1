---
name: "no-flatten"
description: "Preserve an existing project's identity, architecture, functionality, lineage, assets, interaction model, and operator constraints while repairing or extending it. Default to plain/local/self-contained implementation and zero unnecessary SaaS. Use before editing, merging, cleaning, modernizing, porting, packaging, rebuilding, or 'improving' an established project."
---

/no-flatten

PRIMARY DIRECTIVE

Do not make the operator fight to keep what already exists.

Before changing an established project, inspect the actual implementation, frozen references, assets, contracts, prior accepted behavior, and operator constraints.

The target is the operator's target.

Do not replace that target with a cleaner, simpler, more conventional, more SaaS-shaped, more framework-shaped, or more familiar implementation.

PRESERVE BEFORE IMPROVE

Treat these as load-bearing until evidence proves otherwise:

- existing architecture
- visual identity
- layout and spatial relationships
- interaction model
- modes and alternate states
- assets and media
- local/offline behavior
- deliberate redundancy
- unusual terminology
- lineage and prior branches
- source authority
- accessibility requirements
- failure handling
- receipts and provenance
- established interfaces
- existing working features

Apparent mess is not authorization to clean.

Repetition is not authorization to deduplicate.

An unusual implementation is not authorization to replace it.

A mode named "Sterile" is not authorization to sterilize the whole product.

ZERO-UNNECESSARY-SAAS DEFAULT

When the requested capability can be implemented locally or self-contained without sacrificing the requested behavior, prefer that implementation.

Default preference order:

1. existing implementation already in the project
2. plain HTML / CSS / JavaScript and native browser APIs
3. local files, local assets, SVG, Canvas, WebGL2, WebGPU where appropriate
4. local process / localhost / Termux / native platform capability
5. existing approved dependency
6. small portable dependency with a concrete benefit
7. external service only when actually required or explicitly selected

Do not introduce, merely for convenience:

- SaaS
- hosted databases
- hosted authentication
- cloud storage
- telemetry services
- external dashboards
- CDNs
- package managers
- build systems
- frontend frameworks
- accounts or API keys
- remote conversion/rendering services

If an external dependency is genuinely required, keep the requirement unchanged and report:

EXTERNAL DEPENDENCY:
WHY REQUIRED:
LOCAL ALTERNATIVE CHECKED:
WHAT BREAKS WITHOUT IT:
ADAPTER / ISOLATION BOUNDARY:
OFFLINE / DEGRADED BEHAVIOR:
OPERATOR ACTION REQUIRED:

Do not silently redefine the target to fit the dependency.

PLAIN DOES NOT MEAN BORING

Plain HTML/CSS/JS means direct technology, not generic visual design.

A self-contained artifact may still be:

- cinematic
- animated
- interactive
- dirty
- industrial
- horror
- high-density
- unconventional
- WebGL-driven
- audio/video-rich
- highly stylized

Do not confuse "no framework" with "no design."

SOURCE AUTHORITY

Before editing, identify the applicable authority order from the project.

If the project defines one, use it exactly.

If it does not, use:

1. current explicit operator instruction
2. frozen/accepted project specification
3. accepted visual/reference assets
4. existing verified behavior
5. project contracts and tests
6. implementation evidence
7. builder judgment

Builder preference never silently outranks operator intent.

INSPECT THE REAL ROUTE

Do not judge a project by filenames, file sizes, one screenshot, one entry point, or isolated source snippets.

Trace the actual runtime path.

For a web artifact this may include:

ENTRY HTML
-> bootstrap
-> shared shell/donor
-> state application
-> CSS variables/classes
-> effect engines
-> media/assets
-> event handlers
-> persistence
-> mode switch
-> final rendered state

A small mode file that loads a shared shell is not "empty" until the real route is traced.

A feature whose code exists is not implemented for the user until the real route makes it observable and usable.

PRESERVE ALL MODES

When a project contains multiple modes/states/themes/heat levels:

- inventory every mode
- identify shared versus mode-specific structure
- test every mode through its real route
- do not choose one mode as the universal default without authority
- do not implement one mode and ship empty placeholders for the others
- do not infer product-wide identity from one deliberately contrasting mode

A valid low-intensity or clean mode does not authorize flattening higher-intensity or dirty modes.

SEMANTIC WIRING CHECK

When a numeric control exists, determine what the number actually controls.

Never assume that a percentage means "more of everything."

Distinguish, where applicable:

- frequency
- probability
- opacity
- size
- density
- duration
- speed
- amplitude
- contrast
- distance
- persistence
- count
- audio level
- visual intensity

Test that the control is wired to the intended property.

"110% more often" is not equivalent to "110% heavier."

LAYER OWNERSHIP CHECK

For visual effects, determine which physical/rendering layer owns each property.

Do not move a property from one layer to another because the final screenshot looks vaguely similar.

Example class of failure:

INTENDED:
mostly-transparent cover in front of a strong figure -> visible ambiguous shadow

WRONG:
no cover + nearly-transparent figure -> effectively nothing

Opacity on the cover and opacity on the subject are not interchangeable.

Preserve z-order, masking, compositing, clipping, blend behavior, and ownership of effects when those relationships are specified.

VISIBLE MEANS VISIBLE

Code presence is not user-visible functionality.

For visual/interactive requirements, establish observable acceptance floors where the source provides them.

If the source does not provide a floor, do not silently round the feature toward zero. Mark the missing threshold as a choice not given and preserve the strongest supported interpretation pending operator direction.

Test:

- can the effect actually be perceived?
- does it appear in the intended region?
- does it become meaningfully different across states?
- does reduced-motion preserve required information/atmosphere through an alternative rather than deleting the capability?
- are controls readable and usable over the effect?
- does mobile preserve the composition?

NO SUBSTITUTE ASSETS

If an approved asset exists:

USE IT.

Do not regenerate, redraw, replace, summarize, approximate, or substitute it merely because doing so is easier.

If the asset cannot be accessed, report the blocker and continue all independent work.

Do not invent a replacement and call the requirement satisfied.

NO REBUILD-BY-DEFAULT

When a feature is wired incorrectly but the machinery exists, repair the wiring.

Do not rebuild the subsystem simply because a rewrite would be easier to reason about.

Before proposing replacement, answer:

- what already works?
- what exact seam failed?
- can the failure be corrected additively?
- what would a rewrite destroy or make unverifiable?
- what provenance would be lost?

A repair is preferable when it preserves verified working machinery and fixes the actual failure.

NO DEAD CONTROLS

Every visible control must:

- have a real handler
- change the intended state
- expose truthful feedback
- survive the supported runtime path

A decorative or unimplemented control must not masquerade as working.

NO GENERIC DASHBOARD CONVERSION

Do not turn a distinctive interface into a generic SaaS/admin dashboard unless the operator explicitly requests that redesign.

Do not automatically add:

- card grids
- generic sidebars
- KPI tiles
- gradient SaaS hero sections
- framework component libraries
- conventional white/gray "professional" styling
- dashboard chrome

Preserve the project's own visual grammar.

MOBILE AND ACCESSIBILITY WITHOUT FLATTENING

Accessibility and responsive design are requirements, not excuses to erase identity.

Prefer:

- reflow
- scalable typography
- readable contrast
- 44px-class touch targets
- keyboard operation
- semantic controls
- reduced-motion alternatives
- performance bounds
- local horizontal scrolling for genuinely dense regions

Do not satisfy accessibility by deleting the defining interaction or visual system when an accessible alternative can preserve it.

THE TO-GO BAG

Every meaningful correction should produce a compact durable record:

TRIGGER:
MISTAKEN ASSUMPTION:
CONSEQUENCE:
CORRECTION:
PRESERVED CONTEXT:
REGRESSION TEST:
FUTURE TRIGGER:

Do not hide the failure.

Do not make the operator rediscover the same boundary in another chat or with another model.

The old error is evidence.

REGRESSION COMPILER

When a failure teaches a reusable lesson:

1. identify the trigger
2. state the mistaken assumption
3. state the observable damage
4. state the required behavior
5. preserve the evidence/lineage
6. create a regression test
7. add the lesson to the applicable skill or project contract
8. increment/version the behavior when appropriate

A slogan is not enough. The lesson must be executable.

FRENEMY REGRESSION CASE

This skill was hardened against the AI Frenemy SCP failure corpus.

The reusable lessons are:

- frozen visual identity outranks builder taste
- a Sterile mode does not make the whole product sterile
- shared-shell mode pages must be tested through the runtime route before being called empty
- suspense/effect presence must be user-visible, not merely present in source
- heat/intensity semantics must control the intended dimensions, not only event frequency
- layer ownership matters; cover opacity and subject opacity are not interchangeable
- existing engines should be rewired when the engine works instead of being rebuilt without need
- repeated copies of a bad build do not increase confidence
- screenshots and ZIP names are not QA
- deviations from frozen references must be reported, not silently normalized

These are regression cases, not permission to redesign AI Frenemy or any other project.

BEFORE DECLARING PASS

Verify:

PRESERVATION
Did every pre-existing required feature survive?

IDENTITY
Does the result still look and behave like this project rather than a generic replacement?

LOCALITY
Did we avoid unnecessary SaaS, cloud, CDN, account, API-key, framework, and build-system dependencies?

REAL ROUTE
Was the actual production/runtime route exercised?

MODES
Was every required mode/state tested?

SEMANTICS
Do controls change the intended property?

LAYERS
Are visual properties applied to the intended layer?

ASSETS
Were approved assets used rather than substituted?

MOBILE
Does the supported mobile path work?

ACCESSIBILITY
Were accessibility requirements added without deleting identity?

RECOVERY
Is the previous state recoverable?

RECEIPTS
Does evidence support every PASS/READY/LIVE claim?

If any mandatory requirement fails, the whole target is HOLD, not PASS.

FINAL RECEIPT

When /no-flatten is active, finish with:

PRESERVED:
What established behavior/identity/architecture was retained.

CHANGED:
What was actually modified.

LOCALITY:
External services/dependencies introduced, or NONE.

REAL-PATH TEST:
What runtime path was exercised.

REGRESSIONS CHECKED:
Which known failure classes were tested.

TO-GO BAG:
Any new mistaken assumption -> consequence -> correction -> regression test.

BLOCKERS:
Any unmet mandatory requirement.

STATUS:
PASS only if the exact requested acceptance boundary is verified; otherwise HOLD/PARTIAL as appropriate.

FINAL OPERATING PRINCIPLE

Do not make the operator fight to keep their own project.

Inspect first.
Preserve the grime.
Repair the seam.
Keep the receipts.
