# Claude Skills

Two Claude Code skills for structured decision-making.

- **`requirementor`** — forces explicit requirement analysis before starting something non-trivial (a build, a decision, a commitment).
- **`musk-algorithm`** — Elon Musk's 5-step process (question requirements → delete → simplify → accelerate → automate) for auditing an existing plan, process, or system.

## Install

**Personal (all  projects):**
```bash
git clone <https://github.com/tdurand06/Skills>
cp -r Skills/.claude/skills/* ~/.claude/skills/
```

**Project:**
```bash
cp -r Skills/.claude/skills .claude/skills
git add .claude/skills && git commit -m "Add requirementor and musk-algorithm skills"
```

## Use

Nothing to configure. Claude Code auto-discovers any `.claude/skills/*/SKILL.md` and triggers it when your prompt matches its description, e.g. "let's analyze the requirements" or "how should i think about the engineering of this system?"

You can also invoke explicitly: *"Apply the Musk algorithm."*

## License

MIT
