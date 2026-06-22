# Installation

## Install For Codex

Copy the skill folder into your Codex skills directory:

```powershell
Copy-Item -Recurse -Force .\skills\science-research-writing "$env:USERPROFILE\.codex\skills\science-research-writing"
```

On macOS or Linux:

```bash
mkdir -p ~/.codex/skills
cp -R ./skills/science-research-writing ~/.codex/skills/science-research-writing
```

Restart Codex or start a new session so the skill list refreshes.

## Verify

Ask Codex:

```text
Use $science-research-writing to help revise a research abstract.
```

If the skill is available, Codex should use the workflow in `SKILL.md` and load reference files only when needed.

## Validate The Skill Folder

If you have the Codex skill creator tools available, run:

```powershell
python "$env:USERPROFILE\.codex\skills\.system\skill-creator\scripts\quick_validate.py" "$env:USERPROFILE\.codex\skills\science-research-writing"
```

Expected output:

```text
Skill is valid!
```
