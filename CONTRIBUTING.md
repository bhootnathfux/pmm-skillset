# Contributing to PMM Skillset

Thanks for considering contributing. This project is opinionated by design — every skill encodes a specific PMM framework, not generic marketing advice. Contributions should match that bar.

---

## How to Contribute a Skill

### 1. Check the Roadmap

Before building a new skill, check the [Full Skill Roadmap](README.md#full-skill-roadmap) in the README. If the skill you want to build is already listed, open an issue to claim it and discuss the approach before writing code.

If the skill isn't on the roadmap, open an issue describing:
- What the skill does (one sentence)
- Who it's for (specific PMM scenario)
- What artifact it produces
- Which existing skills it connects to

### 2. Skill Structure

Every skill follows this structure:

```
skills/tier-X/skill-name/
├── SKILL.md              # Required. The skill definition.
└── examples/             # Optional. Example outputs.
    └── *.md or *.html
```

### 3. SKILL.md Format

```yaml
---
name: skill-name
description: "When to trigger this skill. Include natural language trigger phrases."
metadata:
  version: 1.0.0
  author: Your Name
  category: product-marketing
---
```

After the frontmatter, the skill should include:

- **Expert persona** — Who the AI is when running this skill
- **Core question** — The one question the skill answers (bold, quoted)
- **Acts overview** — What the skill does in sequence
- **Conversation Flow Rules** — Pacing, confirmation gates, push-back rules
- **Before You Start** — Mode selection (A/B/C/D pattern)
- **Prerequisites** — What the user needs before starting
- **Steps with quality tests** — Every step has scoring rubrics, minimum viable thresholds, and specific push-back examples
- **Output template** — The exact format of the final artifact
- **Related Skills** — What to run before/after

### 4. Naming Rules

- Lowercase letters, numbers, hyphens only
- Name must match the directory name
- No consecutive hyphens, no starting/ending with hyphens

### 5. Quality Checklist

Before submitting:

- [ ] Skill produces a specific, shareable artifact — not just advice
- [ ] Every step has a quality test with a scoring rubric
- [ ] Push-back examples show what rejection looks like (not just what good looks like)
- [ ] Prerequisites reference other skills where relevant (`/positioning-audit`, etc.)
- [ ] Output template is presentation-ready markdown — clean headers, no instruction text
- [ ] "Related Skills" section connects the skill to the ecosystem
- [ ] Tested end-to-end: ran the skill with a real scenario and the output is usable

---

## Reporting Issues

If a skill produces weak output, open an issue with:
- Which skill you ran
- The inputs you provided (anonymize if needed)
- What the output was
- What you expected instead

---

## Code of Conduct

Be direct, be helpful, skip the fluff. Same energy as the skills themselves.
