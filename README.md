# Science Research Writing Skill

A Codex skill for helping researchers draft, revise, and diagnose STEMM research writing for publication.

This skill focuses on structure before surface polishing. It treats a research paper as a reader-facing narrative: each section, paragraph, and sentence should have a clear function.

## What It Does

Use this skill for tasks such as:

- revising an Introduction so it moves from research territory to gap, aim, and contribution
- improving Methods for reproducibility, rationale, and sequence
- separating Results from Discussion-style interpretation
- strengthening a Discussion without overclaiming
- writing or revising Abstracts and Titles
- checking claim strength, terminology consistency, paragraph function, and reader flow
- reverse-engineering target journal articles to build field-specific writing models

## Skill

| Skill | Purpose |
| --- | --- |
| `science-research-writing` | Publication-oriented STEMM research writing coach using section models, language functions, and checklists. |

## Example Prompts

```text
Use $science-research-writing to revise this Introduction for a materials science journal.
```

```text
Use $science-research-writing to diagnose the logic of this Discussion section before I polish the English.
```

```text
Use $science-research-writing to rewrite this abstract within 250 words for a structured journal abstract.
```

```text
Use $science-research-writing to compare these three target papers and extract an Introduction model for my paper.
```

## Repository Layout

```text
science-research-writing-skill/
  README.md
  install.md
  LICENSE
  skills/
    science-research-writing/
      SKILL.md
      agents/
        openai.yaml
      references/
        section-models.md
        language-functions.md
        checklists.md
```

Install the whole `skills/science-research-writing` folder. Do not copy only `SKILL.md`, because the skill refers to files in `references/`.

## Design Notes

The skill is intentionally compact:

- `SKILL.md` contains the core workflow and triggering instructions.
- `references/section-models.md` contains section-level models.
- `references/language-functions.md` contains adaptable function-based phrase patterns.
- `references/checklists.md` contains review checklists.

This keeps Codex from loading long reference material unless it is needed for the task.

## Attribution And Scope

This skill is inspired by genre-based and reverse-engineering approaches to scientific writing, including ideas popularized in Hilary Glasman-Deal's *Science Research Writing*. It is not affiliated with the author or publisher, and it does not reproduce the book text.

The skill provides writing support, not scientific validation. Users remain responsible for factual accuracy, ethical compliance, journal requirements, and authorship decisions.

## Installation

See [install.md](install.md).

## License

MIT License. See [LICENSE](LICENSE).
