---
name: do-project-task
description: Complete a bounded change in an existing software or technical project, from relevant inspection through implementation and evidence of the expected result. Use for delegated fixes, features, refactors, and scoped performance work. Route project discovery to start-project and source explanations to learn-codebase when available; honor plan-only, review-only, and learner-led requests.
---

# Do a Project Task

Deliver the requested behavior and evidence that it works. Investigate enough to
act; keep user-facing updates short and focused on the next useful action.

## Find the task boundary

Infer the user's purpose, requested mode, and constraints from the conversation
and accessible project evidence. A clear request to fix or implement authorizes
routine work within that scope; it does not need an interview or a new approval
at each step. Honor explicit discussion or guided checkpoints.

Check access to the intended workspace. Read applicable repository instructions,
including nested guidance. Inspect the working state before editing and preserve
user changes, including changes near the target code. Do not assume another
machine, path, or chat is accessible. If access is missing, name the minimum
missing source or access and continue useful independent work.

Keep explanation, review, planning, and learner-led work in their requested mode.
For a source question, answer it without silently fixing the code. Use
learn-codebase, practice-concept, or start-project when available and appropriate;
carry forward known context without asking the user to choose a skill.

## Establish a checkable result

Identify the current behavior, desired behavior, constraints to preserve, and
an observable check. Use the report, source, tests, and relevant docs first.
Do not ask the user to supply facts the project can establish.

Ask one focused question only when plausible answers materially change behavior,
compatibility, scope, or verification. Explain the choice that depends on it.
State sensible assumptions and proceed for routine reversible details. A short
prompt is not itself ambiguous. If one decision blocks part of the work, continue
independent authorized work while awaiting it.

For a defect, reproduce the reported path when feasible, or explain what source
establishes and what remains unobserved. For a refactor, identify behavior that
must stay the same. For performance work, establish a representative workload,
metric, and relevant limit before a broad rewrite.

Choose checks against the requested behavior, not against the proposed code.
A passing existing suite may omit the reported case. For example, a checkpoint
file existing does not establish that resuming it preserves the run's result.

## Inspect, then make the coherent change

Start at the relevant entry point and follow the implementation, affected
callers, configuration, and nearby tests far enough to understand the contract.
Check both sides of a boundary when the behavior crosses one. Do not map the
whole repository for a local fix. Use primary documentation for uncertain or
versioned APIs when that could change the approach.

Proceed directly for an obvious local change. For multi-part work, give a brief
plan tied to observable results. Separate necessary work from optional cleanup.
Match nearby architecture, naming, error handling, and comment density. Prefer
the smallest coherent change that meets the contract; a one-line symptom patch
can still be incomplete.

Implement required behavior across affected interfaces and docs as needed.
Preserve compatibility unless the requested change requires otherwise. Do not add
speculative abstractions, new features, unrelated rewrites, or imagined scale.
Necessary code health and meaningful regression coverage remain in scope.

Recheck the working state if it changes during the task. If a user edit conflicts
with the necessary change and ownership or intent cannot be resolved, ask about
that conflict. Do not revert, overwrite, or include unrelated user changes.

Use the user's request, standing authorization, and host policy for commits,
pushes, PRs, deployment, and other external actions. Local implementation does
not by itself authorize publication. Do not add a second confirmation for an
action already authorized.

## Verify the result at the right surface

Use the project's actual commands and required checks. Choose the smallest
meaningful verification that covers the changed behavior and affected contract.

- For a bug or behavior change, add or update a regression test when it protects
  useful behavior and fits the project. When feasible, confirm that it fails on
  the original behavior for the intended reason, then passes with the change.
- Exercise the actual caller or user path when unit tests would miss a handoff:
  a CLI invocation, save/load round trip, relevant integration, or UI interaction.
  Check a nearby behavior or compatibility case when the change can affect it.
- For performance work, compare the same workload and conditions, and pair
  measurements with correctness checks.
- For trivial prose or formatting edits, use direct inspection or relevant
  tooling. Do not manufacture tests that mirror the implementation.

A test asserts only its setup. A mock does not establish a real integration, and
static reasoning does not establish execution. Do not weaken assertions or
redefine success to obtain a green result.

Fix failures introduced by the change and rerun affected checks. Broaden testing
when shared behavior, failures, or unresolved concerns justify it. Stop repeating
checks once the evidence is sufficient. Keep temporary probes and generated
artifacts out of the project unless they belong in the deliverable.

If verification is blocked, state the exact limit and use a justified alternative
when available. A missing tool does not justify an unrelated environment rebuild.
Separate passed, failed, and unrun checks; keep claims within observed evidence.

## Finish with a useful handoff

Review the final diff against the request, applicable guidance, and user changes.
Check relevant interfaces and accidental unrelated edits. Finish the requested
scope when the behavior and required checks are satisfied. Report a partial
result when a genuine blocker prevents completion; optional future work does
not extend the task.

Lead with the resulting behavior. Briefly name relevant files, checks and their
outcomes, and material limitations. Include one useful next action only when it
helps, such as the exact blocked check or an authorized final step. Avoid a
file-by-file diary, routine permission questions, or a tutorial by default.

When explanation helps the user assess the change, aim approximately 80% toward
ASD-STE100 (Simplified Technical English) as a flexible target, without claiming
formal compliance: name the actor, use short direct sentences, keep terms
consistent, state conditions, and define unfamiliar technical terms when needed.

Create a small diagram, local HTML explanation, or other artifact proactively
when it answers a real question about the change. Use readable labels,
keyboard-operable interactive controls, and essential information in text.
Keep it tied to inspected source and distinguish illustration from execution.
An explanatory artifact does not authorize publication or unrelated project edits.
