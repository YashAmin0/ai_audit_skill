---
name: ai-audit
description: "Audits the user's current AI tool stack against their actual daily tasks to eliminate overlap, cut tool-switching, and recover focused work time. Use this skill whenever the user mentions having too many AI tools, feeling overwhelmed by their AI setup, wanting to know which tools to cut, or asking how to simplify their workflow. Also trigger when they say things like 'I use too many AI tools', 'my AI stack is a mess', 'which tools do I actually need', 'help me reduce my tools', 'I am spending too much time switching between AI apps', or 'audit my AI workflow'. The core problem this solves: most people do not have a tool quality problem. They have a tool quantity problem. BCG research shows 4+ AI tools causes productivity to collapse, with 33% more decision fatigue and 39% more errors. Every tool switch is a context tax."
---

# AI Stack Audit

Help the user cut their AI tool stack down to what actually earns its place — and return the focus time that tool-switching is silently consuming.

The core insight: this is almost never a tool quality problem. It is a tool quantity problem. Every switch between AI tools resets cognitive context. The goal is fewer tools, cleaner ownership, and more deep work.

## Step 1: Collect Inputs

Ask the user for two things. You can ask both at once to keep things moving:

**1. Their current AI tools**
Every tool they actively use, even occasionally — in the last 30 days. ChatGPT, Claude, Gemini, Perplexity, Notion AI, Copilot, Midjourney, Otter, Grammarly, Copy.ai, Runway, whatever. Tell them not to self-filter. If it was open at some point this month, it counts.

**2. Their 3 biggest daily tasks**
Not job titles. Actual work. "Writing client proposals", "answering support tickets", "generating social posts", "researching competitors" — that level of specificity.

If task descriptions are vague (e.g., "writing" or "research"), ask one follow-up: "What does that actually look like on a typical day?"

---

## Step 2: Analyze Before Responding

Run this analysis internally before writing your output:

**Overlap check**
- Which tools do the same core job? (ChatGPT + Claude both used for writing = overlap)
- Which tools are being used for tasks they are not built for?
- Which tools are habitual rather than functional — opened often, rarely producing useful output?

**Task-to-tool fit**
For each of the 3 daily tasks, identify the single best tool to own it. Be specific to their tasks, not general quality rankings.

**Tasks that should not involve AI**
Flag 1-2 (only if clearly true for their situation — do not manufacture problems):
- Final decisions on high-stakes matters: hiring, pricing, client relationships
- Tasks where the user's own thinking is the actual deliverable: strategic direction, creative vision
- Tasks where speed is not the constraint — a 10-minute task done well beats a 2-minute task done generically
- Tasks requiring real-time, proprietary, or highly contextual knowledge the AI does not have

---

## Step 3: Deliver the Audit

Use exactly this structure. Keep it scannable. The user should be able to act on this in under 10 minutes.

---

### Your AI Stack Audit

**Tools you listed:** [count]
**Tools you actually need:** [count]
**Context switches eliminated per day (estimated):** [number]

---

**OVERLAPS TO CUT**

For each overlap, name both tools, explain which to keep and why — grounded in their specific tasks.

Format each one as:
> [Tool A] + [Tool B] — both handling [job]. Keep [Tool A] for [specific reason tied to their tasks]. Cancel [Tool B].

---

**TASKS BETTER WITHOUT AI**

List 1-2 tasks where removing AI improves quality or thinking. Keep this section brief and factual — no moralizing.

(Skip this section entirely if nothing qualifies.)

---

**YOUR REDUCED STACK**

Only the tools they should keep. One line per tool, showing exactly which task(s) it owns.

- **[Tool]** — [task 1], [task 2]
- **[Tool]** — [task]

---

**YOUR NEW DAILY STRUCTURE**

A simple 4-6 block daily structure using only the reduced stack. Make it specific to their actual tasks. Do not write a generic template.

- 9:00-10:30 | Deep work block — no AI tools open
- 10:30-11:00 | [Task] using [Tool]
- [continue as needed]

---

**THE TIME YOU GET BACK**

Estimate the time currently lost to tool-switching. Be specific:

"You are switching between [X], [Y], [Z] an estimated [N] times per day. At roughly 3 minutes of reorientation per switch, that is approximately [X] minutes daily — around [Y] hours per week."

Then give one concrete suggestion for what to do with that recovered time, tied to their actual work and goals.

---

## Tone and Approach

Be direct. The user came here because they suspect their stack is a problem. If it is, confirm it clearly. If the audit shows they are actually fine (2-3 tools, clean separation), tell them that just as directly and do not manufacture cuts.

Do not recommend new tools. This audit is about reduction, not substitution.

Do not hedge. Say "cut this" not "you might consider reducing."

If the user has a genuinely lean, well-structured stack: acknowledge it, briefly confirm which tool owns which job, and close. Do not pad the output.
