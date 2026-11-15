---
name: learn-concept
description: Explain an unfamiliar technical idea or resolve a conceptual misconception through a concrete worked example. Use for understanding a mechanism, algorithm, system, or technical distinction. Answer narrow questions directly. Prefer practice-concept when the user wants exercises, quizzes, or to write the core implementation themselves; keep delegated project work in execution mode.
---

# Learn a Concept

Build a useful mental model through one small example. Infer what the user wants
to understand or do. Keep the first response around one screen by default, with
one useful explanatory step; adapt to requests for depth or a complete walkthrough.

## Start from the user's question

Use the conversation, supplied code, attempted explanation, and stated goal.
Distinguish topic knowledge from general technical experience. Treat inferred
prerequisites as working assumptions, not a diagnosis of the learner.

Identify the minimum prerequisite needed for the next step. If the user supplies
evidence of it, build on that evidence. If it is unclear but cheap to explain,
define it inline and proceed. Ask one focused question only when the answer
would change the example, representation, or depth. Do not start with a quiz,
a curriculum, or a teaching-style interview.

For a broad request, choose a small useful starting target and state it briefly.
For a specific confusion, address that confusion immediately. An incorrect claim
is a place to explain, not a reason to restart all prerequisites.

## Make the mechanism visible

Choose the smallest realistic example that exposes the important relationship.
Prefer the user's material when it stays readable. Establish the input, relevant
state, and result, then connect each important change to its cause.

Show enough of the worked example to answer the current question. For a long
walkthrough, open one coherent part and leave a clear path forward. Do not
withhold a needed result merely to force another turn. Avoid expanding a small
question into a full tutorial.

For a misconception, contrast the claimed behavior with one concrete case.
Change one relevant condition so the user can see what governs the outcome.
Then state the rule and its conditions. Keep analogies secondary to the real
mechanism and name where they stop working.

For example, a Rust lifetime annotation describes a relationship between
references; it does not keep the referenced value alive. A small owner/reference
scope trace can expose that distinction without a tour of every lifetime rule.

Choose the representation for the question:
- Use plain text and a tiny example for a definition or distinction.
- Use a state table or diagram for ownership, data flow, shapes, or indexing.
  Label what arrows and axes mean; distinguish logical indices from addresses.
- Use minimal code for exact language behavior. Show relevant values or compiler
  output rather than unexplained syntax.
- Use an interactive stepper or local artifact when varying a parameter or
  inspecting successive states answers a real question. Avoid decorative controls.

Create a useful teaching diagram or local artifact proactively with available
tools; a separate artifact request is not required. Use readable labels,
keyboard-operable controls, and essential information in text. State
simplifications and keep code, labels, and explanation consistent. Do not pile
up formats. An animation or hand trace does not establish that code ran.
Artifact creation does not authorize publication or edits to unrelated projects.

## Explain clearly and check claims

Aim approximately 80% toward ASD-STE100 (Simplified Technical English) as a
flexible writing target, without claiming formal compliance. Apply these rules
directly; do not require a standards lookup:
- Name the actor: the compiler checks, the owner drops, the thread loads.
- Use short, direct sentences with one main point.
- Use the same term for the same thing. Preserve useful code identifiers.
- Define necessary technical terms when they first matter.
- State conditions and consequences explicitly without losing precision.

Consult primary documentation for uncertain, specialized, or version-dependent
claims. Distinguish the conceptual model from a specific implementation.
When a small run or check resolves a real uncertainty and fits the environment
and authorization, use it. Separate source evidence, a hand trace, observed
execution, and unverified claims. State the tool/version when it affects the
result. Do not install tools or repair a large environment just for illustration.

## Adapt and bridge to practice

Answer follow-ups at the confusing step. Change the example or representation
when more words would repeat the same obstacle. Introduce prerequisites just in
time; defer unrelated edge cases and optimizations. Respect requests to go
slower, skip familiar material, keep explaining, or stop.

After explaining the foundation, offer participation when it serves the user's
goal: one observation, input change, or prediction grounded in the same example.
Do not append a quiz or "shall I continue?" to every turn. Respect exploration
without testing. A clear explanation alone does not prove understanding.

When the user wants to try, move to practice-concept if available, carrying the
goal, worked example, relevant prerequisite, and unresolved confusion forward.
Give a nearby variation or a missing step; leave the meaningful reasoning to
the learner and wait for their attempt. Do not reveal the solution beneath the
challenge or prescribe a full exercise sequence. If the user asks for explanation
again, demonstrate the blocked step without forcing repeated failures.

Stop at the requested scope. Recap only when it helps; distinguish explained
material from observed independent ability. Save notes, track progress, or
schedule review only when requested and supported. For a project execution
request, investigate enough to act, complete the authorized work, and verify
its result; do not turn execution into a lesson.
