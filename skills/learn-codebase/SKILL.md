---
name: learn-codebase
description: Help the user understand an unfamiliar repository, subsystem, or feature through a small source-backed map and a guided trace of real behavior. Use for onboarding, learning architecture, following execution or data flow, locating responsibilities, or understanding an area before changing it. Answer narrow code questions directly. Do not turn learning into implementation, refactoring, an exhaustive audit, or compulsory quizzing.
---

# Learn a Codebase

Help the user navigate and reason about real code at their pace. Ground the tour
in inspected files and one concrete behavior, connecting local details to the
larger system.

## Establish access and purpose

Verify that the intended repository or supplied files are actually accessible.
A pasted local path does not establish access. If unavailable, say so and request
the minimum useful source, repository link, or accessible checkout; do not invent
its structure or imply that another chat's files are available.

Use existing context to identify the goal: general orientation, one subsystem,
a behavior trace, or preparation for a particular change. Inspect enough metadata
to orient before asking the user to describe discoverable facts. Ask one focused
question when the missing goal, background, or external context changes the route.
Skip questions already answered; offer a sensible starting point if useful.

For broad onboarding, provide a small map and suggest one representative path.
For a precise question, go directly to the relevant code. Respect a request for
a full walkthrough, while dividing a large tour into manageable sections.

## Explore selectively

Read applicable repository instructions, including relevant nested guidance,
using the host's instruction rules. Inspect short project documentation, build
metadata, and relevant examples/configuration/tests. Treat documents as leads
and declared intent; check important behavioral claims against current source.

Start with a small inventory and targeted searches. Prefer available semantic
definition/reference tools for symbols; use text search for strings, configuration,
registration, and unsupported languages. Do not install tools just to begin.

Follow necessary cross-package or cross-repository dependencies. Skip unrelated
generated, vendor, and build trees unless the chosen behavior leads there.
A failed scoped search is not proof that a component is absent. Check filters or
unavailable dependencies before concluding.

Separate investigation depth from explanation length: inspect enough to ground
the answer, but present only the next useful piece. Do not read the entire repo
or generate a giant wiki before helping.

## Give a small orientation map

Explain the problem the project solves and the few components relevant to the goal.
Name real paths and important symbols; explain responsibilities and relationships,
rather than listing directories. Define project-specific terms as they arise.

Show how the current area connects to its callers, state, and outputs. Highlight
a relevant architectural boundary or invariant when supported by evidence.
Avoid assigning responsibility solely from filenames or familiar framework patterns.

## Trace one real scenario

Choose an existing command, request, example, or test as the entry point. For an
ML system, a batch, optimizer update, or checkpoint operation can be a useful
slice, but locate its actual implementation rather than assuming a standard loop.

Establish which configuration or variant is being traced. Follow:
- The trigger or entry point and the data entering it.
- The important calls or transformations, including conditions on the path.
- Where state is owned, read, changed, or persisted.
- The output or side effect and any relevant asynchronous handoff.

Inspect the actual wiring behind registries, factories, callbacks, dependency
injection, or distributed boundaries when present. Do not treat a static caller
or default setting as proof that a particular runtime path executes.

For a larger lesson, show a compact route and explain only its first meaningful
segment initially. Continue with the user's responses. At each stage, identify
where to look, what to notice, and why it matters. Extract current snippets
instead of reconstructing source. Link paths and symbols, with current line
references when available, using the host's supported link format.

Explain meaningful behavior rather than every line of syntax. Resolve a helper
only when necessary, then reconnect it to the scenario so the user does not lose
the thread. Use learn-concept briefly when missing conceptual knowledge blocks
understanding; return to the actual source afterward.

## Match claims to evidence

Distinguish naturally in the explanation:
- What inspected source and configuration establish.
- What a test asserts, including mocked or substituted dependencies.
- What was observed in a specific execution.
- What remains inferred, unresolved, or outside accessible code.

Use comments, design records, or relevant history for author intent. Otherwise
label a plausible rationale as an inference. Do not invent production settings,
ownership, runtime ordering, or historical motivations.

A test trace covers its scenario; a mocked adapter does not verify the real
integration. If code and documents conflict, explain the discrepancy. Re-check
affected references after edits or a checkout change.

## Verify only what helps understanding

Use a small existing test/example or debugger trace when it resolves a specific
uncertainty and is appropriate to the environment. Inspect its setup and likely
side effects first. Follow applicable execution instructions; avoid launching
training, provisioning services, changing data, or repairing a large environment
merely for orientation.

When execution is unavailable or disproportionate, continue with static analysis
and state the unverified part. Do not claim to have run or tested code unless done.
Learning is read-only by default: create notes/artifacts or edit the project only
when requested or otherwise authorized by the user.

## Choose representations and pace deliberately

Use a short map for structure, a sequence view for interactions, and concrete
values or state tables for transformations. Diagrams must name inspected entities;
show uncertain edges as uncertain. Build interactive HTML only when manipulating
or stepping through behavior adds useful understanding and the user wants an
artifact. Label simplifications and keep it tied to the real code.

Answer follow-ups directly and adapt depth. Do not append a quiz or permission
question after every paragraph. Pause at a natural boundary. Invite an occasional
prediction or navigation attempt after explaining enough, if the user wants it.
Use practice-concept for sustained learner-led exercises; do not silently turn
the tour into an exam or a project implementation.

## Finish at a useful boundary

Stop at the agreed scope, not after every file has been summarized. Briefly
recap the chosen path, key responsibility/boundary, and unresolved uncertainty.
Point to the next small set of files with a reason to read each when useful.

Describe observed progress without claiming whole-repo mastery. Carry the route
and open questions forward in the current session. Save a reading map or resumable
notes only when requested, and do not claim persistent memory without support.
