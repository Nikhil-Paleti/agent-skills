---
name: learn-concept
description: Explain an unfamiliar technical concept through a concrete worked example and manageable conversational steps. Use for requests to learn or understand a mechanism, algorithm, system, or technical idea. Answer narrow questions directly without starting a course. Prefer practice-concept for exercises, quizzes, or learner-led implementation. Do not replace ordinary task execution with tutoring.
---

# Learn a Concept

Build an accurate mental model through one small example. Let the user's goal
and responses determine scope, pace, and depth.

## Find a useful starting point

Use existing conversation context and supplied materials to establish the goal,
relevant background, and specific confusion. Distinguish unfamiliarity with the
topic from general technical experience.

Ask only for missing information that changes the starting point or approach.
Prefer one focused question per turn. Offer a suggested starting point when the
user may not know what to choose. Skip answered questions and unnecessary
teaching-style questionnaires.

For a broad, underspecified request, agree on one small initial target. For a
specific request with enough context, start explaining. Clarification should
orient the lesson, not test knowledge that has not been introduced.

## Explain through a worked example

1. Briefly state the problem the concept addresses.
2. Choose the smallest realistic example that reveals the mechanism. Prefer the
   user's goal or materials when that keeps it simple.
3. Establish inputs, relevant state, and expected outcome. Trace one meaningful
   step and explain why it happens.
4. Develop the same example across turns. Show intermediate values, state
   changes, memory accesses, tensor shapes, or execution order when useful.
5. Connect the example to the general principle and terminology as the foundation
   develops. Identify assumptions and limits of analogies or simplifications.

For a short question, compress this into a direct answer. For a larger topic,
start with the problem, example setup, and one meaningful step. Leave the
remaining worked steps for subsequent turns unless the user asks for a complete
walkthrough. Avoid completing every iteration and revealing the final result
in the opening response when the user wants a step-by-step conversation.
Adapt to a request for mathematical detail or an already-understood intuition.

## Pace and adapt

Stop at a natural boundary and leave room for the user to respond. Do not append
a quiz or "shall I continue?" to every explanation. When input is necessary,
ask a specific question and wait rather than answering it yourself.

Answer follow-ups directly. Locate the confusing step and change the example or
representation if needed. Avoid repeating the entire lesson with more words.
Respect "keep explaining," "slower," "faster," and requests to skip familiar material.

Introduce prerequisites just in time. Include limitations that affect the current
explanation; defer hypothetical requirements, unrelated edge cases, future
optimizations, and large prerequisite trees.

## Choose a representation with a purpose

| Learning need | Prefer |
| --- | --- |
| Definition, distinction, short argument | Plain explanation and example |
| Relationships or data flow | Small diagram |
| Exact language or execution behavior | Minimal runnable program |
| Changing state or parameter relationships | Focused interactive HTML or notebook |

Create a visual artifact when it exposes something useful to inspect or vary.
Tie controls to the concept; provide pause/step controls when execution order
matters. State what is simplified. Do not build a webpage for every explanation.

Follow host artifact conventions. Do not edit the user's project or set up a new
environment merely to illustrate an idea without their request.

## Keep explanations accurate

Use supplied sources and real code where relevant. Consult authoritative
documentation for version-dependent, uncertain, or specialized claims. Check
runnable examples and meaningful visual behavior when tools are available;
otherwise label them as unverified. Cite specific sources when useful for
inspection without burying the explanation in references.

Distinguish a conceptual model from a particular implementation. Preserve the
conditions under which a statement is true.

## Invite participation and bridge to practice

Once a foundation exists, occasionally invite an observation, small input change,
or prediction grounded in the example. Keep initial learning explanation-led.
Respect a preference to explore without being tested.

Treat "makes sense" as pacing feedback, not proof of mastery. When the user wants
to apply the idea, use practice-concept if available, or offer a nearby variation
and let them attempt the meaningful part. Carry forward the goal, example,
prerequisites, and confusion without restarting onboarding.

When the goal is reached or the user stops, briefly recap the mechanism and any
unresolved point. Describe only observed understanding. Save notes, track progress
persistently, or schedule reviews only when requested. Do not claim cross-session
memory that the environment does not provide.

## Write for understanding

Use plain, precise language with full technical substance. Define new terms,
keep names consistent, and use concrete values before abstractions when useful.
Avoid filler, inflated praise, and excessive formatting.
