# Design sources

Reviewed November 14, 2026. These references inform the design; they need not be
loaded on every use. Exact skill boundaries and instructions are design judgments.

## Explanation and practice

- [OpenAI Academy: Learn Difficult Concepts](https://academy.openai.com/en/public/clubs/higher-education-05x4z/blogs/learn-difficult-concepts-2026-05-18)
  (2026): plain explanations, technical depth, examples, then application and recall.
- [OpenAI: Study Mode](https://openai.com/index/chatgpt-study-mode/)
  (2025): scaffolding, self-pacing, participation, and feedback. Product rationale.
- [Anthropic: Teaching and learning AI](https://claude.com/resources/articles/anthropics-approach-to-teaching-and-learning-ai)
  (2026): agency, reflection, experimentation, diagrams, and interactive explainers.
- [Jane Street: Socratic Tutor](https://github.com/janestreet/agent_skills/blob/master/socratic-tutor/SKILL.md):
  one-at-a-time questions and demonstrated performance. Our skills allow direct
  explanation and omit its mandatory diagnostic, grading map, and strict
  questioning throughout. The instructions here are original.
- [Claude Code: Output styles](https://code.claude.com/docs/en/output-styles):
  distinguishes explanations from learner participation in implementation.
- [Anthropic: Coding skill formation](https://www.anthropic.com/research/AI-assistance-coding-skills)
  (2026): small randomized study learning Trio; completion can differ from
  comprehension. Associations between usage patterns and scores are not causal.
- [Bastani et al.: AI guardrails and learning](https://pmc.ncbi.nlm.nih.gov/articles/PMC12232635/)
  (2025): assisted performance can diverge from subsequent unaided performance.
  Students received instruction before practice. A guarded tutor removed
  detectable harm without an unaided gain over control.
- [Atkinson, Renkl, and Merrill: Fading worked examples](https://asu.elsevierpure.com/en/publications/transitioning-from-studying-examples-to-solving-problems-effects-/)
  (2003): non-AI experiments inform the bridge toward independent variations.
- [Josh Comeau: How To Learn Stuff Quickly](https://www.joshwcomeau.com/blog/how-to-learn-stuff-quickly/)
  (2021, updated 2025): guided learning, intentional experiments, tutorial fading,
  and related independent projects. Practitioner advice.

## Representations

- [OpenAI: Interactive math and science](https://openai.com/index/new-ways-to-learn-math-and-science-in-chatgpt/)
  (2026): manipulating variables exposes relationships; it does not establish
  that arbitrary AI-generated HTML improves learning.
- [Simon Willison: Interactive explanations](https://simonwillison.net/guides/agentic-engineering-patterns/interactive-explanations/)
  (2026): a concrete example of inspecting an algorithm through animation.
- [Andy Matuschak: How Might We Learn?](https://andymatuschak.org/hmwl/)
  (2024): authentic goals, dynamic media, and contextual support. A design vision.
- [Karpathy: Clear explanations and output formats](https://x.com/karpathy/status/2105819303471976479):
  indexed copies recommend simplified technical language, diagrams, HTML, and
  videos. The original was inaccessible during research; it is not the sole
  basis for any instruction. Use plain language flexibly, not mandatory ASD-STE100.

## Learning a codebase

- [OpenAI: Understand large codebases](https://learn.chatgpt.com/use-cases/codebase-onboarding):
  responsibilities, request flow, validation/state changes, and next files to read.
- [Anthropic: Common workflows](https://code.claude.com/docs/en/common-workflows):
  overview, relevant components, interactions, then execution flow. Product guidance.
- [Anthropic: Large codebases](https://code.claude.com/docs/en/large-codebases):
  scope context and navigation to relevant packages and applicable instructions.
- [Simon Willison: Linear walkthroughs](https://simonwillison.net/guides/agentic-engineering-patterns/linear-walkthroughs/)
  (2026): deliberate reading order and tool-extracted code snippets. A small-app
  practitioner example, not evidence for exhaustive monorepo tours.
- [matklad: ARCHITECTURE.md](https://matklad.github.io/2021/02/06/ARCHITECTURE.md.html)
  (2021): coarse component maps, important symbols, boundaries, and invariants.
- [Birgitta Boeckeler: Onboarding with AI](https://www.martinfowler.com/articles/exploring-gen-ai/09-ai-help-onboarding-codebase.html)
  (2024): real exploration including missing domain/multi-repo context and failed
  setup attempts. Useful discovery does not establish complete understanding.
- [Sillito et al.: Questions Programmers Ask](https://www.cs.ubc.ca/~murphy/papers/other/asking-answering-fse06.pdf)
  (2006): observational studies catalog questions from initial focus points through
  connected models of behavior. Predates AI; informs question-driven navigation.
- [CodeMap author project](https://gaojie058.github.io/code-map/)
  (2026): overview-to-detail navigation, small auditor interviews and prototype study.
  Perceived usefulness and interaction changes are not measured learning gains.
- [Faster but Not Wiser](https://arxiv.org/abs/2511.02922)
  (v3, September 2026): 15 graduate students, improved assisted task performance
  without a significant overall comprehension gain. Small study; verification-loop
  associations do not prove causality. Earlier versions differ in sample reporting.
- [Feeling Easier, Working Harder](https://arxiv.org/abs/2611.12019)
  (November 2026): 20 novices reading Java snippets; added measured cognitive load
  and no detected comprehension gain, with ceiling effects. Do not generalize this
  result to all repositories, engineers, or forms of AI help.

Use these sources to distinguish source-backed navigation from directory summaries,
and task completion from understanding. The exact learn-codebase workflow is an
original design inference, not a validated research intervention.

## Starting projects and completing tasks

- [OpenAI: Best practices](https://learn.chatgpt.com/docs/learn/best-practices):
  goal, relevant context, constraints, and observable completion. Plan/interview
  when ambiguity or complexity warrants it, not for every small change.
- [OpenAI: Idea to proof of concept](https://learn.chatgpt.com/use-cases/idea-to-proof-of-concept):
  a small useful prototype, verification, and scoped iteration. Its visual/browser
  workflow is web-specific, not a required process for ML or CLI projects.
- [OpenAI: Using Goals in Codex](https://developers.openai.com/cookbook/examples/codex/using_goals_in_codex)
  (2026): outcome, verification surface, constraints, boundaries, and blocked stop
  conditions. These skills do not create a persistent Goal or scheduled task.
- [OpenAI: Rethinking skills and prompts](https://developers.openai.com/blog/rethinking-skills-and-prompts-for-gpt-6-astra)
  (September 2026): specific triggers, contextual reading, proportional checking,
  and completion boundaries. Model-specific advice informs general decision rules;
  these skills do not assume identical behavior across models.
- [OpenAI: PLANS.md for multi-hour work](https://developers.openai.com/cookbook/articles/codex_exec_plans):
  observable milestones and bounded feasibility experiments. Its full document
  template is not mandatory for small work.
- [Anthropic: Claude Code best practices](https://code.claude.com/docs/en/best-practices):
  provide missing project context, supply a runnable check, and review actual
  requirements. These skills ask only material questions and avoid blanket
  persistence or approval rituals.
- [Martin Fowler: Yagni](https://martinfowler.com/bliki/Yagni.html)
  (2015): defer speculative capabilities while preserving necessary code health.
- [Birgitta Boeckeler: Spec-driven development tools](https://www.martinfowler.com/articles/exploring-gen-ai/sdd-3-tools.html)
  (October 2025): practitioner evaluation highlights excessive process on small
  changes. Use specifications to reduce ambiguity, not manufacture work.
- [Simon Willison: Agentic manual testing](https://simonwillison.net/guides/agentic-engineering-patterns/agentic-manual-testing/)
  (2026): execute the relevant behavior; unit-test success alone can miss practical
  failures. Use the simplest appropriate check rather than installing every tool.

These are engineering recommendations and experience reports, not experimental
validation of these exact skills. Separate project direction from bounded task
execution; let the user's intent determine planning, learning, and action scope.
Clarification ends when enough is known for the next sound action. Keep required
checks while avoiding speculative work and repeated verification without reason.

## Interpretation

Use explanation-led and practice-led workflows as complementary defaults.
Choose media because it reveals a mechanism. Ask questions that clarify the next
step or engage reasoning the learner is ready to do. Judge learning through
observed understanding and independent attempts; reassess through actual use.
