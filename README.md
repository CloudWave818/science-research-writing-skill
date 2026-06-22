# Science Research Writing Skill

![Status](https://img.shields.io/badge/status-v0.1.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Codex Skill](https://img.shields.io/badge/Codex-skill-black)

A Codex skill for helping researchers draft, revise, and diagnose STEMM research writing for publication.

This skill focuses on structure before surface polishing. It treats a research paper as a reader-facing narrative: each section, paragraph, and sentence should have a clear function.

中文简介：这是一个面向科研论文写作的 Codex skill，用于帮助研究者改写、诊断和构建英文 STEMM 论文。它优先处理论文结构、段落功能、研究空白、贡献表达和结论强度，而不是只做表层润色。

## Why This Skill

Many research writing problems are not grammar problems. A sentence can be grammatically correct but still fail because the reader cannot tell why the information is there, how it connects to the research question, or how strongly the authors are allowed to claim the result.

This skill helps Codex work like a research-writing coach:

- diagnose the function of each paragraph before rewriting it
- separate scientific content from reader-facing narrative
- reverse-engineer recent target articles instead of forcing one universal template
- calibrate claim strength to the evidence
- preserve technical meaning while improving publication style

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

## Quick Start

Install the full skill folder:

```text
skills/science-research-writing
```

into your Codex skills directory:

```text
~/.codex/skills/science-research-writing
```

Windows:

```text
C:\Users\<YourName>\.codex\skills\science-research-writing
```

Then start a new Codex session and invoke it explicitly:

```text
Use $science-research-writing to revise my Introduction.
```

See [install.md](install.md) for detailed installation steps.

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

## Example Workflows

### Introduction Diagnosis

Input:

```text
Use $science-research-writing to diagnose this Introduction. I want to submit to an environmental engineering journal.
```

Expected behavior:

- identify the current paragraph functions
- check whether the Introduction moves from broad territory to specific problem
- locate the research gap and whether it actually motivates the study
- revise the section only after the structural problem is clear

### Abstract Revision

Input:

```text
Use $science-research-writing to rewrite this abstract within 250 words.
```

Expected behavior:

- preserve factual content
- include context, aim, method, main result, and conclusion
- make the main result concrete
- avoid unsupported impact claims

### Discussion Claim Strength

Input:

```text
Use $science-research-writing to check whether this Discussion overclaims the results.
```

Expected behavior:

- distinguish evidence, interpretation, and speculation
- weaken causal language when the design does not support causality
- connect limitations to interpretation
- keep the final contribution clear

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

## What This Skill Does Not Do

- It does not verify scientific correctness or statistical validity.
- It does not replace journal instructions for authors.
- It does not decide authorship, ethics, or data availability requirements.
- It does not copy language from target papers.
- It does not reproduce copyrighted book text.

## Version

Current version: `v0.1.0`

This is an early public version. The core workflow is usable, but the skill should improve through real paper-revision examples and field-specific testing.

## Roadmap

- Add more worked examples for Introduction, Abstract, and Discussion revision.
- Add optional templates for reviewer-response writing.
- Add a target-article reverse-engineering worksheet.
- Add scripts for extracting section text from PDFs if a stable cross-platform approach is useful.

## Contributing

Contributions are welcome. Useful contributions include:

- clearer section models
- more field-tested checklists
- examples based on original or public-domain text
- installation fixes for different operating systems
- issue reports showing where the skill gave weak writing advice

Please avoid adding copyrighted book passages or copied journal-paper text.

## Attribution And Scope

This skill is inspired by genre-based and reverse-engineering approaches to scientific writing, including ideas popularized in Hilary Glasman-Deal's *Science Research Writing*. It is not affiliated with the author or publisher, and it does not reproduce the book text.

The skill provides writing support, not scientific validation. Users remain responsible for factual accuracy, ethical compliance, journal requirements, and authorship decisions.

## Installation

See [install.md](install.md).

## License

MIT License. See [LICENSE](LICENSE).
