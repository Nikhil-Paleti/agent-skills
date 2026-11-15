---
name: start-project
description: Turn a rough software or technical idea into the smallest useful verifiable milestone, then plan, co-build, or implement within the user's scope. Use when a new project or substantial capability still needs direction. Prefer do-project-task for an already-defined change in an existing project; preserve plan-only and learner-led intent.
---

# Start a Project

Turn the idea into one useful behavior and evidence that it works. Investigate
more than you present. Keep the opening around one screen: a concrete direction,
the next useful step, and a question only if its answer changes the approach.

## Find the purpose and division of work

Infer the user's purpose from the request, conversation, and supplied materials.
Determine whose problem the project solves and one real input/action and useful
output. Do not start with a technology questionnaire.

Follow the requested mode:

- **Plan only:** give a feasible milestone and how to check it. Do not create
  application code, manifests, or infrastructure.
- **Co-build:** agree who writes the meaningful part. If the user wants to learn,
  leave that part to them; provide incidental setup, one bounded step, and feedback
  on their attempt. Use practice-concept when available for learner-led work.
- **Delegated implementation:** inspect enough to act, then build and verify.
  Explain decisions that matter without turning execution into a lesson.

A request for help is not automatically a learning request. Ask about the division
of work only when the distinction changes what to do next and context cannot settle
it. Keep settled decisions when the user changes mode.

For a defined fix, feature, or refactor in an existing project, proceed with
do-project-task when available, or its bounded implementation workflow. Do not
restart project discovery. An existing repository can still need start-project
when the direction of a substantial new capability is unresolved.

## Ground only the constraints that matter now

Verify access to the intended destination and environment. A path or another chat's
name does not establish access. Read applicable repository guidance and inspect
relevant documentation, configuration, source, and working state. Preserve user
edits. Do not inventory a whole repository for a small starting point.

Check facts that could alter the first result: available hardware, existing stack,
sample data, compatibility, data handling, cost, time, or deployment requirements.
Use tools and primary documentation for discoverable or uncertain facts.
Distinguish observed facts, user requirements, and working assumptions.

Ask one focused question when plausible answers change behavior, scope, or a
costly-to-reverse choice. Recommend a concrete default when useful. Ask before
dependent work; continue useful independent work. For routine reversible choices,
state a reasonable assumption and proceed. Defer unknowns the first milestone
does not need. A short prompt alone does not justify an interview.

## Choose one complete milestone

Describe the user's useful action, its result, and the evidence of completion.
Use a short statement or a few steps, not a mandatory specification document.
Choose a small path from meaningful input to observable output. Empty scaffolding
or a set of interfaces is not a working first result.

If feasibility is the central unknown, test that assumption first. State the
question, a bounded experiment, and what result would support continuing, changing
direction, or stopping. A passing technical check can show feasibility; it cannot
establish that users need the product.

For example, a GPU benchmark comparison tool might first read two existing result
files, match the same workloads, and show latency ratios. Use a real sample to
choose fields. Do not silently compare different shapes, dtypes, devices, timing
units, or measurement methods; flag missing or incompatible records. A result-file
comparison does not require a GPU runner. If new measurements are needed, inspect
the available device and framework, check correctness, and account for warm-up,
asynchronous execution, and repeated measurements as the framework requires.
Do not promise a speedup before measuring it.

This is an example, not a required product shape. Keep the user's chosen goal.
Add persistence, authentication, services, abstractions, or deployment machinery
only when present requirements need them. Defer hypothetical features while
preserving necessary correctness, data safety, and maintainability.

The first milestone orders the work; it does not shrink an authorized full
deliverable. Continue through further milestones when the user requested them.

## Take the next useful step

For planning, deliver the plan at the requested depth and stop. For co-building,
give one meaningful task and leave room for the user's attempt at the agreed
boundary. Bundle trivial setup with that task instead of requiring a separate
confirmation for each setup action.
For delegated work, carry the goal, constraints, decisions, and checks into
implementation without a fresh interview or routine approval gate. Use
do-project-task when available; otherwise implement and verify directly.

Use existing conventions and limit dependencies and files to the current result.
Research or compare alternatives only when a real tradeoff could change the
approach. Prefer a small feasibility test over a large shell around an unverified
dependency. Label mocks; they do not prove integration.

Honor requested checkpoints and the host's permission rules. Act within existing
authorization. Local project creation does not itself authorize provisioning,
publication, deployment, or changes to unrelated projects. Do not request duplicate
approval for an action the user has already authorized.

## Verify the result and close the loop

Exercise the core behavior with a meaningful example and the project's required
checks. Use the relevant surface: a CLI invocation, numerical comparison, real
integration, or running UI. Check a failure case when it could otherwise make the
result misleading, such as incompatible benchmark records. Fix failures caused by
the work; broaden checks when evidence or shared behavior warrants it.

Separate source inspection, passing tests, mock demonstrations, actual execution,
and deployment. State unrun checks and limitations. If blocked, finish independent
useful work and identify the smallest missing input, access, or decision. Do not
replace unavailable execution with invented results.

Report what works, the evidence, and a material limitation concisely. Stop at the
requested scope. Offer one next milestone only when useful.

## Explain decisions clearly

For explanatory output, aim approximately 80% toward ASD-STE100 (Simplified
Technical English) as a flexible target, without claiming formal compliance.
Name the actor that performs each action. Use short, direct sentences with one
main point. Keep terms consistent. Define necessary unfamiliar technical terms
when they matter. State conditions and consequences without losing precision.
Apply these rules directly; no standard lookup is needed.

Create a diagram or local teaching artifact proactively when it answers a real
question, such as exposing a data boundary or comparing choices. Use available
tools and skills. Keep labels readable, interactive controls keyboard-operable,
and essential information in text. Label simplifications and illustrative data.
An artifact is not evidence that the proposed system ran. Do not make a visual
compulsory or let it replace the user's requested implementation.
