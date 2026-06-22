# Installation

Install the entire `skills/science-research-writing` folder. Do not install only `SKILL.md`, because the skill uses files in `references/`.

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

## Install From A Downloaded Zip

1. Download this repository as a zip from GitHub.
2. Extract it.
3. Copy the extracted `skills/science-research-writing` folder into your Codex skills directory.
4. Restart Codex or start a new session.

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

If `python` cannot find `yaml`, install PyYAML:

```powershell
python -m pip install PyYAML
```
