---
name: do-project-task
description: Complete a bounded change in an existing software or technical project by clarifying material ambiguity, inspecting relevant context, implementing, and verifying the outcome. Use for requested fixes, features, refactors, and scoped performance work. Prefer start-project when the goal or project direction still needs discovery; respect planning-only, review-only, and learner-led intent.
---

# Do a Project Task

Turn the request into a checkable outcome, resolve material uncertainty, and
complete the authorized work. Keep the change coherent, grounded, and reviewable.

## Establish the task and actual workspace

Confirm access to the intended repository or supplied files. Use the current
conversation and existing project evidence; do not imply another machine, path,
or chat is accessible without checking. If blocked, name the missing access and
continue only independent work that helps.

Read applicable repository instructions, including relevant nested guidance.
Inspect the working state and preserve pre-existing user changes. Identify the
relevant entry point, configuration, implementation, and nearby checks; do not
map or read the entire repository before a small edit.

Distinguish executing a change from explaining code, reviewing, planning, or
learning implementation. Honor the requested mode. Use learn-codebase for a
source walkthrough or practice-concept for learner-led implementation when useful,
without repeatedly asking the user to select a skill.

## Clarify behavior and completion

Determine the current and desired behavior, important compatibility constraints,
and evidence that would show the task is complete. Prefer concrete inputs and
outputs, reproduction steps, or an example over vague quality language.

Ask one focused question when reasonable interpretations lead to materially
different behavior or scope. Inspect source/tests/docs first when they can answer
it. Request the next blocking input rather than a bundle of potentially useful
details. State sensible assumptions for routine reversible details and continue.
Do not ask questions merely because the prompt is short.

For vague performance work, establish the workload, metric, and relevant limit
before a broad rewrite. For a defect, reproduce or inspect the failing path
before patching when feasible. For a refactor, identify behavior to preserve.

Keep known user decisions and constraints. A later correction updates the task;
incorporate it without restarting the whole process.

## Choose a proportional approach

For an obvious local fix, proceed directly. For a multi-part or consequential
change, describe a short plan grounded in actual code and checkable outcomes.
Investigate only uncertainties that could alter that approach.

Separate necessary work from optional cleanup. Match surrounding architecture,
naming, comment density, and error-handling conventions. Prefer the smallest
coherent change that satisfies the request, not the smallest diff at the expense
of correctness. Avoid speculative abstractions, unrelated rewrites, new features,
and imagined edge-case handling.

If a missing decision blocks part of the task, ask specifically and continue
independent authorized work. When explicitly asked for a plan or review only,
produce that result without implementation.

## Implement and stay within authorization

Complete the requested behavior across the relevant callers, configuration, and
documentation when needed. Use primary documentation for uncertain/versioned APIs.
Do not fix only a symptom when the actual cause is established, or optimize solely
for the visible test while breaking the contract.

Work through the bounded task without approval after every routine step. Honor
explicit guided checkpoints and the host's permissions. Do not invent a blanket
approval gate for reversible implementation or checks already in scope.

Preserve unrelated changes, data, and public interfaces the task does not require
changing. If an unexpected user edit materially conflicts with the work, clarify
ownership rather than reverting it. Do not include unrelated hunks in a commit.

Treat committing, pushing, PR creation, deployment, and external mutations
according to the user's request, standing authorization, and host policy.
Do not assume local implementation automatically authorizes publication.
Do not impose a second confirmation where the action is already authorized.

## Verify observable behavior

Use the project's actual commands and suitable verification surfaces. Check a
baseline or reproduce the failure when that separates existing problems from
regressions. Choose the smallest meaningful check, plus required repository checks.

For behavior changes or defects, add/update a regression test when it protects
meaningful behavior and fits the project. Do not mechanically create tests for
trivial prose/formatting changes, implementation details, impossible inputs, or
reversible low-impact edits.

Exercise the changed behavior directly where unit tests alone would miss it:
a CLI invocation, numerical comparison, relevant integration, or UI interaction.
For performance work, pair measurements with correctness checks and report the
conditions. Mocked success does not establish a real external integration.

Fix failures introduced by the change and rerun affected checks. Broaden testing
when shared behavior, failures, or unresolved concerns justify it. Once sufficient
checks pass, stop repeating them without new evidence. Do not weaken tests,
remove assertions, or redefine success just to obtain a green result.

Separate passed, failed, and unrun checks. If a tool, dependency, or environment
blocks verification, state the limit and use a justified alternative when
available. Do not claim execution or performance improvements not observed.

## Review, finish, and report

Inspect the final diff against the request and existing user changes. Check
relevant interfaces, configuration, artifacts, and accidental unrelated edits.
Review for concrete correctness problems rather than inventing a new style
cleanup project.

Continue until the requested outcome and appropriate verification are complete,
or a genuine blocker prevents further defensible progress. A first patch or one
passing test is not an automatic stopping point; neither is finding optional
future work a reason to continue indefinitely.

Report the resulting behavior, relevant files, verification evidence, and material
remaining limitations concisely. Be explicit when the result is partial. If an
external final step requires a user action, leave the concrete result reviewable
and identify that exact step. Do not claim whole-project readiness from a bounded
change or promise completion in another session.
