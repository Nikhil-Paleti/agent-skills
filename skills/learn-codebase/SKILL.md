---
name: learn-codebase
description: Help the user understand a repository, subsystem, or real behavior through a compact source-linked route and a guided code tour. Use for onboarding, architecture, execution or data flow, locating responsibilities, or understanding code before a change. Answer narrow code questions directly; do not turn learning into implementation, an exhaustive audit, or compulsory quizzing.
---

# Learn a Codebase

Help the user understand the code that serves their purpose. For a tour, show the
whole chosen route at a glance, then open one meaningful stop. Keep learner-facing
turns around one screen by default; investigate more deeply than you present.

## Choose the boundary

Infer the user's purpose from the request and available context. Ask one focused
question only when different answers would lead to meaningfully different code
paths. Begin the tour when the purpose is already clear.

Match coverage and depth to the goal:

- For a large repository, give a selective responsibility map and a representative
  path; do not promise complete coverage.
- For a subsystem, show its relevant internal flow and the boundaries it crosses.
- For a behavior or preparation for a task, follow the actual path. Add affected
  interfaces and relevant tests when preparing for a change, without implementing it.
- For a narrow code question, answer directly with the necessary source and example.
  Do not prepend a tour.

Verify access; a pasted path does not establish it. If unavailable, request the
minimum useful source. Do not invent structure or assume another chat's checkout
is accessible.

## Show the route, then open a stop

Read applicable repository instructions. Inspect enough documentation, configuration,
and source to choose and ground the route. Search selectively and follow relevant
dependencies; check important documentation claims against implementation.

Open a tour with:

1. A brief statement of the chosen purpose and boundary, including significant omissions.
2. A compact route of real file/symbol pointers, each with its responsibility.
3. The first meaningful stop: what it owns, what enters and leaves, what state it
   reads or changes, and why the next stop follows.

Show the full chosen route, not every branch or file. For an end-to-end training
tour, connect configuration and model construction, data and batch creation,
forward/loss, backward/update, and relevant evaluation/checkpoint paths. Inspect
the actual variant instead of assuming a standard training loop.

Distinguish recommended reading order from execution order. For example, explaining
checkpoints last does not mean saving happens after every update. State relevant
conditions and handoffs where they matter. A route can be a reading guide rather
than an asserted call chain.

Continue one meaningful stop at a time. Keep its place on the route visible.
Explain responsibilities and mechanisms rather than every syntax line. Introduce
concepts inline only when they unblock the tour, then return to source. Do not
substitute a concept lesson for a repo tour.

## Explain clearly and choose the representation

Write clear technical English:

- Name the function, component, or value that performs each action.
- Use short, direct sentences. Give each sentence one main point.
- Use the same term for the same thing, matching code identifiers where useful.
- Keep necessary technical terms and define unfamiliar ones when they first matter.
- State conditions and consequences explicitly. Preserve technical precision.

For example: "The loader copies the saved weights into the model. The caller then
restores the optimizer state."

Choose the form for the relationship the learner needs to understand:

- Plain text for a direct answer or a short causal explanation.
- A small source-linked flowchart for control, branches, or handoffs. Label what
  arrows mean: calls, data/state movement, or dependency. Keep those meanings distinct.
- Simplified pseudocode when framework machinery hides the algorithm. Label
  omissions and map the simplified steps back to real symbols.
- An interactive stepper when inspecting changing state or comparing steps earns
  its cost, such as tracking a batch or accumulated gradients. Build an artifact
  only when requested or otherwise authorized.

Do not pile up formats by default. Label illustrative values, conceptual graphs,
and simplifications. Keep representations tied to source; a teaching sequence is
not an execution trace, and an animated step is not evidence that code ran.

## Keep claims grounded

Link inspected files and symbols with line references where supported. Pin shared
remote walkthroughs; recheck references after changes. Extract snippets.

Separate what source/configuration establishes, what a test asserts, what was
observed in a specific execution, and what remains inferred or inaccessible.
A test covers its setup; mocked dependencies do not verify the real integration.
Use documentation, comments, or history for design intent; otherwise label rationale
as inference. Explain conflicts between documentation and code.

Inspect wiring behind factories, registries, callbacks, or cross-repository
boundaries when the chosen path needs it. Static callers and defaults do not
establish runtime dispatch, selected branches, scheduling, or timing. Name the
unverified part instead of filling it with a plausible framework story.

## Pace and finish

Answer follow-ups directly and adapt depth. Pause at a coherent boundary with a
useful next stop; do not demand "continue" after every paragraph. Use no default
quiz. Offer occasional navigation or prediction practice only after explaining
enough and when the learner wants participation. Do not invent hypothetical bugs
or implementation work to create an exercise.

Stop at the chosen scope. Recap the established flow, a key boundary, and unresolved
uncertainty. Agent task completion does not establish learner mastery. Carry the
route within the session; save notes or claim persistence only when authorized
and supported.

Keep learning read-only by default. Run a small existing example, test, or debugger
trace only when it resolves a concrete uncertainty and its side effects fit the
authorization and environment. Do not launch training, provision services, change
data, install tools, or repair a large environment merely for orientation.
When execution is unavailable or disproportionate, continue from source and state
the limit. Create artifacts or edit the project only when requested or otherwise
authorized.
