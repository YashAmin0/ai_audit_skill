# AI Audit Skill — Claude Code

A Claude Code skill that audits your AI tool stack, cuts the overlap, and returns the focus time that tool-switching is silently consuming.

## The Problem

Most people don't have a tool quality problem. They have a tool quantity problem.

BCG research shows 4+ AI tools causes productivity to collapse — 33% more decision fatigue, 39% more errors. Every switch between AI tools resets cognitive context. The result: you're paying for tools you barely use, and paying again in fragmented attention every time you jump between them.

## What This Skill Does

You tell it:
- Every AI tool you've opened in the last 30 days
- Your 3 biggest daily tasks (specific, not job titles)

It gives you:
- Overlaps to cut — which tools are doing the same job, and which one to keep
- Tasks that are better done without AI
- A reduced stack with clear ownership per task
- A daily structure built around your actual work
- A concrete estimate of how much time you're losing to context-switching

## Install

1. Copy the `ai-audit/` folder into your Claude Code skills directory:

```
~/.claude/skills/ai-audit/
```

Your directory should look like this:

```
~/.claude/skills/
└── ai-audit/
    ├── SKILL.md
    └── evals/
        └── evals.json
```

2. Restart Claude Code (or reload skills).

3. Trigger the audit by typing `/ai-audit` or describing the problem naturally:

> "I use too many AI tools and I'm not sure which ones I actually need."
> "Audit my AI workflow."
> "Help me cut down my AI stack."

## Usage

Claude will ask for your tools and tasks, then deliver a structured audit:

```
Your AI Stack Audit

Tools you listed: 9
Tools you actually need: 3
Context switches eliminated per day (estimated): 11

OVERLAPS TO CUT
...

YOUR REDUCED STACK
...

YOUR NEW DAILY STRUCTURE
...

THE TIME YOU GET BACK
...
```

## What It Won't Do

- Recommend new tools. This is about reduction, not substitution.
- Manufacture problems. If your stack is already lean, it will say so directly.
- Hedge. "Cut this" not "you might consider reducing."

## Evals

The `evals/evals.json` file includes 3 test cases covering:
- A bloated 9-tool stack with heavy overlap
- A developer stack with clear tool roles
- A lean 2-tool stack that needs no cuts

Use these to verify the skill is producing correct output after any modifications.

## License

MIT
