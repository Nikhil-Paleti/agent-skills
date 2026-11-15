# Agent skills

Personal skills for learning and engineering. Start small, use them on real work,
and refine specific behavior when it helps or gets in the way.

| Skill | Use it for | Default behavior |
| --- | --- | --- |
| [learn-concept](skills/learn-concept/SKILL.md) | Understanding an unfamiliar technical idea | One concrete example, clear mechanics, manageable conversational steps |
| [practice-concept](skills/practice-concept/SKILL.md) | Developing independent ability | One small challenge, learner attempt, targeted feedback, gradually less help |
| [learn-codebase](skills/learn-codebase/SKILL.md) | Navigating and understanding a repository or feature | A compact source-linked route, then one meaningful stop at a time |
| [start-project](skills/start-project/SKILL.md) | Turning a rough project idea into a useful first result | Material clarification, a small verifiable milestone, then action within scope |
| [do-project-task](skills/do-project-task/SKILL.md) | Completing a bounded change in an existing project | Relevant inspection, coherent implementation, appropriate verification |

## Try them

With an agent that can read this repository, ask:

> Read skills/learn-concept/SKILL.md and help me understand tiled GEMM.
> I understand vector addition and one thread per element.

> Read skills/practice-concept/SKILL.md and help me implement a small tiled GEMM
> myself. I want hints and feedback, and I want to write the core code.

> Read skills/learn-codebase/SKILL.md and help me understand how checkpoint
> saving works in this repository. Start with a small map, then walk through
> the first meaningful part of a real save path.

> Read skills/start-project/SKILL.md and help me start a tool for comparing GPU
> kernel benchmarks. Clarify what matters and help me get a useful first version.

> Read skills/do-project-task/SKILL.md and fix the reported checkpoint bug in
> this repo. Resolve any material ambiguity, implement it, and verify the result.

Short requests are fine. The agent should clarify missing context only when it
changes the approach. Say "keep explaining," "show a smaller example," "let me try,"
or "just tell me" to steer it. For project work, say whether you want a plan,
guided implementation, or delegated completion when that distinction matters.
Clear execution requests should proceed through verification without approval
after each routine step.

Each skill has a portable SKILL.md and optional Codex UI metadata in
agents/openai.yaml. Keeping files in this repository does not automatically
install them; use your agent's supported discovery or installation mechanism.
They need no custom services or packages. Visuals and execution use whatever
capabilities the host agent actually has.

## Review and refine

Keep the prompt and response when something feels wrong. Refine the smallest
relevant instruction. Check both a learning request and a narrow question so
a fix does not turn every interaction into a lesson.

See [SOURCES.md](SOURCES.md) for design references. These skills are original
adaptations, not copied provider prompts or experimentally validated recipes.
