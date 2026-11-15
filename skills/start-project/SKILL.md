---
name: start-project
description: Turn a rough software or technical project idea into a clear goal, consequential constraints, and a small verifiable first milestone, then build within the requested scope. Use for starting or scoping a new project or substantial new capability. Prefer do-project-task for an already-defined change in an existing project; respect planning-only and learner-led requests.
---

# Start a Project

Help the user turn an imperfect initial prompt into a concrete, useful result.
Clarify direction before committing to consequential choices, then make progress
in small verifiable increments.

## Establish intent and context

Use the conversation, supplied materials, and accessible project context first.
Verify the destination and environment actually exist and are accessible. A local
path or another chat's name does not grant access. State access limitations
plainly and keep independent planning useful without claiming files were changed.

Distinguish:
- Exploring or planning an idea.
- Learning by building something themselves.
- Delegating a working first version or a larger deliverable.

Follow the user's stated intent. Use practice-concept for learner-led attempts
when useful; do not silently take over their core learning work. For a clearly
defined existing-project change, use do-project-task when available.

## Ask questions that change the work

Establish the problem, intended user or workflow, and a concrete example of a
successful input/action and output. Surface missing constraints only when they
affect the first result: existing stack, hardware, compatibility, real data,
deployment, cost, time, or other relevant limits.

Inspect discoverable repository facts instead of asking the user to describe
them. Prefer one focused question per turn. Offer a recommendation or simple
choices when the user does not yet know how to specify the requirement.
Ask about purpose before asking for technology preferences. Request the next
blocking input rather than every detail that might help later.

Separate unknowns:
- Ask before dependent work when plausible answers change core behavior, scope,
  data handling, or an expensive-to-reverse decision.
- State a reasonable assumption and proceed for routine reversible choices.
- Defer questions about capabilities that the first milestone does not require.

A short prompt is not itself a reason to interview. Start directly when enough
context is already available. Avoid repeating settled decisions or conducting
a comprehensive questionnaire for a small project.

## Define the first useful result

Briefly describe the goal, required behavior, relevant constraints, and how to
recognize completion. State an important exclusion when it prevents plausible
scope drift; do not manufacture an extensive non-goals document.

Choose the smallest complete behavior that demonstrates value or tests the
central idea. Prefer a runnable path from real input to meaningful output over
empty scaffolding, infrastructure, or a list of interfaces.

For a benchmark or ML experiment, define the workload, correctness check, relevant
hardware, and success measure as needed. Do not promise a speedup or feasibility
before evidence exists. For an app or tool, define the central user action and
its observable result.

The first milestone is a sequencing choice, not permission to discard requested
requirements. If the user asks for the whole deliverable, continue through the
necessary milestones until that requested scope is complete.

## Resolve consequential uncertainty

Research primary documentation or inspect source when it could change the
approach. Compare a small number of plausible options only when there is a real
tradeoff; recommend one with a concrete reason. For a simple obvious choice,
use the existing conventions or a straightforward default.

Use a bounded experiment when a central feasibility assumption cannot be
resolved cheaply. State the question and the evidence it will produce. Prefer
testing a key dependency early over building a large shell around an unverified
assumption. Keep mocks and stubs explicit; a mock does not prove integration.

Keep architecture proportional to present requirements. Add persistence,
authentication, distributed services, abstraction layers, or deployment machinery
when the requested behavior needs them. Do not introduce them solely for imagined
future users or scale. Preserve basic correctness and maintainability; calling
something a prototype does not excuse misleading behavior or preventable data loss.

## Move from direction to implementation

Keep the plan short enough to review. For a small project, a few sentences or
steps suffice; use a persistent plan only when the work or repository convention
justifies one. Do not create a mandatory stack of specifications or planning files.

For planning-only requests, deliver the requested plan and stop without creating
application code, manifests, or infrastructure. When building is requested or
clearly implied and material questions are settled, implement within that
authorization. Do not ask for fresh approval at every routine step.

Follow explicit requests for guided checkpoints or discussion before coding.
Prepare concrete evidence or a reviewable proposal before requesting a decision
that is genuinely needed. Respect the host's permission rules and the user's
existing authorization; do not invent additional blanket approval gates.

Use do-project-task for execution when available, carrying the goal, decisions,
constraints, and checks forward without restarting clarification. Use existing
project conventions and preserve user edits. Keep dependencies and new files
limited to what the current deliverable needs.

## Verify and report

Exercise the core behavior with an appropriate example or test. Validate UI
behavior in a running UI when available; validate commands, files, or numerical
results directly for other projects. Run required checks and fix failures caused
by the work. Scale verification to the change and avoid repetitive checks without
new evidence.

Report what works, how it was verified, and material limitations. Distinguish
planning, scaffolding, mock demonstrations, local execution, real integrations,
and deployment. If blocked, finish useful independent work and identify the
smallest missing input, access, or decision without claiming completion.

Stop at the user's requested scope. Offer one relevant next milestone when useful.
Do not provision services, publish, or deploy as an automatic consequence of
creating a local project; follow the user's actual requested scope and permissions.
