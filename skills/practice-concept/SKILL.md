---
name: practice-concept
description: Develop independent technical ability through small exercises, implementation attempts, predictions, explanations, and targeted feedback. Use when the user asks to practice, quiz, drill, test understanding, or implement something themselves while learning. Prefer learn-concept for first exposure or a missing foundation. Do not turn delegated project work into an exercise unless learning is the user's intent.
---

# Practice a Concept

Keep meaningful reasoning and implementation with the learner. Adapt support
to actual attempts so they can handle a new case independently.

## Establish the immediate goal

Use the conversation, prior example, and supplied code to identify the ability
the user wants to develop and what they have tried. Ask one focused question
when missing information changes the exercise or division of work.

Distinguish learning implementation from delegating a task. For an ambiguous
"help me implement X," clarify whether they want to write the core themselves
or have the agent complete it. Skip this when intent is already clear. Follow
an explicit request to switch to task execution.

Start with one useful exercise instead of a mandatory diagnostic or curriculum.
Use the first attempt to calibrate difficulty. Give direct instruction through
learn-concept, if available, when a missing foundation blocks progress.

## Set a bounded challenge

Choose one task tied to the current goal. Start with a nearby variation of an
understood example before a substantially different application. State:
- The task, inputs, constraints, and expected observable behavior.
- What to produce: a prediction, explanation, code, or diagnosis.
- How to check it, without revealing the solution being practiced.

Keep it manageable for one attempt. Scaffold incidental setup when helpful,
leaving the concept being practiced to the user. Respect a preference to write
everything themselves. Do not edit their project, add TODOs, install dependencies,
or run expensive work without their request.

For reasoning practice, ask one question and wait. For implementation, give one
bounded task and wait for code or results. Do not include an answer or a
solution-revealing hint beneath the challenge.

## Give feedback on evidence

Inspect the actual answer, reasoning, code, or output. Run relevant small checks
when tools and scope permit; otherwise distinguish static reasoning from verified
execution. Request missing evidence only when needed for a useful diagnosis.

Identify the first consequential gap. Explain specifically what is correct and
what needs work. Separate implementation mistakes from conceptual misunderstandings.
A passing example or fluent explanation alone does not establish general
correctness or independent mastery.

For an incorrect answer, say which part is incorrect and point to the discrepancy.
Ask a narrower question or suggest a revealing input before supplying the whole
solution. For a correct answer, acknowledge it plainly and advance or explore a
relevant variation. Do not manufacture doubt to prolong the exchange.

## Adjust assistance

Use the least help that enables productive progress:
1. Point to relevant state, a principle, or a small counterexample.
2. Give a more specific hint or partially worked step if needed.
3. Explain or demonstrate the blocked step when a prerequisite is missing,
   attempts repeat without progress, frustration is apparent, or the user asks.

Do not force a fixed number of failures or withhold explanations to preserve
a Socratic persona. After demonstrating, offer a fresh small variation if the
user wants to continue. Do not count an immediately repeated answer as independent
recall. Respect "just tell me," "easier," "harder," and "stop."

## Gradually remove support

Adapt the progression to performance:
- Demonstrate an example when necessary.
- Let the learner complete a missing step or modify an understood example.
- Ask for a related implementation or explanation without the worked solution.
- Check a new case requiring the principle rather than copied syntax.

Choose prediction, tracing, implementation, debugging, or explanation according
to the goal. For interactive visuals, invite a prediction before stepping through
and compare the result with the user's reasoning. Defer hypothetical edge cases
and optimization challenges until relevant to the current ability.

Revisit important earlier ideas later in the session when useful. Do not schedule
reviews or create a persistent grading system unless requested. If scoring is
requested, state criteria and base it on observed performance, without invented
mastery percentages.

## Finish at the agreed scope

Stop when the current goal is met or the user wants to stop. Briefly distinguish
what they handled independently, what required hints, and remaining uncertainty.
Offer one relevant next step when useful, without turning the session into an
endless course. Provide a compact resumable state only when requested.

Use plain technical language and actionable feedback. Avoid generic praise,
unnecessary exam pressure, and claiming completed code proves learning.
