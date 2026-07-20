---
name: musk-algorithm
description: Apply Elon Musk's 5-step engineering algorithm to a part, process, system, or plan. Use when the user wants to interrogate a design, a workflow, a job description, a deliverable, or any artifact before committing more resources to it. Triggers on phrases like "apply the Musk algorithm", "let's delete what we can", "make requirements less dumb", "simplify this", or when reviewing a plan, system, or process that may have accumulated cruft.
---

# Musk algorithm

Use this skill when interrogating an existing design, process, plan, or system. Walk the 5 steps in strict order. The order matters: skipping ahead causes the optimization step to entrench things that should have been deleted, and the acceleration step to dig the grave faster.

## When to use

Apply when the user:
- Is about to commit significant resources (time, money, headcount) to an artifact.
- Wants to interrogate a plan, system, process, or specification.
- Says "let's apply the Musk algorithm" / "make this leaner" / "delete what we can" / "we should simplify before optimizing".
- Has a working but bloated system that needs an audit.

Do NOT use for greenfield creative ideation (no artifact to interrogate yet) — use a different framework (e.g. requirements analysis via the requirementor skill).

## The 5 steps — in order

### 1. Make requirements less dumb

The requirements are dumb regardless of who gave them, especially if a smart person did. Walk each requirement and:

- **Name the source**: who specifically said this requirement was necessary? Every requirement / constraint must come with a name — not "the team", "the customer" generically. A specific person.
- **Challenge the requirement**: under what conditions would this be wrong? What if it didn't exist?
- **Distinguish necessary vs. inherited**: did this come from a real constraint, or from "we've always done it this way"?

Output: an annotated list of requirements with each one tagged by source and confidence.

### 2. Try very hard to delete the part or the process

This is the most important step.

- **Bias check**: the default human bias is "let's keep this just in case." Resist it.
- **Delete rule**: if you are not adding deleted things back ~10% of the time, you are not deleting enough. (You should occasionally find yourself adding things back — that proves you tried hard to delete; if you never have to add anything back, you didn't try hard enough.)
- **For each part or process**: ask "what breaks if we delete this?" If the answer is speculation, delete it. If the answer is concrete and you can name what breaks, keep it.
- **Apply to people too**: meetings, reports, roles, sign-offs.

Output: a list of deletions made + any add-backs after testing.

### 3. Simplify or optimize

**Only now** — after steps 1 and 2 — do you simplify what remains.

- **The #1 problem of smart engineers**: they optimize a thing that should not exist. Steps 1 and 2 prevent this.
- **Simplify before optimize**: reduce complexity first, then improve performance within the simpler shape.

Output: the simplified version.

### 4. Accelerate the cycle time

**Hold off on this until 1-3 are complete.** Accelerating a broken or bloated process digs the grave faster.

- **Cycle time**: how long from problem identified to solution shipped?
- **What's the limiting factor?** Address it. Then re-ask.
- **Iterate weekly or daily** on shortening the loop.

Output: the limiting factor named, and a concrete intervention to shorten the cycle.

### 5. Automate

**Last.**

- Automating a bad process scales the badness.
- Automating an over-engineered process locks in the over-engineering.
- Once steps 1-4 are done, the remaining thing is worth automating.

Output: candidates for automation, prioritized by ROI on the deletions and simplifications you already made.

## How to apply in conversation

When invoked:

1. Ask the user what artifact (part, process, plan, system) they want to interrogate.
2. Walk the 5 steps explicitly, one at a time, narrating what you are doing.
3. At each step, surface the output for the user's review before moving to the next step.
4. End with a punch list: deletions made, simplifications proposed, cycle-time intervention named, automation candidates listed.

## Anti-patterns

- Optimizing before deleting (step 3 before step 2).
- Adding requirements without naming the source (step 1 done loosely).
- Skipping step 2 because deletion feels risky — that is the whole point of the step.
- Calling something "automation" when it just hides complexity.
