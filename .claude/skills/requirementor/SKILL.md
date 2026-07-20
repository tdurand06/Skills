---
name: requirementor
description: Force explicit requirement analysis before any implementation work. Use whenever a user is about to build, write, choose, or commit to something — especially when the direction itself is uncertain. Triggers on phrases like "let's start building", "I want to write X", "should I take this role / pick this approach", "let's apply the requirementor", or any moment where premature execution would optimize in the wrong direction.
---

# Requirementor

Choose the direction before accelerating toward it. This skill prevents premature implementation by forcing explicit requirement analysis at the moment a user is about to commit resources to a path.

## When to use

Apply when the user is about to:
- Start building, writing, or implementing something non-trivial.
- Make a significant decision (career, project scope, technology choice, hire, architecture).
- Optimize a process or refine an output.

The signal: someone is moving toward execution before the destination is clearly named. The requirementor's job is to slow this down for the duration of one structured pass.

Skip this skill if requirements are already explicit, named, and validated.

## The pass — 5 deliberate checks

### 1. Name the actual goal in one sentence

Force a single-sentence goal. If the user cannot write it, the requirements work has not been done.

- **Test**: can a smart outsider read this sentence and tell you whether something I built passes or fails?
- **Sharpen**: replace vague abstractions ("better", "good", "useful") with concrete targets ("response time under 100ms", "I am the person someone calls when they need X").

### 2. Name each requirement with its source

Borrowed from Musk step 1. Every requirement / constraint must come with a named source (not "the team" or "the customer" generically — a specific person, document, or observed pain point).

Tag each one with:
- **Source**: who or what made this a requirement?
- **Confidence**: how sure are we this is real (high / medium / low)?
- **Cost of being wrong**: small / medium / large.

### 3. Stress-test the requirements

For each requirement, ask:
- **Under what conditions would this be wrong?**
- **What would have to be true for me to drop this?**
- **Is this a real constraint or a cultural artifact?**
- **What is the dumb version of this requirement, and what would it look like to fix it?**

Drop or downgrade any requirement that cannot survive this pass.

### 4. Distinguish must-have vs. nice-to-have

Force a binary classification on every surviving requirement. No middle ground.

- **Must-have**: failure of this requirement is a failure of the whole thing.
- **Nice-to-have**: deferrable; will be addressed in a later iteration or not at all.

If everything is "must-have", you have not classified — try again.

### 5. State the direction before moving

End with a short paragraph the user signs off on:
> "Given these named requirements, the direction I am committing to is [direction]. I am accepting trade-offs: [trade-offs]. I will revisit this if [trigger condition]."

The trigger condition is the most important sentence: it is the explicit signal under which the direction itself gets re-examined, not just iterated on.

## How to apply in conversation

When invoked:

1. Ask the user what they are about to build / decide / commit to.
2. Walk steps 1-5 deliberately, one at a time. Each step has its own output.
3. Push back on vague language ("better", "scalable", "good fit") — make the user produce concrete targets.
4. End with the direction statement in step 5, written in their own words.

This is a one-pass tool — do not loop indefinitely. The output is a frozen set of requirements + a direction + a re-examination trigger.

## Anti-patterns

- Letting requirements be lists without named sources (looks rigorous, is not).
- Accepting "I'll know it when I see it" — that is a defer to step 0, not a requirement.
- Classifying everything as must-have.
- Skipping step 5 (the direction statement) because "we already know what we're doing."
- Using this skill on small / clear / reversible decisions — it is a heavy pass, reserve for things worth structuring.

## Why this exists

People (and Claude) frequently jump to optimizing or executing before the destination is clearly defined. The cost of running in the wrong direction at high speed is much higher than the cost of pausing to confirm direction. This skill makes that pause structured, finite, and concrete — so the rest of the work can move fast.
